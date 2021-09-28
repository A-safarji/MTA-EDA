<!-- ### Assumptions:
As a daily subway commuter, based on experience, commuters are more willing to talk to a surveyor while waiting for train than when exiting a station. So, the focus of this analysis was limited to entries into stations (commuters exiting stations were excluded) who are waiting
### Problem Statement:
*Identify how to improve traffics and delays on crowded stations that waste commuters time.
-->


###  ![#1589F0](https://via.placeholder.com/15/1589F0/000000?text=+) Project Proposal EDA

### Introduction. 

* New York Metropolitan Transportation Authority (MTA) commute plagued by delays as riders gripe over crowds
and delays on lines led to dangerously-crowded trains.  

#### Question/need:
* The goal of this analysis is to determine traffics and delays of trains station that casuses riders gripe over crowds. Therefore, helping decision-making process for MTA and paving the way to provide more buses on thses crowded stations which to decentralize crowds without any addtional costs. 

* Identify how to improve traffics and delays on crowded stations that waste commuters time.

* Identify un-busy trains and buses to support crowds.

### Objective and Goal:

Optimize the stations that led to dangerously-crowded trains and crowds.
* Finding the overall busiest stations and quitest.
* Finding none traffic trains to support other stations.
* Finding time period of day with highest traffic and crowds per station.
* Finding the best time for buses to support if trains out of capacity.

#### Data Description:
* MTA Turnstile Data:
Data obtained from http://web.mta.info/developers/turnstile.html.

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



#### Tools:
* Python3, Pandas, Numpy, Jupiter, Seaborn, Sqlite3 and Matplotlib.


#### MVP Goal:
* What would a [minimum viable product (MVP)](./mvp.md) look like for this project?
* What would a minimum viable product (MVP) look like for this project? A MVP for this project would be a list of ten subway stations with the best (....)
