# Downloading and Displaying Data from American FactFinder

## Using FactFinder to Download Census Data

Census data can be downloaded from the [American FactFinder](http://factfinder.census.gov/), [Social Explorer](https://www.socialexplorer.com/), or [NYC Population FactFinder](https://popfactfinder.planning.nyc.gov/#12.25/40.724/-73.9868). This tutorial uses American FactFinder to find and extract Census data.

There are many ways to narrow down your search on the American FactFinder website. You can use `Community Facts` for popular tables for a city of interest. `Guided Search` filters by type of data, topics, geographies, and demographics. We will use the `Advanced Search` in this tutorial as it provides the most options for filtering your results.

![t11-0.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-0.png)

Click on `Advanced Search` and `Show Me All`.

![t11-1.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-1.png)

On the next page, the sidebar on the left includes options to search for data. These include `Topics` (age, income, year, dataset), `Geographies` (states, countries, places), Race and Ethnic Groups (race, ancestry, tribe), Industry Codes (NAICS industry), and `EEO Occupation Codes` (executives, analysts).

It is advised to use `Geographies` as an initial search because not all data is available at all scales of geography.

Click on `Geographies`. This will open a new dialog box titled `Select Geographies`.

![t11-2.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-2.png)

You can browse the tabs at the top of the dialog box to browse by List, Name, Address, or Map. We will use the List tab. Make sure the `Select from` option is checked to `most requested geographic types`. For this tutorial we will select `Census Tract` from the `Select a geographic type` dropdown menu. We will select New York from the `Select a state` dropdown menu. Select `All Census Tracts within New York`. Next click `Add To Your Selections` at the bottom of the dialog box.

![t11-3.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-3.png)

The geography will now be applied to your search and added to the `Your Selections` box on the top left side of the page. You can then close the `Select Geographies` dialog box.

The data available for the selected geography will be displayed as a list under `Search Results`. You can narrow your search from your selected geographies using the `Topics` tab on the left side of the page.

Click `Topics` at the left opening the `Select Topics` dialog box.

![t11-4.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-4.png)

Once the dialog box opens, you can expand the topics to browse available datasets. For this tutorial we will expand the `Housing` topic, browse within `Financial Characteristic`, and select `Gross Rent`. Once you click on the topic it will be added to `Your Selections`. Then you may close the dialog box and return to the `Search Results`.

![t11-5.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-5.png)

The list will now be updated to include the filters for both your selected `Geographies` and `Topics`.

![t11-6.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-6.png)

To preview the content of each Table, File, or Document Title, you can click on the `About` icon on the right side of the list, with the `i` for information icon. An example of the data included will be previewed in a new window.

![t11-7.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-7.png)

Once you find the dataset you wish to download, click on the dataset of interest. In this tutorial we will select `Gross Rent` also called table `B25063`. This opens a new window with a detailed preview of the dataset. Here you can download the data using the `Download` button on the `Actions` panel. Click on the `Download` button opening the `Download` dialog box.

![t11-8.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-8.png)

In the `Download` dialog box choose the `Data and annotations in a single file` option and check the box `Include descriptive data element names` if you wish to include a description of each variable in the dataset.

If you select multiple datasets, you will have to download each dataset individually.

The dataset will be downloaded as a packaged zip file. You can now open your downloaded .csv files in Microsoft Excel (make sure to extract/unzip the folder into your working directory).

## Downloading TIGER shapefiles

Navigate to the [TIGER Download Webpage](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html) on the US Census site.

![t11-13_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-13_new.png)

Navigate to the tabs at the bottom and choose the appropriate year (2017) for your download. Then click `Web Interface` in the `Download` box.

![t11-14_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-14_new.png)

On the next page, choose the year of interest and the layer type. From the `Select year` dropdown menu we will choose `2017` and from the `Select a Layer Type` dropdown we will choose `Census Tracts`.

![t11-15_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-15_new.png)

On the next page choose the geography of your interest. From the `Select a State` dropdown menu we will choose `New York` and click `Download`. Your download will now begin. You may need to disable pop-up blockers for the download to start.

*Note: If you download these files in Google Chrome or some web browsers, you may need to disable security preferences indicated by a security shield to the right of the address bar.*

TIGER shapefiles can also be downloaded directly from the American Factfinder without having to navigate to a new webpage. In the preview page of your selected data, choose `Create Map`.Click `Create Map`. Click on any piece of hyperlinked data in the table to create the map, in this case the first entry for the `Gross Rent Estimate` column. 

![t11-15_1.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-15_1.png)

Once the map is created you can preview the map and legend. To download the associated TIGER shapefile, click “Download” from the “Actions” panel.

![t11-9_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-9_new.png)

In the `Download` dialog box, select the option for “Shapefiles (.zip)” at the bottom of the window under `Spatial Data formats.` Click `OK` and `Download` in the next window. You may have to turn off pop-up blockers to download the data. If the file does not contain projection data, it is recommended to download the TIGER shapefiles directly from the TIGER website.

![t11-10_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-10_new.png)

*Note: If you download these files in Google Chrome or some web browsers, you may need to disable security preferences indicated by a security shield to the right of the address bar.*

## Preparing FactFinder Data for Importing and Joining into ArcMap

Unzip the .zip file of the dataset you downloaded for Gross Rent. Open the `.csv` file in Microsoft Excel.

Choose the `ACS17_5YR_B25063_metadata.csv`. We can use this file to see how our field names are defined.

![t11-11.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-11.png)

Choose the `ACS17_5YR_B25063_with_ann.csv`. We will need to modify this table so that it can properly join with the shapefile in ArcMap.

![t11-12_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-12_new.png)

Once the file is open, ensure the following:

  * Use only one header row. Rename these headers as meaningful to their associated data.
  * Start data values in row 2.
  * Ensure there are no special characters (periods, commas, ampersands, hyphens, etc.) in the headings (e.g. rename `GEO.id2` to `GEO_id2`).
  * Delete any extra columns of data that you do not need in your dataset.
 
![t11-16_1_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-16_1_new.png)

*Note: If you downloaded your TIGER data from the TIGER website, you will have to change the column in your Excel file including your `GEO_id2` field to a `Text` type. This will make it possible to join in ArcMap. If you downloaded the TIGER data from the `Create Map` feature on the FactFinder website, you can leave this column as a `General` or `Number` type.*

![t11-16_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-16_new.png)

Once the modifications to the table are made, save the file in an Excel Workbook `.xls` format (Excel 97-2003 Workbook). Close the Excel file after saving.

## Joining Excel Table to TIGER Shapefile in ArcMap

Open ArcMap and new blank map. Add the TIGER Census Tracts shapefile you unzipped to the map. You may have to `connect to folder` to locate the file. The shapefile will now be displayed on the map. Next add the Excel table to the map using the same technique. Please be aware that it will not correctly load unless you have closed the file in Excel first.

Right click on TIGER layer and select `Open Attribute Table`. When joining a shapefile to tabular data, we must have a unique ID column in both attribute tables to join on. Note that in the attribute table for the TIGER file, the field name `GEOID` matches the second ID field (`GEO_id2`) in the Excel table you formatted (you can check the attribute table of the excel file by right clicking on the table in the table of contents window and selecting `Open`. To check that they are stored as the same type of data, right click on column header `GEOID` in the attribute table and click `Properties`. Repeat this step for the `GEO_id2` column in the Excel table. Those two fields should match `Type` as a `String` type. We will use these fields to join the data.

![t11-17_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-17_new.png)

![t11-18_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-18_new.png)

Right click on the layer name of the TIGER file and select `Joins & Relates` and then `Joins`. **Note** about joins: ALWAYS join a table to the shapefile (i.e. always right click on the shapefile layer to initiate the join).

![t11-19_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-19_new.png)

In the dialog box that appears, make sure the dropdown menu asking `What do you want to join to this layer?` is set to `Join attributes from a table.` Using the `GEOID` field for the tiger file, select the table to join to the layer and use the ID field you renamed in Excel containing the 20-digit Geo ID code (GEO_id2). Before performing the join, let's click `Validate Join`. This is a way to check how many rows in each table match. In the `validation report` shown below, there is a warning because I did not remove special characters from a few of my column headers. That's fine, ArcMap will still be able to join the tables (although best practice would be to fix the column header labels in advance so as not to run into other issues). *Note* that the important information in this dialogue box is that 4918 of 4918 records matched. 

![t11-19_1.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-19_1.png)

Now we are ready to join the tables. Ensure the `Keep all records` option is checked and select `OK`. 

![t11-20.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-20.png)

You can now open the attribute table of the TIGER file to view the joined dataset (right click on the census tracts layer and select `Open Attribute Table`).

![t11-21_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-21_new.png)

We will now create a selection to include only Census Tracts in New York County. From the top menu bar go to `Select` > `Select by Attributes`. In the dialog box that appears we will build the following formula: "tl_2017_36_tract.COUNTYFP" = '061'. First, double click on "tl_2017_36_tract.COUNTYFP" to move that field to the `SELECT * FROM` formula builder box. Next, click on the equals (=) sign. Finally, click on `Get Unique Values`and scroll to '0.61', then double click on that number. Click `Apply` then `OK`. This will select only the Census tracts with the county ID number for New York County.

![t11-22_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-22_new.png)

The join is only temporary unless you export the data as a new shapefile. Right click on the data and file name in the table of contents and navigate to `Data` > `Export Data`. When prompted to `add the exported data to the map as a layer` click yes and the new shapefile will now appear in the table of contents.

![t11-23_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-23_new.png)

Once the new shapefile (only New York County tracts) is displayed, you can turn off the TIGER shapefile by clicking the box next to the layer, or you can right click on the TIGER layer to remove it from the table of contents/data frame.

## Displaying and Visualizing Census Data

To graphically analyze the dataset you created and joined we can symbolize the data using the `Symbology` under the `Layer Properties`.

![t11-24_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-24_new.png)

Right click on the newly added layer and select `Properties`. Under the tab named `Symbology`, select the “Quantities” on the left sidebar and choose `Graduated colors`. Choose the variable for the field `Total_Rent`. You can choose a color ramp or create a custom ramp by right clicking on the color ramp. If you want to classify your data using specific breaks, click the `Classify` button to choose your selected method of breaks. You can also format labels to remove decimal points or change the significant figures of the displayed data. Select `Apply` and then `OK` and your shapefile will be symbolized using your specified parameters.

![t11-25_new.png](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/Images/Tutorial_11/t11-25_new.png)

Adjust colors and add legends, scale bars, and other graphics to complete your map.

![t11-26.png](https://github.com/jai2125/gis_tutorials/blob/master/Images/Tutorial_11/t11-26.png)

## Tutorial Deliverable

Export this image and submit! 

Source: American FactFinder, United States Census Bureau. U.S. Department of Commerce, 2000 http://factfinder.census.gov/
