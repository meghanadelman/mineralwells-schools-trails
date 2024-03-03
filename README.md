# Mineral Wells Schools and Trails
Map of school locations and hikes in and around Mineral Wells, TX.

## Project Contents

- [Data Source](#data-source)
- [Project Background](#project-background)
- ....

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

If you set the view to the whole state of Texas you will have a lot of data on the screen so to simplify, set your scale to 1:125000 at the greatest and pick an area in Texas that you would like to focus on. For this example, we will be focused on the Mineral Wells area.

![in process image](map-progress-1.png)
*Data viewed throughout the state of Texas*

Format the school points and trail 

### Map summary

What are the key findings to take from your map and the overall mapmaking process?

## Final Project Link

Here you are linking from the README.md to the index.html.

Please view the [final map online](www.github...)
