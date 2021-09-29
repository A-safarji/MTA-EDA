<!-- ### Assumptions:
As a daily subway commuter, based on experience, commuters are more willing to talk to a surveyor while waiting for train than when exiting a station. So, the focus of this analysis was limited to entries into stations (commuters exiting stations were excluded) who are waiting
### Problem Statement:
*Identify how to improve traffics and delays on crowded stations that waste commuters time.
-->

<img width="523" alt="Screen Shot 2021-09-29 at 6 09 26 AM" src="https://user-images.githubusercontent.com/20365333/135302457-f11fd9c7-22c1-4cc6-b6dc-ee73d4e48e39.png">

###  ![#1589F0](https://via.placeholder.com/15/1589F0/000000?text=+) Project Proposal EDA For MTA Project

### Introduction:

* New York Metropolitan Transportation Authority (MTA) commute plagued by delays as riders gripe over crowds
and delays on lines led to dangerously-crowded trains.  

#### Question/need:
* The goal of this analysis is to determine traffics and delays of trains station that casuses riders gripe over crowds. Therefore, helping decision-making process for MTA and paving the way to provide more buses on thses crowded stations which to decentralize crowds without any addtional costs. 

* Identify how to improve traffics and delays on crowded stations that waste commuters time.

* Identify un-busy trains and buses to support crowded stations.

### Objective and Goal:

Optimize the stations that led to dangerously-crowded trains and crowds.
* Find the busiest and quitest stations.
* Find demand of passengers across all stations and further optimize the avaliablity of trains to busy stations.
* Discover the impact of rush hour on trains and passenger experience. <!--time period of day with highest traffic and crowds per station * Observe the best time for buses to support if trains out of capacity..-->

   
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

* A MVP would be an identification of the subway stations that have the most traffics and crowds, correlated with those whose commute everyday and decressing crowds from busy stations. For these, I will also include the best top 3 stations and trains that can support reducing crowds in busy stations.

## Status
Project is: ![##f01515](https://via.placeholder.com/15/f01515/000000?text=+) _Under Approval_

