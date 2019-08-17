# Creating a Basic Map in ArcMap

*This tutorial will cover some basics of the ArcMap user interface, using map symbology, and creating a map layout. In this tutorial we use the following data (right click on each link and select "open link in a new tab" to download the files), although any other GIS datasets will also work:*
* [PLUTO](https://www1.nyc.gov/assets/planning/download/zip/data-maps/open-data/nyc_mappluto_18v2_1_shp.zip)
* [Parks Properties](https://data.cityofnewyork.us/api/geospatial/rjaj-zgq7?method=export&format=Shapefile)
* [Hydrography](https://data.cityofnewyork.us/api/geospatial/drh3-e2fd?method=export&format=Shapefile)

Once you've downloaded each of the three folders, you will have to extract the files from each folder (these folders are zipped because of their size). Extract **ALL** the files (from the three zipped folders) to the same folder (you could create a new folder for this exercise called "Arc_Lab_1", etc.). Make sure all the files go into that same folder. Each of the three zipped folders contains 6-8 files, and these files need to stay together!! 

![t1-1.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_01/t1_1.PNG)

Open ArcMap. Go to `Start` > `Programs` > `ArcGIS` > `ArcMap`. A dialogue box should appear, as below. To start a new map project, select `Blank Map` and click `OK`.

![t1-2.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_01/t1_2.PNG)

To connect ArcMap to your working directory, click on the `Catalog` tab (all the way to the right of the data frame), when you click on it, the catalog dialog box will expand. Click the pushpin/thumbtack icon (it’s small) in the right corner of the catalog dialog box
(by the X).

![t1-2-1.png](https://github.com/alisaalias/gis_tutorials/blob/50374381d33d00ceb24a3403c195723b7a7666e0/Images/Tutorial_01/t1-2-1.PNG)

Click on the icon with a folder and a plus sign. `Folder connections` should appear in the menu. Click the plus sign (+) next to `folder connections`. Select the folder where your files are located on your computer, i.e. the file path.

You should see several shapefile icons for the files of the PLUTO map, parks, and water. Drag and drop each shapefile into the white space in the data frame. You should see list of the shapefiles show up in the Table of Contents dialog box on the left
hand side of the interface (with the box checked). If any boxes are unchecked, check the boxes next to each layer.

Alternatively, to Add Data to the map project, you can also click on the `Add Data` button on the toolbar, shown below. A dialogue will appear, allowing you to navigate to the data files you want to add as layers of your map.

![t1_3.png](https://github.com/alisaalias/gis_tutorials/blob/50374381d33d00ceb24a3403c195723b7a7666e0/Images/Tutorial_01/t1_3.png)

To see the data associated with each shapefile, right click on the layer name and choose `Open Attribute Table.` For the PLUTO layer, you will see there is a spreadsheet/table with many rows and columns. 

![t1-2_2.png](https://github.com/alisaalias/gis_tutorials/blob/50374381d33d00ceb24a3403c195723b7a7666e0/Images/Tutorial_01/t1-2_2.png)

Each row represents a polygon of one building footprint. The columns contain geographic information about each building, but also additional information. For example, the column "NumFloors" represents the number of floors in that building. 

![t-2_3.png](https://github.com/alisaalias/gis_tutorials/blob/50374381d33d00ceb24a3403c195723b7a7666e0/Images/Tutorial_01/t1-2_3.png)

Close the attribute table.

![t1-3.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_01/t1_3.PNG)

Once you have added data/layers, you can zoom and pan using the buttons on the toolbar. Select tools allow you to make selections from the data features. The `identify` tool allows you to query individual features for their attribute data.

![t1-4_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_01/t1-4_new.png)

You can arrange the ordering of the layers by stacking the data layer names in the `Display` tab of the `Table of Contents` on the left of the screen. The ordering of the layers in the `Table of Contents` will correspond to their ordering in the map. Below is an example. The open space (parks) layer is displayed above the building (PLUTO) layer, which is in turn displayed above the water layer.

![t1-5_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_01/t1-5_new.png)

Drag the building layer above the open space layer.

To change the symbology of your layers, right-click on the layer name and choose `Properties`. A dialogue will appear. Under the `Symbology` tab, you will find the options for coloring or visualizing your data.

Option A: To keep all features a single color, choose `Features` > `Single Symbol` on the left. You can change the color by clicking on the swatch. For example, make sure the Parks layer is symbolized as green and the water layer is symbolized as blue.

![t1-6.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_01/t1_6.PNG)

Option B: To visualize your data based on a qualitative category, choose `Categories` on the left and specify (by clicking) the type of categorization. In the image below `Unique Values` is chosen. In the `Value Field` drop down menu, select the field by which you'd like to visualize your data. In the image below, the borough field was chosen. Click `Add All Values` to display the category values. You can change the color of your symbols by either using the Color Ramp drop-drop down menu or double-clicking on the swatches to the left of the `Values` list.

![t1-7_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_01/t1-7_new.png)

Option C: To visualize your data based on numeric quantities, select `Quantities` on the left and specify (by clicking) the type of visualization. In the image below, `Graduated Colors` is chosen. In the `Value` drop-down menu, select the field by which you'd like to visualize your data. If appropriate, you can normalize your data by another quantity field by selecting it from the `Normalization` drop-down. You can change the color of your symbols by either using the Color Ramp drop-down menu or by double-clicking on the swatches on the left of the `Range` list. In the image below, the `NumFloors` value is chosen. You might get an error that the max sample size has been reached. The fix for this error is described in the following section.

![t1-8_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_01/t1-8_new.png)

To change the number of displayed value ranges, you can select the number of classes from the `Classes` drop-down menu. By default, 5 classes are displayed and delineated using Jenks Natural Breaks algorithm. If you want to change this default, you can click on the `Classify…` button. A dialogue appears as below.

![t1-9_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_01/t1-9_new.png)

To fix the sampling size error, click on the `Sampling...` button. In the `Data Sampling` pop up box, type 1000000 (one million) into the box next to `Maximum Sampling Size` and click `OK`.

![t1-9_1_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_01/t1-9_1_new.png)

You can change the number of classes by using the `Classes` drop-down menu. You can change the method of classification by using the `Method` drop-down. Your options include manually classifying your data, equal interval, and standard deviation classification as well as some others. The histogram displays the distribution of your data, with blue vertical lines showing the breaks between classes. To manually classify the dataset, you can either move the blue break lines (by clicking and dragging them) or typing in the Break Values in the list to the right of the dialogue. On the upper right corner of the dialogue box, basic statistics corresponding to the data is displayed that can be useful in deciding how to visualize your data.

In all cases, clicking `OK` will save and display your new symbology.

## Laying Out and Exporting Your Map:

To create a map layout, switch your view from `Data View` to `Layout View` by clicking on the icon of a page in the lower left corner of the map window as below.

![t1-10.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_01/t1_10.PNG)

The map window should now show you your map's data frame on a sheet of paper. You can adjust the size and location of the data frame by adjusting its bounding box.

A new set of tools to zoom and pan appears when you are in the `Layout View`. The `Data View` zoom and pan tools are still active and will affect the map within the data frame. To zoom and pan on the page without affecting the map, use the (page) `Zoom` and `Pan` toolbar. Zoom in so that Morningside Heights shows in the layout view. 

**Note** about zooming/panning: in general, but also specifically in this case, when you are visualizing a lot of data (e.g. the PLUTO shapefile containing all buildings in NYC), it may take ArcMap some time to redraw the map each time you zoom or pan or move the map. Many times, ArcMap will time out and will not finish redrawing the map. If you move/pan/zoom the map too much, ArcMap is likely to crash.

![t1-11.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_01/t1_11.PNG)

You can add standard elements to your map through the `Insert` menu shown below. The `Legend`, `North Arrow`, `Scale Bar`, and `Scale Text` options each lead to dialogues that allow you to customize those map elements. To edit the layer titles for the legend, click on the layer value `NumFloors`, then click again (not a double click, a click... then a click i.e. how you would change the name of a file on your computer). Once you can edit the layer name, type in "Number of Floors". In the legend dialogue box, you can also select a border or background for your legend, or edit other stylistic elements.

![t1-12.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_01/t1_12.png)

To edit the font and size of the title, click to add `Title` from the `Insert` menu, then type in the title (in this case, the title of the map could be "Morningside Heights buildings and parks"). Then once you've added the title, double click on the title text box to open the properties dialogue box for editing the title. Click on `Change Symbol...` to edit the font and size of the title text.

![t1-13.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_01/t1_13.PNG)

You can change the position the elements you inserted into the page area.

![t1-14.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_01/t1_14.PNG)

When you are finished with your map, you can export it to a variety of formats. Go to `File` > `Export Map…` to reach a dialogue box where you can choose your export format and save your map. You will find that you can export your map as an image file (i.e. JPG) for immediate use or as a vector-based file (i.e. EPS) for further graphics editing.
