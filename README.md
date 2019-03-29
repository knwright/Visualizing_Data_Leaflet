# Visualizing Data with Leaflet

## Background
The USGS is interested in building a new set of tools that will allow them visualize their earthquake data. They collect a massive amount of data from all over the world each day, but they lack a meaningful way of displaying it. Their hope is that being able to visualize their data will allow them to better educate the public and other government organizations (and hopefully secure more funding..) on issues facing our planet.

## Visualize the Data

![Earthquake Map with Tectonic Plate Boundaries](images/earthquake_map)

1. **Obtain the data sets**

   ![3-Data](images/3-Data.png)

   The USGS provides earthquake data in a number of different formats, updated every 5 minutes. Visit the [USGS GeoJSON Feed](http://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php) page and pick a data set to visualize. When a data set is selected, a JSON representation of the data is returned. The URL of this JSON is used to pull in the data for the visualization.

   ![4-JSON](images/4-JSON.png)

2. **Import & Visualize the Data**

   A map was created using Leaflet that plots all of the earthquakes from the data set based on their longitude and latitude.

   * The data markers reflect the magnitude of the earthquake in their size and color. Earthquakes with higher magnitudes should appear larger and darker in color.

   * Popups are included that provide additional information about the earthquake when a marker is clicked.

   * The legend provides context for the map data.

A second data set was used to illustrate the relationship between tectonic plates and seismic activity. Data on tectonic plates can be found at <https://github.com/fraxen/tectonicplates>.

This data set adds the following to the map:

* A number of base maps to choose from as well as two different data sets shown as overlays that can be turned on and off independently.

* Layer controls to the map.
