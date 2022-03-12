# Mapping Earthquakes
Module 13 challenge prepared by Hannah Wikum - March 2022
___
## Resources
Data Source: Earthquake data from USGS (https://earthquake.usgs.gov/earthquakes/feed/v1.0/); Tectonic plate data in GeoJSON form from GitHub repopsitory (https://github.com/fraxen/tectonicplates/blob/master/GeoJSON/PB2002_boundaries.json)

Software: JavaScript, HTML, Mapbox, Leaflet, Visual Studio Code
___
## Overview
This challenge built off the tasks in Module 12 that had us create maps with JavaScript and HTML coding of earthquake data from GeoJSON objects and Mapbox/Leaflet formatting. There were three different components in the challenge:
  
  **1. Add tectonic plate lines**
  The GeoJSON line string coordinates for all tectonic plates was provided in a GitHub repository. I added a new call to the data using d3 and then applied a style to the lines using a pink color and weight of 4 before adding it to the map. This was a useful visual because most earthquakes fall on a fault line between tectonic plates.
  
  **2. Add an additional layer for major earthquakes (>4.5 magnitude)**
  To add a third layer to the exisitng Earthquakes and Tectonic Plates option, I copied most of the code and formatting from the allEarthquakes section, but connected to U.S. Geological Survey data only for earthquakes with 4.5+ magnitude in the last seven days. I edited the color coding to have three categories: less than five was yellow, greater than five orange, and greater than 6 red. This can be turned on or off, just like the other layers.
  
  **3. Add a third basemap option**
  For the final part of the challenge, I added a third map background option. I started with street and satellite views and added a third for outdoors. I used the Mapbox Styles API to copy and edit my code from the street view to update to outdoors and then added the third option to the basemaps object.
  
  
