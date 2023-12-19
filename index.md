---
---
# Nuclear Power Plants in the U.S <br>
**Command Line GIS**<br>
**Masouma Tajik**<br>

<p>Nuclear_Power_Plants.csv contains power plants built accross the world in different countries. The dataset was retrieved from Global Power Plant Database. It has 17 columns and 803 rows. It has a list of power plants with different construction dates from 1968 to 2023.  For this project, we are only interested in the power plants locatd in the United States. therefore, the dataset is filtered accordingly so that it only displays power plants in the U.S.</p> 
<br>
<iframe src="Distribution_map.html" width="1000" height="700"></iframe>
<br>
<p>It appears that most power plants are locaed in the east cost compared to Midwest and west coast. Fortunately, our data subset does not have missing values. The dataset has 17 columns, but the important variables for this study are Power plant names, Capacity of the power plant, and their status (whether they are operational or shutdown).</p> 
<br>
<iframe src="map_number_of_nuclear_plants.png" width="1080" height="640"></iframe>
<br>
In the map above, we spatial joined nuclear dataset with the shapefile and plotted the number of nuclear plants across states in the United States.
<br>
<iframe src="map_with_nuclear_points.png" width="800" height="1000"></iframe>
<br>  
