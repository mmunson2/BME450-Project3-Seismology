# BME450-Project3-Seismology
#### Matthew Munson
#### 2/26/2020
#### Professor Shima Abadi

# Introduction:

Many of the Pacific Northwest's stunning features are a result of its vast and complex geology. Situated along the Ring of Fire, shifting tectonic plate boundaries off the Pacific Coast are responsible for the region's distinct terrain. Immediately off the Washington Coast sits the Juan De Fuca Plate, one of the smallest tectonic plates on earth. It's wedged between the Pacific Plate and the North American plate and contains nearly all plate boundary types, including divergent, convergent, and transform boundaries. This makes the Jaun De Fuca Plate a prime location for geologic study.

This assignment tasked students with mapping earthquake data on the Jaun De Fuca plate. Data was retrieved from the United States Geological Survey in a ten year period from 2010 to 2020. The plotted earthquake data illustrates the outline of many of the plate boundaries off the Pacific Coast.


# How I Did It:

I began the assignment by retrieving the relevant data from the USGS earthquake catalog. I limited my earthquake data to between the latitudes of 38.891 and 52.107 and the longitudes of -122.168 and -131.836. This encompassed the entirety of the Juan De Fuca plate while keeping the processing requirements minimal. I downloaded this data in a .csv format which can be easily processed in Python.

Once the data was read into my Python file, I performed some minor processing to prepare it for plotting. Time values are converted into datetime and converted from UTC to Pacific time. This process is actually dependent on the time zone of the machine running the code, so time values will vary slightly depending on where this program is executed.

To fulfill the first assignment requirement, I plotted earthquake magnitude versus time over a ten year period. To make the graph more readable and visually appealing I made the scatter plot entries larger for greater magnitudes and applied a color gradient to further illustrate the data trend.

To create the main earthquake map I retrieved a map image from OpenStreetMap and created a bounding box the same size as my earthquake data's outermost lat/long positions. I plotted each earthquake based on its latitude and longitude and once again made the scatter points larger based on their magnitude. Creating the map for April 2015 was simple as I only needed to reduce the number of data points to a one month period. 


# Results:


## Earthquake Magnitude vs. Time:

![alt text](https://github.com/mmunson2/BME450-Project3-Seismology/blob/master/Results/EarthquakeMagnitudeVsTime.png "Magnitude_vs_time") 




## Earthquake Locations and Magnitude:

Earthquake Locations           |  Tectonic Plates
:-------------------------:|:-------------------------:
![](https://github.com/mmunson2/BME450-Project3-Seismology/blob/master/Results/EarthquakeMap.png "Earthquake Locations") | <img src="https://github.com/mmunson2/BME450-Project3-Seismology/blob/master/Results/TectonicPlates.png" width="432" height="582">


## Earthquake Locations and Magnitude in April 2015:


Earthquake Locations           |  Tectonic Plates
:-------------------------:|:-------------------------:
![](https://github.com/mmunson2/BME450-Project3-Seismology/blob/master/Results/EarthquakeMap2015.png "Earthquake Locations") | <img src="https://github.com/mmunson2/BME450-Project3-Seismology/blob/master/Results/TectonicPlates.png" width="432" height="582">


# Analysis:

#### Across what geographic area are you able to observe earthquake data in this map? Why do you see most of the earthquakes in that area?   

The largest clusters of earthquakes are along the tectonic plate boundaries to the north and south of the Juan De Fuca plate. These locations actually contain even smaller tectonic plates, the Explorer Plate and South Gorda Plate, which broke off of the Juan De Fuca Plate millions of years ago. In the south, the Blanco Fracture Zone, Gorda Ridge, and Mendocino Fracture Zone have hundreds of earthquakes of various magnitudes. To the north, Explorer Ridge and the Sovanco Fracture Zone have a cluster of earthquakes with a greater magnitude than other regions. 

The large amount of earthquakes along the Blanco Fracture Zone are likely due to the transform boundary. As the Juan De Fuca Plate moves east towards the Cascadia Subduction Zone, it slides along a portion of the Pacific Plate which protrudes inwards towards the coast. The earthquakes along the Mendocino Fracture Zone are likely due to a similar transform boundary. In this case it's the Gorda Plate making contact with the Pacific plate.

The larger earthquakes on the northern end of the Juan De Fuca Plate are likely due to the transform boundary between the Pacific Plate and the North American Plate. This trend, while outside of the scope of my data, is visible north and south of the Juan De Fuca Plate.

The scatter of earthquakes inland of the Juan De Fuca plate are likely a result of the covergence boundary at the Cascadia Subduction zone. This is where the Juan De Fuca Plate slides under the North American Plate. These boundaries are known to create up to 80% of all earthquakes, and are also responsible for the numerous volcanos in the Pacific Northwest.


#### What is the range of earthquake size (magnitude) in these data? What is the average earthquake size in this area?  

The magnitude of earthquakes between 2010 and 2020 ranged between 2.5 and 6.8. The average magnitude was 3.24, indicating that the vast majority of earthquakes were small.

#### In the month of April 2015, where are the earthquakes mostly located? What event can you link these earthquakes to?  

During this time period there was a cluster of earthquakes along the divergence boundary between the Pacific Plate and the Juan De Fuca Plate. This boundary is divided into the Cobb, Coaxial, and Cleft Segement, and the earthquakes appear to be primarily located on the Coaxial Segment.

These earthquakes can be attributed to the eruption of the Axial Seamount Volcano on April 23rd 2015. The volcano is active and last erupted in 2011 and 1998.

## Part II:




