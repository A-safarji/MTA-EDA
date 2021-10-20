<!-- ### Assumptions:
As a daily subway commuter, based on experience, commuters are more willing to talk to a surveyor while waiting for train than when exiting a station. So, the focus of this analysis was limited to entries into stations (commuters exiting stations were excluded) who are waiting
### Problem Statement:
*Identify how to improve traffics and delays on crowded stations that waste commuters time.
-->



<p align="center">
  <img width="523" src="https://user-images.githubusercontent.com/20365333/135308375-7014d076-2012-44d8-ac93-4cea66f4026e.png">
</p>

###  ![#ed7d2d](https://via.placeholder.com/15/ed7d2d/000000?text=+) Project Proposal EDA For MTA Project(1)

### Introduction:

* New York Metropolitan Transportation Authority (MTA) commute plagued by delays as riders gripe over crowds
and delays on lines led to dangerously-crowded trains.  

#### Question/need:
* The goal of this analysis is to determine congestions and crowds of trains stations that casuses riders gripe over crowds. Therefore, helping decision-making process for MTA and paving the way to provide more buses on thses crowded stations which to decentralize crowds without any addtional costs. 

* Identify busy trains of crowded stations.
* Find congestions between morning and evening.
* How to reduce congestions and delays on crowded stations that waste time.

### Objective and Goal:

Optimize the stations that led to dangerously-crowded trains and crowds.

* Find the congestion and detected it on a live map.
* Discover demand of trains across all stations and further optimize the availability of trains to busy stations.
* Help identify how to reduce congestion and delays on crowded stations that waste commuters' time.
* Provide fetching external transportations near congestion stations and track lines on map to help shift track managment. 

 <!--time period of day with highest traffic and crowds per station * Observe the best time for buses to support if trains out of capacity..-->

   
#### Data Description:
* MTA Turnstile Data:
Data obtained from [MTA Turnstile](http://web.mta.info/developers/turnstile.html).
- [MTA.info](http://www.mta.info/nyct), for maps and line logos

* Field Description:

| Field Name | Description                                                                     |
|------------|---------------------------------------------------------------------------------|
| C/A        | Control Area (A002)                                                             |
| UNIT       | Remote Unit for a station (R051)                                                |
| SCP        | Subunit Channel Position represents an specific address for a device (02-00-00) |
| STATION    | Represents the station name the device is located at                            |
| LINENAME   | Represents all train lines that can be boarded at this station                  |
| DIVISION   | Represents the Line originally the station belonged to BMT, IRT, or IND         |
| DATE       | Represents the date (MM-DD-YY)                                                  |
| TIME       | Represents the time (hh:mm:ss) for a scheduled audit event                      |
| DESC       | Represent the "REGULAR" scheduled audit event (Normally occurs every 4 hours)   |
| ENTRIES    | The comulative entry register value for a device                                |
| EXITS      | The cumulative exit register value for a device                                 |
| Traffic    | The total traffic ENTRIES.diff() + EXITS.diff().                                |
| Congestion | Which is the number of entries and exists added up to know how busy the station |



#### Tools:
* To carry out the project and explore the data, Jupyter,Sqllite3 and Python3. In addition, Python3 libraries which are:
Matplotlib, and Seaborn for data visualization.
Numpy, and Panda for data read and write operations.


#### MVP Goal:

* The goal of this project would be an identification of the subway stations that have the most congestion and crowds, correlated with those who commute every day. And to find how decreasing crowds from busy stations. For these, I will also include stations and external sources that can support reducing crowds in busy stations between morning and evening. 

Dynamic maps to detect and predict crowds on maps. Also, helping reduce crowds by using external transportations and track shifting where they can be spotted on the maps.


[Further details on the MVP of this project](https://github.com/A-safarji/MTA-EDA/blob/main/MVP.md) - feel free to click me!

## Status
Project is: ![#00FF00](https://via.placeholder.com/15/00FF00/000000?text=+) _Done_

