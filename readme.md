## 911 Calls Data Science - Python Project

This project aims to analyse 911 call data sourced from Kaggle. The dataset includes various fields such as latitude, longitude, description, postcode, title, timestamp, township, address, and a dummy variable.

### The data contains the following fields:

* lat : String variable, Latitude
* lng: String variable, Longitude
* desc: String variable, Description of the Emergency Call
* zip: String variable, Zipcode
* title: String variable, Title
* timeStamp: String variable, YYYY-MM-DD HH:MM:SS
* twp: String variable, Township
* addr: String variable, Address
* e: String variable, Dummy variable (always 1)

### Summary of Findings:

#### Basic Data Exploration:
- Top 5 postcodes and townships for 911 calls.
- Number of unique title codes in the dataset.

#### Feature Engineering:
- Creation of a new column "Reason" derived from the "title" column, categorising calls into EMS, Fire, and Traffic.
- Identification of the most common reason for 911 calls, which is visualised using a count plot.

#### Time-based Analysis:
- Conversion of the "timeStamp" column from strings to DateTime objects.
- Extraction of hour, month, and day of the week from timestamps.
- Visualisation of 911 call counts by day of the week and month with a breakdown by reason.

#### Monthly Call Trends:
- Grouping data by month to fill in missing months and plotting call counts per month.
- Using seaborn’s lmplot to fit a linear model on the number of calls per month.

#### Date-based Call Analysis:
- Creation of a "Date" column from the timestamp.
- Plotting daily 911 call counts and separate plots for each reason (EMS, Fire, Traffic).

#### Heatmaps and Clustermaps:
- Restructuring data to create heatmaps where columns represent hours and index represents the day of the week.
- Creation of clustermaps for better visualisation of call patterns.

#### Further Exploration:
- Encouragement to continue exploring the data with additional plots and analyses.

The project effectively demonstrates data preprocessing, feature engineering, and various visualisation techniques to analyse and interpret 911 call data. The findings highlight patterns in emergency call occurrences and provide insights into temporal trends and categorical distributions of call reasons.
