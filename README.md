
# Citi-Bike-Analytics

![alt text](https://d21xlh2maitm24.cloudfront.net/nyc/Annual-Membership-Image.png?mtime=20170331121650)

<p align="center">
  <a href="#data-source">Data Source</a> •
  <a href="#findings">Findings</a> •
  <a href="#technology-Used">Technology Used</a>
</p>

A analysis for the New York Citi Bike Program, in which responsible for overseeing the largest bike sharing program for 200,000+ data points in the United States
 in order to generate business insights in terms of visulize the peak time in both summer and winter period and the top start location in New York City and Jersey City, New Jersey
 
* Click [here](https://public.tableau.com/profile/davidgu#!/vizhome/citibikeanalysis/Forcityofficials?publish=yes) to view complted dashboard

![alt text](images/ridership:membership-growth.png)

![alt text](https://raw.githubusercontent.com/david880110/Citi-Bike-Analytics/master/image/avg_bike_distance.png)

![alt text](https://raw.githubusercontent.com/david880110/Citi-Bike-Analytics/master/image/popularity_over_time.png)

## Data Source
![alt text](https://raw.githubusercontent.com/david880110/Citi-Bike-Analytics/master/image/citibikedata.png)

This [Citi Bike Data](https://www.citibikenyc.com/system-data) has been processed to remove trips that are taken by staff as they service and inspect the system and any trips that were below 60 seconds in length 
(potentially false starts or users trying to re-dock a bike to ensure it's secure).

<table class="hide-while-loading table table-striped">
<tbody id="tbody-content">
<thead>
<tr>
<th>Name</th>
<th>Date Modified</th>
<th>Size</th>
<th>Type</th>
</tr>
</thead>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201701-citibike-tripdata.csv.zip">JC-201801-citibike-tripdata.csv.zip</a></td>
<td>Apr 6th 2017, 02:01:43 pm</td>
<td>255 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201702-citibike-tripdata.csv.zip">JC-201802-citibike-tripdata.csv.zip</a></td>
<td>Apr 6th 2017, 02:01:44 pm</td>
<td>275 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201703-citibike-tripdata.csv.zip">JC-201703-citibike-tripdata.csv.zip</a></td>
<td>Apr 6th 2017, 02:01:44 pm</td>
<td>241 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201704-citibike-tripdata.csv.zip">JC-201804-citibike-tripdata.csv.zip</a></td>
<td>Aug 1st 2017, 09:20:54 am</td>
<td>432 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201705-citibike-tripdata.csv.zip">JC-201805-citibike-tripdata.csv.zip</a></td>
<td>Aug 1st 2017, 09:20:55 am</td>
<td>529 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201706-citibike-tripdata.csv.zip">JC-201806-citibike-tripdata.csv.zip</a></td>
<td>Aug 1st 2017, 09:20:56 am</td>
<td>647 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201707-citibike-tripdata.csv.zip">JC-201807-citibike-tripdata.csv.zip</a></td>
<td>Aug 1st 2017, 09:20:57 am</td>
<td>676 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201708%20citibike-tripdata.csv.zip">JC-201808 citibike-tripdata.csv.zip</a></td>
<td>Oct 3rd 2017, 08:52:49 am</td>
<td>711 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201709-citibike-tripdata.csv.zip">JC-201809-citibike-tripdata.csv.zip</a></td>
<td>Oct 3rd 2017, 08:52:49 am</td>
<td>667 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201710-citibike-tripdata.csv.zip">JC-201810-citibike-tripdata.csv.zip</a></td>
<td>Jan 31st 2018, 01:15:18 pm</td>
<td>703 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201711-citibike-tripdata.csv.zip">JC-201811-citibike-tripdata.csv.zip</a></td>
<td>Jan 31st 2018, 01:15:19 pm</td>
<td>477 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201712-citibike-tripdata.csv.zip">JC-201812-citibike-tripdata.csv.zip</a></td>
<td>Jan 31st 2018, 01:15:19 pm</td>
<td>324 KB</td>
<td>ZIP file</td>
</tr>
</tbody>
</table>

* Limitation
There were 7% user did not provide gender information and most of them (14%) are weekend users so we will not be able to tell if female are more willing to ride
on the weekend then they do on weekdays, but we may still determine that male user are the dominant customer at all time

![alt text](https://raw.githubusercontent.com/david880110/Citi-Bike-Analytics/master/image/limitation.png)


## Findings 


### (1) The current major citi bike riders fall into young male group between 18 -20 but number of femal reiders increases over time as they are showing interest to start riding during the weekend

![alt text](https://raw.githubusercontent.com/david880110/Citi-Bike-Analytics/master/image/customer_base.png) ![alt text](https://raw.githubusercontent.com/david880110/Citi-Bike-Analytics/master/image/femal_ridership.png)

### (2) The 1st and 2nd peak hours during a day would usually be 7-8 AM and 5-6 PM season-regardless 

![alt text](https://raw.githubusercontent.com/david880110/Citi-Bike-Analytics/master/image/peakhours.png)

### (3) As the temperature gets cold as winter begins, people tend not to ride as well because of the lack of comfort individuals face when riding in low temperatures. Therefore, at some point the ridership does not grow. However, the total amount of annual member have been kept increased over time in 2017

![alt text](https://raw.githubusercontent.com/david880110/Citi-Bike-Analytics/master/image/2017_growth.png)

## Map visualization for city officials

* More and more people choose to live in Jersey City and work in Manhathan

![alt text](https://raw.githubusercontent.com/david880110/Citi-Bike-Analytics/master/image/popular_location.png)

## Technology Used

<img src="https://raw.githubusercontent.com/david880110/tech-logo/master/python%20logo.png" width="240" height="50"/>

<img src="https://raw.githubusercontent.com/david880110/tech-logo/master/tableau%20logo.png" width="240" height="60"/>

