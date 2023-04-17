# MUMBAI WEATHER ANALYSIS
### Project Overview
Analysis of weather in Mumbai over 3 decades.
* The Original Dataset contained 5 columns.
    1. Time 
    2. Tmin 
    3. Tavg
    4. Tmax 
    5. precp
* Parsed the time column to get day,week,year information.
* Further seperated the data into 3 major seasons over 3 decades 
* Calculated mean temperature for:
     1. Specific Year 
     2. For a specific season of that year 
* Used Linear Regression to capture Trends purely based on serial dependence 
* The main purpose of the project is to look for any changes in mean temperature over the last 3 decades 

### Code and Resources 
* Dataset from kaggle.com
* Packages : Pandas, Numpy, sklearn, statsmodel, datetime, matplotlib, seaborn
* Webscrapper : None 
* Code : Kaggle time series notebook referred (https://www.kaggle.com/learn/time-series) 
 
 ### Data Cleaning 
 * 15 percent overall missing values ,hence imputed with the weekly mean temperature of that month 
 * Day,month,year was exctracted from "Time" column and made into new columns with respective names 
 * From above created 2 Dataframe :\
        1. Mean monthly temperature\
        2. Mean yearly temperature 
 * With the help of monthly dataframe, grouped data according to 3 major seasons 
 
### Exploratory Data Analysis 
* The Dataset contained only two variables :1- Temperature, 2- Precipitation 
* This Project focuses soley on temperature,also,40% of Precipitation data was missing 
![alt text](https://github.com/svrashank/Mumbai_Weather_Analysis/blob/main/Avg_daily_temp_yearly.JPG "Avg temp of last 30 years")
![alt text](https://github.com/svrashank/Mumbai_Weather_Analysis/blob/main/Monsoon.JPG "Avg tmep in monsoon")
![alt text](https://github.com/svrashank/Mumbai_Weather_Analysis/blob/main/Summer.JPG "Avg temp in summer")
![alt text](https://github.com/svrashank/Mumbai_Weather_Analysis/blob/main/WInter.JPG "Avg temp in winter")

### Time Series Analysis 
* Went with time series analysis with regression to capture trends 
* I created 3 dataframes for 3 variables(Tavg,Tmin,Tmax) 
* Rolling average was calculated with window of 5 years 
* Only Tavg showed a linear increasing trend and hence I decided to model linear regression on it 
* Linear Regression was chosen due to its capablity of capturing trends
* Using Deterministic Process training variable (X_avg) and forecast varaiable(X_fore) were created 
![alt text](https://github.com/svrashank/Mumbai_Weather_Analysis/blob/main/Time_series_forecast.JPG "Forecast of Tavg for next 5 years")

### Project Conclusions 

 

        

 
