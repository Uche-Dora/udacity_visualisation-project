# udacity_visualisation-project
## Dataset

The bike sharing system also known as public bicycle scheme is a shared transport service that makes bicycle's accessible for short term use by individuals at low to no cost. The dataset contains information on the bicycle stations, bicycle, users information and trip duration. 

The dataset was read into a dataframe using ```pd.read_csv('201902-fordgobike-tripdata.csv')``` 
At the data wrangling stage, I checked for the number of rows and columns, presence of null and duplicated values, datatype of each colum present in the datatype using ```bike_sharing.head(5)```, ```bike_sharing.shape```, ```bike_sharing.isnull().sum()```, ```bike_sharing.duplicated().sum()```, ```bike_sharing.dtypes```. Some tidiness issues and quality issues were detected from the dataset which was treated. Null values were dropped, wrong datatypes were corrected and date and time column was sepearted into different columns. To aid more insight, new columns were created from the start_time and duration_sec columns.

## Summary of Findings

 The univariate exploration was used to see the distribution of the variables of interest in the dataset. Relationship between the variables were also established using both bivariate and multivariate visualization. It was found that most trips were taken on tuesdays and thursday by 8am and 5pm. More bike users are males and most are subscribers. Most users were between the age 20 - 40 years.

 Most users between age 50 - 60 were Males. Across all genders however, users between 30 to 40 years had more count. Regular customers have more difffude use across duration_min compared to subscribers that was concentrated between 0 - 20mins.


## Key Insights for Presentation

1. Males use bikes more at sanfrancisco.
2. Most bike users are between age 30 to 50
3. Subscribed users most likely used bikes for their day to day activity just within the area. 

**NOTE:** age above 90 and duration_min above 60 were traeted as outliers and dropped from the dataset. 
