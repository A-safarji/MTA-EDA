# Exploratory Data Analysis (EDA) Projects of MTA Turnstile Data:

## Abstract 

The goal of this project would be an identification of the subway stations that have the most congestions and crowds, correlated with those who commute every day. And to help decreasing crowds from busy stations. For these, I will also include stations and external sources that can support reducing crowds in busy stations between morning and evening time. As a result, the crowds will be shown and detected on map based on congestion time.   

## Design 

The project utilizes a dataset provided by the MTA that helps in getting information regarding the stations especially the turnstiles information. MTA APIs for maps and line logos. Therefore, the design detect congestions based on stations exits, entries between moring and evening. After detecting, the model will generate live map for spoting congestions, to enable MTA take action to improve operations and support busy stations.  

## Data 

The dataset contains over 2.5 million observations in the period from July to September of 2021 with 11 columns. A few feature highlights include numbers of entries/exits for each station. In addtion, using MTA maps dataset for individual features for each station by using  latitude/longitude coordinates and it contians 496 rows × 14 columns.   

## Algorithms 

Exploratory data analysis techniques are used to clean the data and form a proper dataset that can be reasonably aggregated and visualized. 

*Feature Engineering*

1. Upload both datasets to the Jupyter Notebook.
2. Convert the daily report of MTA to monthly.
3. Cleaning the data, dropping duplicates and imputing any missing value.
4. Resting illogical entries and exits of MTA dataset.
5. Finding the sum of entries and exitst were taken for each station, considering the uniqueness of each of the “C/A, UNIT, and SCP” for each station.
6. Discovering the congestions station by calculating the sum of all the entries/exits for each day of the period between JUL to Sep in each station.
7. Grouping and splitting stations based on moring and evening time for the 3 months.
8. Sorting the morning and the evening based on stations congestions time and take the top 20 stations.
9. Visual the result from both morning and the evening congestions.
10. Finding the coordination of congestions from the map dataset and mapping the result on live map of morning and the evening.


## Tools 
* To carry out the project and explore the data, Jupyter,Sqllite3 and Python3. In addition, Python3 libraries which are: Matplotlib, Seaborn, and Plotly-express for data visualization. Numpy, and Panda for data read and write operations.
* Using Folium and plotly dash for maps visualization.  

## Scope
* Due to the computational and time constraint as well as the unavailability of complete datasets. The MTA Turnstile and MTA maps  will be used.

## Communication 

In addition to the slides and visuals presented, [EDA of MTA Turnstile](https://github.com/A-safarji/MTA-EDA/blob/main/Presentation%26Dashbored.md) will be embedded on my personal dashbored. 


<img width="1036" alt="Screen Shot 2021-10-06 at 10 24 18 PM" src="https://user-images.githubusercontent.com/20365333/136509126-17496e7e-cde0-4d84-8c38-06cc0575409c.png">



<img width="1039" alt="Screen Shot 2021-10-06 at 10 23 59 PM" src="https://user-images.githubusercontent.com/20365333/136509130-01e7619a-b014-4a2f-ae39-9c6d4ec90f4b.png">


<img width="975" alt="Screen Shot 2021-10-08 at 9 28 14 AM" src="https://user-images.githubusercontent.com/20365333/136508825-9a668129-4a85-4f07-a22b-843d4ce4c27a.png">


<img width="984" alt="Screen Shot 2021-10-06 at 8 40 39 PM" src="https://user-images.githubusercontent.com/20365333/136508918-120b3062-efa2-48a2-86b3-557f5561ce69.png">






