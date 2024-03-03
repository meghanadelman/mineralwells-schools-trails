# Mineral Wells Schools and Trails
Map of school locations and hikes in and around Mineral Wells, TX.

## Project Contents

- [Data Source](#data-source)
- [Project Background](#project-background)
- [Purpose](#purpose)
- [Mapmaking Process](#mapmaking-process)


***

### Data Source

[Link to school data](https://schoolsdata2-tea-texas.opendata.arcgis.com)
[Link to trail data](https://tpwd.texas.gov/state-parks/park-information/maps/use-the-trails-maps-anytime-anywhere)


### Project Background

<p>This project was designed with Texas data on school locations and Texas State Park trails. To reduce the scope of the project, it was limited to Mineral Wells. The choice to limit to Mineral Wells was mostly because my family used to visit Mineral Wells State Park multiple times a year to go hiking and camping.

### Purpose

<p>The purpose of this project was to map the locations of all schools and hiking trails in and surrounding Mineral Wells to find the distances between schools and hiking trails. 

### Mapmaking Process

To start the map first go to the data sites to download your data. 
To download the Texas State Park trail data simply click on the kmz file link and download to your computer.
To dowload the school data, click on the 'current schools' option. If you want to explore mapping any other options, feel free to do so.

 ![in process image](School-data-1.png)
 *Click on current schools option*

Once you have clicked on the correct tab you will see this selection:
![in process image](School-data-2.png)
*Click on the GeoJSON file download*

Once you have both these files downloaded, open the QGIS Software. 
Start a new project in QGIS and under *XYZ Tiles* select the *ESRI Standard* map format. Then import the Trail data kmz file and the School data GeoJSON file.

If you set the view to the whole state of Texas you will have a lot of data on the screen so to simplify, set your scale to 1:250000 at the greatest and pick an area in Texas that you would like to focus on. For this example, we will be focused on the Mineral Wells area.

![in process image](map-progress-1.png)
*Data viewed throughout the state of Texas*

Once you have selected your area of focus, format the school points and trail. You can do this by right clicking on the layer and selecting *properties*. 
For the trails layer, I would suggest editing the line properties. Go to *symbology* and select *single symbol*. Choose a color that represents trails and select the stroke style *dash line*.

![in process image](map-progress-2.png)

For the school points, leave the symbology as it is and select a color that you feel represents schools.
Once you have the symbology of your layers finalized, it is time to add names!
Find the properties window for the Texas Trails layer and click on *labels*. Click on *single labels* and set the value as *Name*. Then select the font type, size, and color. To help the trail names stand out, you can add a drop shadow. 
Some of the trail names may not be visible with the 1:250000 scale. This is okay based on the purpose of our static map, however if you would like to create a zoomable map you can set them to show up based on scale under the *rendering* tab.
Follow the same steps with the School layers. You should get something that looks like this:

![in process image](map-progress-3.png)

Now, we need to find out how far away the schools are from the nearest trail. 
To do this, select the Texas trails layer. Then, find the *shortest line between features* option under the *Vector Analysis* tab in the Processing Toolbox. 
Select the source layer as the schools and the destination layer as your trails. This is how the paramters should look before you hit Run.

![in process image](map-progress-4.png)







### Map summary

What are the key findings to take from your map and the overall mapmaking process?

## Final Project Link

Here you are linking from the README.md to the index.html.

Please view the [final map online](www.github...)
