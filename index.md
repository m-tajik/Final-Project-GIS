---
---
# Nuclear Power Plants in the U.S <br>
**Command Line GIS**<br>
**Masouma Tajik**<br>

<p>Nuclear_Power_Plants.csv contains power plants built accross the world in different countries. The dataset was retrieved from Global Power Plant Database and it was in CSV format. It has 17 columns and 803 rows. It has a list of power plants with different construction dates from 1968 to 2023.  For this project, we are only interested in the power plants locatd in the United States. therefore, the dataset is filtered accordingly so that it only displays power plants in the U.S.</p> 
<br>
<iframe src="Distribution_map.html" width="1000" height="700"></iframe>
<br>
<p>It appears that most power plants are locaed in the east cost compared to Midwest and west coast. Fortunately, our data subset does not have missing values. The dataset has 17 columns, but the important variables for this study are Power plant names, Capacity of the power plant, and their status (whether they are operational or shutdown). The dataset did not have missing values, and included coordinates to help us map it. There were no issues regading the quality of the dataset, but the geometry cokumn was empty, and I retreived that from the coordinates of Lattitude and Longtitude.</p> 
<br>
<iframe src="map_number_of_nuclear_plants.png" width="1070" height="900"></iframe>
<br>
<p>In the map above, we spatial joined nuclear dataset with the shapefile and plotted the number of nuclear plants across states in the United States. Seem like Pennsylvania, Illinois, South Carolina and California have the highest numbers of nuclear plants compared to other states.</p> 
<br>
<iframe src="map_with_nuclear_points.png" width="800" height="1000"></iframe>
<br>  
<p>We decided to check how many and which nuclear plants are located in New Jersey. We had to clip coast lines so that they do not caue data misrepresentstion in the map. The map above presents the population density of NJ from census data. However, we are interested in areas thts are more populated compard to other areas. Therefore, we calculated the CVs of population, and picked those below 40 (4% when normalized). The reason we are doing that is that the less the CVs, the more polulation living in the aread since the dispersion aorund the median population is less. It means, areas are equally and normally populated. The hatched areas represent the most populated areas, which is another layer of population data with CVs less than 40. Moreover, the red points represent nuclear plants in NJ. It appreas tht 3 nuclear plants each Salem_1, Salem_2, and Hope Creek_1 are located on coast lines where it is less populated, versus Oyster Creek nuclear plant which is close to populated areas. This map is the result of spatial joining of multiple layers of census data, and nuclear plants dataset.  </p>
<br>
<iframe src="map_with_layers.html" width="1120" height="700"></iframe>
<br>
This interactive map shows has multiple toggles to show the features of the dataset. First, it has layers that toggle nuclear plants that are either "Operational" or "Non_operational". Second, It can also display the reactor type in each nuclear plant. Lastly, it also displays capacity level of nuclear plants. The median value for capacity of nuclear plants is 800, and the variable "Capacity" is left skewed. Meaning that values lower than the median value are too far scattered and dispersed, and very smaller than 800. Thus, all values below 800 are considered low capacity. 
