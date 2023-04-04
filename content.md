layout:true

<div class="header">
  
  <p class="header-text">Introduction to GIS Fundamentals</p>
</div>
<div class="footer">
  <p class="footer-text">
    <img src="images/datapolitan-logo-01.svg" class="logo_new">
    <span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">
      <img alt="Creative-Commons-License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" />
      </p>
</div>

--

class: center,middle

![img-center-50](images/datapolitan-logo-01.svg)

# Introduction to GIS Fundamentals

- - -

## Instructor: Richard Dunks

### Follow along at: 

#### See the code at: 

<p class="license-text"><strong><strong>Introduction to GIS Fundamentals</strong></strong> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://www.datapolitan.com" property="cc:attributionName" rel="cc:attributionURL">Richard Dunks</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a></p>

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img style="border-width:0;width:8%" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a>

---

class:center,middle
# Welcome

---
exclude:true
# [Zoom Drill](https://vimeo.com/407215417)
+ Mute and Unmute your microphone
+ Start and Stop your video
+ Post a message in the Chat window with your name and computer operating system (Windows or MacOS)
+ Click the Participants window and Raise your hand 

???
+ Facilitators will cover the following skills: muting themselves, stopping their video, typing in chat box, raising their hand, sharing their screen



---

# A Few Ground Rules
???
+ Facilitators establish the intention we have for the culture of the classroom

--

+ Step up, step back
--

+ One mic
--

+ Be curious and ask questions in the chat box
--

+ Assume noble regard and positive intent
--

+ Respect multiple perspectives 
--

+ Be present (phone, email, social media, etc.)

---

# Introductions
+ Name
+ Department / Job
+ One thing you hope to get out of class today

---

# Goals for the class 
--

+ Describe the foundational concepts of spatial analysis and mapmaking
--

+ Describe the general structure and purpose of Geographic Information Systems (GIS)
--

+ Describe spatial data formats and sources of spatial data
--

+ Apply concepts of spatial analysis using NYC Open Data to answer an NYC-related problem
--

+ Discuss resources for further information and instruction on QGIS and other spatial analysis tools

---

# Outcomes
--

+ You will be familiar with the foundational concepts in spatial analysis and mapmaking
--

+ You will understand the structure and purpose of GIS
--

+ You will be practiced in applying spatial concepts to real-world problems
--

+ You will be familiar with the differences between open source and proprietary software applications
--

+ You will be familiar with resources for further information on how to use QGIS for spatial analysis and mapmaking

---

# Goals for this morning
--

+ Review basic geospatial principles and GIS tools
--

+ Discuss spatial data formats
--

+ Demonstrate and practice how to load, filter, and select data in QGIS
--

+ Demonstrate and practice how to style spatial data
--

+ Demonstrate and practice how to export data from QGIS


---

class:center,middle
# Why Do We Create Maps?

---

class:center,middle
# Types of Maps

---

# General Reference Maps

--

+ Show important physical features of an area
--

+ Include natural and man-made features
--

+ Usually meant to help aid in the navigation or discovery of locations
--

+ Usually fairly simple
--

+ Can be stylized based on the intended audience (tourists vs locals)

---

class:center,middle
![img-center-90](images/referencemap.png)

##### Source: http://nationalmap.gov/small_scale/printable/reference.html
---

# Thematic Maps

--

+ Focuses on a specific theme or subject area
--

+ Features on the map represent the phenomenon being mapped
--

+ Spatial features used for reference
---

![img-center-90](images/thematic1.png)
##### Source: http://www.usna.usda.gov/Hardzone/ushzmap.html 

---

# Choropleth
![img-center-75](images/choropleth.png)

##### Source: http://www.geogalot.com/myp-humanities/year-9/understanding-hazards/003---choropleth-mapping

---

# Choropleth

![img-center-90](images/floatingsheep-beer-church.jpg)

##### Source: http://www.floatingsheep.org/2012/07/church-or-beer-americans-on-twitter.html

---

# Area Cartogram
![img-center-55](images/Cartogram_US.png)

.caption[Electoral Votes by State]
##### Source: http://training.fws.gov/courses/csp/csp7203/resources/Types_of_Maps_2013.pdf 

