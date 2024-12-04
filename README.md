Introduction:

This project focuses on analysing data of 5000 youtube channels. This analysis was conducted using Python programming using packages including pandas, matplotplib, seaborn and numpy.

Dataset:

The dataset is a csv file containing information about 5000 youtube channels with the attributes; channel name, rank, grade, video uploads, video views and subscribers.
loading the dataset, pandas library was employed using pd.read_csv function. 

Dataframe:

Following successful upload of the dataset, a new pandas dataframe is created to facilitate easy exploration with the pandas library fucntions. Using the shape method, the shape of the dataset is checked to know the total number of rows and columns 

Data Information:

The info method which provides details about the total number of rows, total number of columns, data types of each column, and memory requirements. This step is crucial for understanding the structure of the dataset and identifying any potential data type issues.

Data description:

The describe method is used to check overall statistics of the dataset,providing summary of numerical columns. Some of the statistics include count, min, max, std and unique. The display format of the values in the video views column is formatted using pd.options.display_format to enhance readabilty 

Data Cleaning:

Data cleaning steps included replacing '--' values with NaN. Considering the '--' are strings, an error in the dataset indicated there might be leading or trailing spaces in some of the '--' values, therefore to ensure accuracy the str.strip method was applied to each column to remove all trailing spaces from the '--' values before replacing with NaN using the replace method.
The isnull method is employed to check the number of null values in the dataset which are subsequently dropped using the dropna method.

The 'Rank' column is cleaned by removing unwanted characters and converting it to integers. Similar cleaning steps are applied to 'Video Uploads' and 'Subscribers' columns, ensuring numeric consistency and handling missing or non-numeric values appropriately.

Exploratory Data Analysis: 

EDA involved analyzing key metrics such as average views, top channels by video uploads, and creating a correlation matrix to understand relationships between numeric features. Visualizations using seaborn and matplotlib aided in presenting insights about grades, video uploads, average views, subscribers, and video views.


```python

```
