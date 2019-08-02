
# Citi-Bike-Analytics

![alt text](https://d21xlh2maitm24.cloudfront.net/nyc/Annual-Membership-Image.png?mtime=20170331121650)

<p align="center">
  <a href="#data-source">Data Source</a> •
  <a href="#findings">Findings</a> •
  <a href="#technology-Used">Technology Used</a>
</p>

Analysis of the New York Citi Bike Program, which oversees the largest bike sharing program in the United States.
Python and Tableau are utilized to create visualizations to identify trends and report back to city officials.
 
* Click [here](https://public.tableau.com/profile/sam.wimberly#!/vizhome/citibike-analysis_15645924526980/Maps) to view complted dashboard


## Utilization

![alt text](images/ridership:membership-growth.png)

There were 17,593,918 rides taken on Citi Bikes in New York City in 2018. Riders are much more likely to take a Citi Bike during the warmer, summer months than they are during the colder, winter months, as is displayed in the dashboard above. Short-term customer passes (3-day or 24 hour) follow the same overall seasonal trend, but annaul membership continues to trend in a positive direction regardless of season.


## Peak Hours

![alt text](images/peak-hours-by-season.png)

Upon closer investigation, we find that peak hours follow the same trend regardless of season. Citi Bike usage peaks at 8am and then again at 6pm, suggesting that Citi Bikes are utilized by day-time employees. Citi Bikes are utilized more often during summer and fall when outdoor temperatures are most comfortable. It is somewhat surprsing that city bike use during the spring is not as popular as summer or fall. This could be due to cool temperatures carrying into the spring. 


## Station Popularity

![alt text](images/maps.png)

![alt text](images/top-bottom-stations.png)

Looking exclusively at Jersey City data, we see that the most popular stations are located near metro stations (go to dashboard for interactive map). Four out of the five most popular Citi Bike start and end Stations are located at popular subway entrances. Citi Bike's seem integrally tied to public transportation access. In general, people that use Citi Bike's also seem to utilize other forms of public transportation. What can Citi Bike and New York City do to leverage this knowledge and improve the city's overall infrastructure?


## Utilizations by Gender and Age

![alt text](images/age-gender.png)

Overall, Males utilize Citi Bike's much more often than females or gender unknown. However, over the last year the percentage of female riders has grown from 18.47% to 21.79%, indicating that gender outreach could have had some influence. With more time, a detailed investigation of days of the week and gender ridership might provide further insight into the discrepancy between male and female riders. Does the percentage of female riders spike on the weekend? If so, what would cause this? Does fashion/comfort play a role? Above visualizations imply that Citi Bike users are commuting and not biking for pleasure or exercise (as idicated by the most popular start and end stations). Why does it seem like women are not using Citi Bikes as part of their commute?


## Bike Condition

![alt text](images/bike-maintenance.png)

The above visulization shows total trip length and average trip length for each Citi Bike. Over the last year, we can identify which bikes were used the most and which bikes were used the least. This may help identify which bikes will need maintenance soon, but without a history of each bike's maintenance schedule, we can't know if some of these bike's have already been repaired.

## Data Source

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
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201801-citibike-tripdata.csv.zip">JC-201801-citibike-tripdata.csv.zip</a></td>
<td>Sep 6th 2018, 02:44:38 pm</td>
<td>328 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201802-citibike-tripdata.csv.zip">JC-201802-citibike-tripdata.csv.zip</a></td>
<td>Sep 6th 2018, 02:44:38 pm</td>
<td>389 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201803-citibike-tripdata.csv.zip">JC-201703-citibike-tripdata.csv.zip</a></td>
<td>Sep 6th 2018, 02:44:39 pm</td>
<td>443 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201804-citibike-tripdata.csv.zip">JC-201804-citibike-tripdata.csv.zip</a></td>
<td>Sep 6th 2018, 02:44:39 pm</td>
<td>614 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201805-citibike-tripdata.csv.zip">JC-201805-citibike-tripdata.csv.zip</a></td>
<td>Sep 6th 2018, 02:44:40 pm</td>
<td>888 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201806-citibike-tripdata.csv.zip">JC-201806-citibike-tripdata.csv.zip</a></td>
<td>Sep 6th 2018, 02:44:40 pm</td>
<td>1.08 MB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201807-citibike-tripdata.csv.zip">JC-201807-citibike-tripdata.csv.zip</a></td>
<td>Sep 6th 2018, 02:44:41 pm</td>
<td>1.11 MB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201808%20citibike-tripdata.csv.zip">JC-201808 citibike-tripdata.csv.zip</a></td>
<td>Sep 12th 2018, 02:58:07 pm</td>
<td>1.17 MB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201809-citibike-tripdata.csv.zip">JC-201809-citibike-tripdata.csv.zip</a></td>
<td>Oct 3rd 2018, 02:48:13 pm</td>
<td>1.03 MB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201810-citibike-tripdata.csv.zip">JC-201810-citibike-tripdata.csv.zip</a></td>
<td>Nov 7th 2018, 02:44:39 pm</td>
<td>1.03 MB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201811-citibike-tripdata.csv.zip">JC-201811-citibike-tripdata.csv.zip</a></td>
<td>Dec 4th 2018, 11:27:38 am</td>
<td>640 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/JC-201812-citibike-tripdata.csv.zip">JC-201812-citibike-tripdata.csv.zip</a></td>
<td>Jan 8th 2019, 03:51:15 pm</td>
<td>521 KB</td>
<td>ZIP file</td>
</tr>
</tbody>
</table>


## Technology Used

<img src="https://images//python-logo.png" width="240" height="50"/>

<img src="https://images/tableau-logo.png" width="240" height="60"/>