---

# Dorling Cartogram
![img-center-90](images/dorling.png)

.caption[Obesity by State]
##### Source: http://homes.cs.washington.edu/~jheer//files/zoo/ 

---

class:center,middle
# Basic Map Elements

---

# Points  
![img-center-50](images/point_feature.png)
#### Source: http://docs.qgis.org/2.8/en/docs/gentle_gis_introduction/vector_data.html#overview

---

# Lines
![img-center-50](images/polyline_feature.png)
#### Source: http://docs.qgis.org/2.8/en/docs/gentle_gis_introduction/vector_data.html#overview

---

# Polygons
![img-center-50](images/polygon_feature.png)
#### Source: http://docs.qgis.org/2.8/en/docs/gentle_gis_introduction/vector_data.html#overview

---

class:center,middle
# How do we make maps?

---

# Geographic Info System (GIS)
> Any system for capturing, storing, checking, and displaying data related to positions on the Earth's surface

+ [National Geographic Education Encyclopedia](http://education.nationalgeographic.org/encyclopedia/geographic-information-system-gis/)

---

# Or more simply

> In a GIS, you connect _**data**_ with _**geography**_.

+ [GISgeography.com](http://gisgeography.com/what-gis-geographic-information-systems/)

---

# Geographic Info Systems (GIS)
--

+ Create interactive queries (user-created searches)
--

+ Analyze spatial information
--

+ Edit data in maps
--

+ Present the results of all these operations

---

# Basic Map Using QGIS
![img-center-70](images/spatial_example.png)

---

#[QGIS](http://www.qgis.org/)

![img-center-95](images/qgis.png)
#### Source: [NYC Open Data 311 Service Requests](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9), DOT Responsible Agency 1 Jan - 30 Jun 2015

---

# QGIS - The Good
--

+ Freely available desktop application
--

+ Lots of features
--

+ Works with different data types
--

+ A strong community developing new features and plug-ins

---

# QGIS - The Bad
--

+ A bit bug-y sometimes
--

+ Visual style is a little clunky
--

+ Features change between versions
--

+ It will crash (but so will ArcGIS)

---

# QGIS - The Bug-y
--

+ Sometimes things get jumbled -> zoom out then zoom back in
--

+ Things don't work properly -> close and restart
--

+ Other problems that we'll find in class

---

<!-- opening shapefile -->
# Let's Get Started
1. [Click this link](data/boros/boros.zip) and download the file to your desktop
2. Unzip the file
3. Open QGIS

![img-left-20](images/qgis_launch.png)

---

# QGIS Getting Started
![img-center-90](images/qgis_nav1.png)

---

# QGIS Getting Started
![img](images/qgis_nav2.png)

---

![img-center-60](images/qgis_nav3.png)

![img-center-60](images/qgis_nav4.png)

---

# QGIS Getting Started
![img-center-90](images/qgis_nav5.png)

---

# Attribute Table 
![img-center-75](images/qgis_nav6.png)
### Right click on layer


---

# Attribute Table
![img](images/qgis_nav7.png)

---

<!-- Styling -->
# Styling Features
+ Right-click the layer and select the Properties option
+ Select "Style," and finally, choose "Categorized":
        
![img-90](images/styling1.png)

---

# Styling Features
+ Select the column that has the data you want to style:
    
![img-center-60](images/styling2.png)

![img](images/styling3_box.png)

---

# Styling Features
![img](images/styling4_box.png)

---

# Styling Features
![img-center-90](images/styling5.png)

---

# Add labels to data
+ From Properties, select "Labels", "Show labels for this layer"

![img-center-90](images/labeling1.png)

---

# Add labels to data
+ Select the column that has the data you want to use for labels

![img](images/labeling2.png)

+ Click "Apply", "Ok"

---

# Add labels to data
![img-center-90](images/labeling3.png)

---

# Styling Labels

![img-center-90](images/label_placement1.png)

---

# Styling Labels
![img-center-80](images/label_placement2.png)

---

# Your turn
--

+ Style the polygons however you'd like
--

+ Change the outline color or add a pattern
--

+ Style the labels
--

+ Change the font, the font size, or other attributes

---

class: center, middle
# 5 Min Break

![img-center-50](images/sadtopographies/disappointment_cove.png)

##### Source: https://www.instagram.com/sadtopographies/

---

# Layers
![img-center-90](images/map1.png)
#### Image Source: http://www.geocontrolling.com/co-je-gis.htm
---

# Shapefiles
--
        
+ Basic file for storing map elements
--

+ Stores spatial data, like points, lines, and polygons
--

+ Multiple files comprise a "shapefile"

--

![img-center-80](images/file_struct1.png)

---

# Shapefiles

![img-center-80](images/file_struct1.png)
--

+ .shp—The main file that stores the feature geometry
--

+ .dbf—The dBASE table that stores the attribute information of features

---

# Shapefiles

![img-center-80](images/file_struct1.png)

+ .prj—The file that stores the coordinate system information
--

+ .shx—The index file that stores the index of the feature geometry

---

# You might also see
--

+ .cpg—Identifies the character set to be used
--

+ .sbn and .sbx—The files that store the spatial index of the features

---

# Shapefiles

+ Have a few limitations
--

+ One geometry type (Point, Line, Polygon) per shapefile
--

+ So sometimes you end up with this:
![img](images/file_struct2.png)

---

# Shapefiles
--

+ Column names can only be letters, numbers, and underscores "_"
--

+ Column names can only be ten characters long

--

![img-center-100](images/shapefile-column-names.png)


---

class:center,middle
# Let's add another layer

---

# 311 DOT Service Requests
+ [Download the data](data/dot-311/20160201_20160207_DOT_311_ServiceRequests.zip) to your desktop
+ Unzip the file
+ Open in QGIS

![img-center-60](images/DOT_311_1.png)
---

# 311 DOT Service Requests

![img-center-90](images/DOT_311_2.png)

---
        
# Layer Ordering
--

+ Layers on top are drawn on top
--

+ Just drag and drop within the Layers Panel to change order
--

+ Try it now
---

# Filter and Query
+ We can filter the points based on the values in the attribute table

---
        
# Filter and Query
+ Right-click on the layer and select "Filter" to open the Query Builder

![img-center-90](images/filtering_data.png)


---

# Filter and Query
![img-center-60](images/filter1.png)

---

# Filter and Query
![img-left-60](images/filter2.png)
--
![img-right-35](images/filter3.png)

---

# Filter and Query
![img-center-60](images/filter4.png)

---

# Filter and Query
![img-center-90](images/filter5.png)

---

class:center,middle
# We can also filter by multiple conditions

---

# Multiple Conditions
![img-left-60](images/filter6_box.png)
--
![img-right-35](images/filter7.png)

---

# Multiple Conditions
![img-center-90](images/filter8.png)

---

# Zoom to Layer
![img-center-60](images/ztl1.png)

---

# Zoom to Layer
![img-center-90](images/ztl2.png)

---

# Zoom Selection
--

+ Select the zoom on the toolbar
--

![img-right-30](images/zoom_box.png)
--

+ Draw a box around the area you want to zoom into
--

+ Click the icon to return to the previous map extent
--

![img-right-30](images/extent_box.png)

---

# Pan Map
+ Select the hand tool to pan around the map

![img-center-30](images/hand.png)

---

# Exporting Data
![img-left-35](images/export1.png)
--
![img-right-50](images/export2_box.png)

---

# Your Turn
--

+ Filter for service requests in your borough
--

+ Try and find something interesting
--

+ Change the style of the point, either to a different shape, color, or icon
--

+ Export your selection as a new shapefile

---

class:center
# 10 Min Break
![img-center-50](images/sadtopographies/unfortunate_cove.png)

#### Source: https://www.instagram.com/sadtopographies/
---

# Let's add another layer
+ [Right click this link](data/Parking_Facilities.csv)
+ Select "Save link as" 
+ Save the file (`Parking_Facilities.csv`) to your desktop

---

# What is a CSV file?
--

![img](images/csv1.png)

---

# What is a CSV file?
![img-center-90](images/csv2.png)

---

# Adding CSV Data
![img](images/add_csv1.png)

---

![img-center-60](images/add_csv2_box.png)

--

![img-center-55](images/add_csv3.png)

---

# Adding CSV Data
![img](images/add_csv4_box.png)

---

# Adding CSV Data
![img](images/add_csv5.png)

---

class:center,middle
# So what is a Coordinate Reference System?

---

# Projections
--

+ No one's favorite part of GIS
--

+ But a necessary part of it nonetheless
--

+ Convert points on the 3-dimensional Earth (**latitude** and **longitude**) to x and y coordinates on a 2-dimensional map

--

![img-center-65](images/projections-orange.jpg)

#### [Digital Coast Geozone](https://geozoneblog.wordpress.com/2012/05/22/happy-birthday-mercator/)

---

# Projections
+ Every projection distorts some part of your map

![img-center-50](images/projections-faces.png)

[FlowingData](http://flowingdata.com/2014/01/13/map-projections-illustrated-with-a-face/)

---

# Mercator Projections
--

+ A common map projection
--

+ Makes geometries near poles look bigger than geometries near the equator
--

![img-center-50](images/mercator.gif)

---

# Projections Matter
--

+ These circles are all the same size on the globe:

![img-center-50](images/projections-tissot-mercator.png)

[Progonos](http://www.progonos.com/furuti/MapProj/Normal/CartProp/Distort/distort.html)

---

# Projections Matter
+ As are these:

![img-center-60](images/projections-tissot-mollweide.png)

[Progonos](http://www.progonos.com/furuti/MapProj/Normal/CartProp/Distort/distort.html)

---

# Projections Matter
+ And these:

![img-center-50](images/projections-tissot-oblique-mercator.png)

[Progonos](http://www.progonos.com/furuti/MapProj/Normal/CartProp/Distort/distort.html)

---

# Projections Matter
![img-center-90](images/projections.png)

---

# Projections

+ For the most part we will work in **WGS 84** (latitude and longitude)
--

+ In NYC, we use a more accurate projection **NY State Plane/Long Island Zone**
![img-right-60](images/projections_NYSplane.png)

###### Source: https://alidade.wikispaces.com/New+York+SPCS+Zones
---

# Projections
+ Identified by unique IDs that make it easier to talk about them
--

+ WGS 84 is referred to as **EPSG:4326**
--

+ State Plane Long Island is referred to as **EPSG:2263**
--


## Remember these two & you should be set

---

class:center,middle
# Back to Adding CSV Data

---

# Adding CSV Data
![img-center-55](images/add_csv6_box.png)

---

# Adding CSV Data
![img-center-70](images/add_csv7.png)

---

# Saving CSV Data as a Shapefile
![img-left-35](images/save_csv_asSHP1.png)
--
![img-right-60](images/save_csv_asSHP2.png)

---

# Select Points
![img-center-70](images/select1.png)

---

# Select Points
![img-center-40](images/select2.png)

--
+ Click the point
![img-center-40](images/select3.png)

---

# Select Points
![img-center-70](images/select5_box.png)

---

# Select Points - Attribute Table
![img-center-70](images/select6_box.png)

---

# Select Points - Attribute Table
![img-left-30](images/select7.png)

--

![img-right-65](images/select8.png)

---

# Saving Selection
![img-center-70](images/select9_box.png)

---

# Saving Selection

+ If we wanted to reproject the data into a different CRS, we could do that here
--
![img-center-60](images/reproject1.png)
--

+ Pick the new projection in the CRS field (like when we imported the CSV)

---

# What We've Covered
--

+ What is GIS
--

+ Basic GIS concepts and tools
--

+ Adding, styling, and labeling data in QGIS
--

+ Projections
--

+ Selecting features
--

+ Exporting data

---
class:center,middle
# LUNCH
![img-center-50](images/sadtopographies/agony_island.png)

#### Source: https://www.instagram.com/sadtopographies/

---

class: center,middle
# Welcome Back!
## <a href="https://youtu.be/vVX-PrBRtTY" target="_blank">Video to Kick Us Off</a>

---

class: center,middle
# Tell us:
## One thing you learned this morning that you found useful, interesting, and/or helpful

---

class:center,middle
# What do you think of QGIS so far?

---
        
# Goals for the Afternoon
--

+ Add reference data to our maps
--

+ Learn how to join features in QGIS
--

+ Create printable maps in QGIS
--

+ Share resources for further learning

---

class:center,middle
# What have our maps been lacking?

---

# Base Maps
![img-center-90](images/map1.png)
#### Image Source: http://www.geocontrolling.com/co-je-gis.htm
---

# Base Maps
![img-center-80](images/basemap1.png)

---

# Base Maps
--
       
+ Adding base maps will give your map context
--

+ In QGIS, you need a plugin to use base maps
--

+ There are several, but we're only going to use one of them

---

# Base Map Plugin
+ From the Plugins menu, select "Manage and Install Plugins"

![img-center-60](images/basemap2.png)

---

# Base Map Plugin

+ Search for the QuickMapServices plugin and install it

![img-center-70](images/basemap3_box.png)

---

# QuickMapServices Plugin
+ Go to the Settings Menu
![img-center-80](images/basemap4.png)

---

# QuickMapServices Plugin
+ Get the contributed packs
![img-center-80](images/basemap5_box.png)

---

# QuickMapServices Plugin
+ Revel in all the beautiful base maps
![img-right-30](images/basemap6.png)

---

# Choosing a Base Map
--

+ Think about what someone reading your map needs to see for context
--

+ Think about how the base map interacts with the data on your map

---

# Base Maps - Hierarchy
--

+ If your data is the most important part of the map, make sure it looks more important than the base map
--

+ Avoid base maps that strongly emphasize features that aren't relevant on your map

---

# Base Maps - Colors
--

+ Choose base maps with colors that complement the colors on your map
--

+ The contrast between the color on your map and the color on the base map should be enough to make your layers clearly visible

---

# Base Maps - Scale

![img-center-55](images/scale.jpg)

#### Source: http://go.owu.edu/~jbkrygie/krygier_html/geog_222/geog_222_lo/geog_222_lo04.html

---

# Base Maps - Scale
+ Base maps show different levels of detail at different scales
--

+ Make sure the level of detail is appropriate to your map

---

# Scale

![img-center-80](images/scale-basemap.png)

---

# Scale

![img-center-80](images/scale-basemap-denver.png)

---

# Your Turn
+ Find a good base map for your data
+ Think about hierarchy, color, and scale
+ Don't be afraid to play around

---

class:center,middle
# 5 Min Break
![img-center-50](images/sadtopographies/cape_disappointment_lighthouse.png)
#### Source: https://www.instagram.com/sadtopographies/

---

# Basic Spatial Joins

![img-right-30](images/join1.png)

--

## Point to Polygon
+ Relate points inside a polygon to that polygon (ex. count the number of points)

--

## Polygon to Point 
+ Points can take on value of enclosing polygon

---

# Question
## What are some of the spatial joins we could do with this data?
![img-center-50](images/add_csv7.png)

---
class:center,middle
# Let's do one together

---

# Parking facilities by borough
![img-center-60](images/join2.png)

---

# Parking facilities by borough
![img-center-50](images/join3.png)

---

# Parking facilities by borough
![img-center-50](images/join4.png)

--

![img-center-50](images/join5.png)

--

![img-center-85](images/join6.png)

---

# Reproject the boroughs 
## We'll use EPSG:4326
![img-center-70](images/join7.png)

---

# Reproject the boroughs 
## We'll use EPSG:4326
![img-center-45](images/join8_box.png)

---

# Parking facilities by borough
![img-left-45](images/join9.png)

--

![img-right-45](images/join10.png)

---

# Parking facilities by borough
![img-center-90](images/join11.png)

---

# Parking facilities by borough
![img-center-90](images/join12.png)

---

# Your Turn
+ Count the number of DOT 311 service requests in each [community district](data/nycd_16a/nycd_16a.zip) in your borough
+ Style the community districts by the number of service requests

---

class:center,middle
# 10 Min Break
![img-center-50](images/sadtopographies/grumpy_lane.jpg)

#### Source: <a href="https://www.instagram.com/p/Bo_W2MHB_Zp/" target="_blank">sadtopographies on Instagram</a>

---

# Print Composer
--

+ How you make exportable and printable maps in QGIS
--

+ Able to add map elements (legends, scales, text, etc)
--

![img-center-70](images/print_comp1.png)

---

# Create a new print composer

![img-left-50](images/print_comp2.png)
--
![img-right-40](images/print_comp3.png)

---

# print composer
## You are greeted with a blank slate

![img-center-90](images/print_comp4.png)

---

# print composer
## Add New Map adds to your current map
![img-left-20](images/print_comp5_box.png)
--
![img-right-65](images/print_comp6.png)

---

# print composer
## Customize item properties on the right

![img-center-45](images/print_comp7.png)

---

# Print Composer
## Don't forget a title and your sources

![img-left-15](images/print_comp8_box.png)
![img-right-80](images/print_comp9.png)

---

# Print Composer
## Export options

![img-center-50](images/print_comp10.png)

---

# Print Composer
## You can share your map or print it
![img-center-80](images/print_comp11.png)

---

# Print Composer 
## Problems you might encounter
--

+ Map extent -> "Use current map extent"
--

+ Moving map around -> Adjust with arrows
--

+ "North" arrow -> need to manually align

---

class:center,middle
# [Click to submit your work](https://script.google.com/a/macros/datapolitan.com/s/AKfycbwMcE5pcJwZHdbSCN_2epwaXnRLSRPaLbHCAhxaZJ79UXaRpQ_l/exec)


---

class:center,middle
# Presentations

---

class:center,middle
# Take a moment to email your map to yourself

---

# Review of This Afternoon
--

+ Adding base maps to QGIS
--

+ Installing plug-ins
--

+ Joining data
--

+ Creating a printable map in print composer

---

# Some Other GIS Tools

![img-center-90](images/gis.png)

---

# [ArcGIS](http://www.esri.com/software/arcgis/arcgis-for-desktop)

![img-center-large](images/arcgis.jpg)
[Source](http://www.esri.com/news/arcuser/1012/a-workflow-for-creating-and-sharing-maps.html)

---

# [Adobe Illustrator](http://www.adobe.com/products/illustrator.html)/ [Mapublisher](http://www.avenza.com/mapublisher)
![img-center-90](images/illustrator.jpg)
[Source](http://www.avenza.com/resources/blog/2011/06/28/how-get-open-street-map-data-adobe-illustrator-mapublisher)

---

# [Google Earth](https://www.google.com/earth/)

![img-center-80](images/google_earth.png)

---
exclude:true
# [Google Fusion Tables](https://sites.google.com/site/fusiontablestalks/stories)
<iframe width="100%" height="430" scrolling="no" frameborder="no" src="https://www.google.com/fusiontables/embedviz?q=select+col54%2C+col55+from+1dNtdy7FuBBZ2qTxX7jgZ5Dig8n96oxRrWFjuhYpJ+where+col3+%3E%3D+0+and+col3+%3C%3D+4+and+col26+%3D+2+limit+1000&amp;viz=HEATMAP&amp;h=true&amp;lat=40.844685&amp;lng=-73.915349&amp;t=1&amp;z=12&amp;l=col54&amp;y=2&amp;tmplt=2&amp;hmd=true&amp;hmg=%2366ff0000%2C%2393ff00ff%2C%23c1ff00ff%2C%23eeff00ff%2C%23f4e300ff%2C%23f4e300ff%2C%23f9c600ff%2C%23ffaa00ff%2C%23ff7100ff%2C%23ff3900ff%2C%23ff0000ff&amp;hmo=0.6&amp;hmr=26&amp;hmw=0&amp;hml=TWO_COL_LAT_LNG"></iframe>
Source: [NYC Open Data 311 Noise Complaints, 1 Jan - 20 May 2014, Between Midnight and 4 am in the Bronx](https://www.google.com/fusiontables/DataSource?docid=1dNtdy7FuBBZ2qTxX7jgZ5Dig8n96oxRrWFjuhYpJ# map:id=3)

---

# Proprietary vs Open Source
--

+ Proprietary software source code is owned by an individual or an organization and tightly restricted (usually for profit)
--

+ Open source software source code is freely available to anyone for download, alteration, and republishing

---

# Proprietary vs Open Source

--

+ Proprietary software code is generally supported by a team of paid professionals working for the organization that owns the code
--

+ Open source software code is generally supported by a mix of paid and volunteer professionals that contribute changes back to the community
---

# Proprietary vs Open Source
--

+ Proprietary software is often available only by purchasing a license
--

+ Open source software is free to use though there generally a license that specifies the restrictions (if any) on its use and reuse
--

+ Companies using open source software may charge for the use of the software through their proprietary implementations or via their infrastructure

---
exclude:true
class:center,middle
# Examples of Open Source Mapping Software


---
exclude:true

# [CartoDB](https://cartodb.com/)
<iframe width="100%" height="480" frameborder="0" src="https://richard-datapolitan.cartodb.com/viz/c0d4f39e-962e-11e4-9b3b-0e9d821ea90d/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>


---

# Some Things We Didn't Cover
--

+ Normalizing data for choropleths ([see this video](https://www.youtube.com/watch?v=t1RvSxNcafU))
--

+ Buffering features
--

+ Geocoding
--

+ Spatial databases
--

+ Other spatial data types (KML, GeoJSON, GeoTIFF)
--

+ Editing data

---

# QGIS - The Good
--

+ Open-source software that’s freely available
--

+ Works with lots of different data types, including shapefiles, KML (Google Earth), GeoJSON, and text files
--

+ Works with various spatial databases
--

+ Strong community developing features and plug-ins
---

# QGIS - The Bad
--

+ Not an enterprise software like ESRI ArcGIS
--

+ The visual style is a little clunky
--

+ Features tend to change between versions (moving around, menu option changes, etc) 
--

+ Major versions tend to have major feature changes
--

+ Plug-ins tend not to work with newer versions
--

+ And it crashes (as you've probably already experienced)

---

# And of course...
![img-center-80](images/bug.png)

---

# QGIS - The Bug-y
--

+ Projects with different CRS layers tend to get misaligned when zooming
--

+ _Zoom in and then back out to fix_
--

+ Google base maps tend not to appear on load
--

+ _Have to zoom in to get them to appear_
--

+ Other odd behavior that they’re hopefully working on
--

+ _File them here: https://hub.qgis.org/wiki/17/Bugreports_

---

class:center,middle
# Good Resources for Further Information

---

# GIS Stack Exchange

![img-center-90](images/gis-stackexchange.png)

[GIS Stack Exchange](http://gis.stackexchange.com/)

---

# Learning QGIS

![img-center-40](images/learning-qgis.png)

[Learning QGIS](https://www.packtpub.com/application-development/learning-qgis-20)

---

# QGIS Map Design

![img-center-40](images/qgis-map-design.png)

[QGIS Map Design](http://locatepress.com/qmd)

---

# Other Documentation
+ [QGIS online manual Gentle GIS Introduction](http://docs.qgis.org/2.8/en/docs/gentle_gis_introduction)
+ [QGIS Tutorials and Tips](http://www.qgistutorials.com/en/index.html)
+ [Free and Open Source GIS Ramblings](https://anitagraser.com/)

---

class:middle
![img-center-70](images/google.png)

---

# Reminders
--

+ Know your layer CRS
--

+ When in doubt, zoom in and then zoom out
--

+ If you’re working with a CSV file and run into an error, export as a shapefile and try it again
--

+ Save your project often
--

+ Choose good file names

---

# Final Thoughts
--

+ Maps are a great way to visualize and explore spatial data
--

+ Some data is only intelligible when mapped
--

+ QGIS is a cheap (as in free) way to get started 
--

+ There are many resources online for how to use QGIS and other GIS applications
--

+ Share what you know with others -> Data wants to be mapped

---
class:center,middle
# Thank You

---

# Contact Information
+ [Email me](mailto:richard[at]datapolitan[dot]com)
+ Check out [my website](https://wwww.datapolitan.com)
+ Connect on [Twitter](https://twitter.com/Datapolitan)
+ Connect on [LinkedIn](https://www.linkedin.com/in/richarddunks/)
+ Follow us on [Instagram](https://www.instagram.com/datapolitan/)
