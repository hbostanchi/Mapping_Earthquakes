# Mapping_Earthquakes

## Moduale overview
In this module, you will use the Leaflet.js Application Programming Interface (API) to populate a geographical map with GeoJSON earthquake data from a URL. Each earthquake will be visually represented by a circle and color, where a higher magnitude will have a larger diameter and will be darker in color. In addition, each earthquake will have a popup marker that, when clicked, will show the magnitude of the earthquake and the location of the earthquake.

## Resources
We used the Leaflet library to plot the data on a Mapbox map through an API request and created interactivity for the earthquake data. We added the USGS URL for earthquake data by navigating to the USGS Hazards Program, clicking the Earthquakes link to open the Real-time Data Feeds link and scrolled down to "GeoJSON Summary" Feed. There, we clicked the All Earthquakes link under the “Past 7 Days” heading

Data Source: majorAirports.json, torontoRoutes.json, torontoNeighborhoods.json
Software: JS, D3, Leaflet

## Overview
Create a branch from the master branch on GitHub.
Add, commit, and push data to a GitHub branch.
Merge a branch with the master branch on GitHub.
Retrieve data from a GeoJSON file.
Make API requests to a server to host geographical maps.
Populate geographical maps with GeoJSON data using JavaScript and the Data-Driven Documents (D3) library.
Add multiple map layers to geographical maps using Leaflet control plugins to add user interface controls.
Use JavaScript ES6 functions to add GeoJSON data, features, and interactivity to maps.

## Challenge Summary:
## Background
To illustrate the severity of the earthquakes in relation to the tectonic plates, you’ll need to log in to GitHub and access the tectonic plate data from this GitHub repository. (Links to an external site.) You will also need to make an API call to the tectonic plate data using d3.json(), and then add the data as an overlay to the map using the L.geoJSON() layer. In addition to the streets and satelliteStreets maps, you’ll need to add a third map style of your choosing. All map styles must be added to the base layer so that they show up on the map to allow the user to change which layers are visible.

## Objectives
The goals of this challenge are for you to:

- Use d3.json() to get tectonic plate data and add the data using the L.geoJSON() layer.
- Style the tectonic plate LineString data to stand out on the map.
- Add the tectonic plate data as an overlay with the earthquake data.
- Add a third map style to allow the user to select from three different maps.

## Instructions
To complete this challenge, follow these steps:

Create a new folder on your Mapping_Earthquakes repository and name it “Earthquake_Challenge.”
Copy the folders and files from your Earthquakes_past7days branch and add them to the Earthquake_Challenge folder. The folder should have this structure:
Earthquake_Challenge folder
index.html
static
css
style.css
js
config.js
logic.js
Use the GeoJSON/PB2002_boundaries.json data from the GitHub repository (Links to an external site.) for the tectonic plate data. You’ll need to log into GitHub to access the GeoJSON data.
Place the d3.json() call with the L.geoJSON() layer for the tectonic plate data at the end of your code from your Earthquakes_past7days branch.
Style the lines with a strong, bright color so the lines show up on the satellite map and are not too light to be seen on the lighter maps.
Create the tectonic plate layer for the map.
Add the tectonic plate layer to the overlays so that they show up in the tile layer, as shown in the image below.
Add the tectonic plate and earthquake data to the map for any map style choice.
Edit the base layer so that it holds all three maps.
Make the streets map the default map.


For the challenge, a third map style is added to the [logic.js](https://github.com/hbostanchi/Mapping_Earthquakes/blob/master/hbostanchi_Earthquake_Challenge/static/js/logic.js) file and has the following:

It is added to the baseMaps.
When selected the map style is present on the map.
The earthquake and tectonic data are present on the map style.


![final image](https://github.com/hbostanchi/Mapping_Earthquakes/blob/master/image/Screen%20Shot%202020-01-12%20at%205.16.10%20PM.png)


![final image](https://github.com/hbostanchi/Mapping_Earthquakes/blob/master/image/Screen%20Shot%202020-01-13%20at%202.55.10%20PM.png)

## View [Live Demo Map](https://hbostanchi.github.io/Mapping_Earthquakes/)
## App
The map loads with the street view, earthquake circles and tectonic plates showing. Selecting any circle will display more information about the earthquake. When selecting the upper right menu, you have the option to change the base map to satellite or dark mode. You can also remove the earthquake or tectonic plate layers. Earthquake map in action.

![gif](https://github.com/hbostanchi/Mapping_Earthquakes/blob/master/image/earthquake_demo.gif)
