# Planetly_assigment
Updated 4 minutes ago  This is an assignment from Planetly. The data is taken from Kaggle, two datasets: GlobalLandTemperaturesByCity.csv and GlobalLandTemperaturesByCountry.csv . https://www.kaggle.com/berkeleyearth/climate-change-earth-surface-temperature-data. 

The data, especially City dataset is quite big and full. 
In all calculations I used decadal average.
1) The data is more or less clean, especially after 1900 year. Both achieves have around 3-4% of missing data. This data I replaced by mean value calculated over the period 1900-2013. The data was averaged from daily values initially.
2) Obviously that data wasn't manually reconstructed before. This  is good, since it gives us opportunity to work more on the quality control of the data and provide and clean data more carefully. 
3) Data cleaning: Nan's have been replaced by the averaged calculated for the period 1900-2013. It was my "straightforward" approach, since there was no time to go deep into this problem.
However, with the extra time, I could find other temperature data archives and provide a comparison analysis between the data. If data has all necessary values it might be considered for being for replacing. 
Data can be: observational, modelling and reconstructional. Thus, we would have a diverse choice where and which data to take. 
4) With the extra time, I would go more away from decadal averaging and do monthly scaling per year or per 11/30 years. During 20th century there've been small and relatively large climate seasons with similar weather conditions. Relatively large (again, I'm talking only on century scale) last around 30 years, small = 11 year. Thus, I would rather think about doing 11 years averaging or 30 years instead of 10 years. According to climatology, there are certain climatological periods like: 1950-1980, 1981-2010. During those periods, a relatively similar climate was observed. 
5) With more time I would do an outlier analysis, this actually can also help to determine the best averaging periods. I would also spend more time on visualisation part, with providing spatial distribution (maps) of temperature.
6) I have splited data into 70/30 ration for obtaining training and testing data. I didn't perform cross-validation set, however It worth to do. 
6) For modelling approach I have taken LSTM since I worked only on 4 cities and it calculated relatively quick, with good performance (according to baseline model). I employed a very simple baseline model based on averaging. 
7) Of course, since the modelling part is the most interesting, I would probably try to grab other meteorological parameters and would create/generate more features. Then I would probably try some regression approaches (log, lasso) and XGBoosting Regressor.
Of course, I would experiment on baseline models as well. 



