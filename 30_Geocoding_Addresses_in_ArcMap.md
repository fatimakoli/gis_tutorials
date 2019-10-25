# Geocoding Address Data in ArcMap

*This tutorial will guide you through the process of geocoding address data in ArcMap 10.6.1*

The data for this tutorial is [Day Care Centers]() in New York City. The data have been cleaned (e.g. the column headers have been adjusted to remove spaces and redundant columns have been removed). However, there is still some work to do in Excel before the data can be geocoded in ArcMap. This is often the case with datasets that contain address data and no other location information. Addresses are often contained within one column and delimited with a variety of separators (e.g. comma, tab, space, etc.).  

1. Open the dataset (DAYCARECENTERS_NYC_CLEAN.csv) in Excel. Insert a new column between STREETNAME and ZIP. Type `ADDRESS` as the column header for the new column (i.e. in cell D1).
2. We need to combine columns B and C (HOUSENUMBER and STREETNAME) in order to have a street address with number and street name in one cell. In D2 (or the second row cell in the ADDRESS column), type the formula as depicted in the image below (note there is a space between the quotation marks):

![t30-1.png]()

3. Copy the forumla down the entire ADDRESS column
4. Select the address column and COPY it (control C on a PC, or click on the `D` to select the column and right click in the selection and select `Copy`). Paste the column back into the same column (column D) by right clicking and selecting Paste Values in the Paste options (the clipboard with the 123). See below.

![t30-2.png]()

5. Save the csv with the ADDRESS column and close Excel.

Open a blank map in ArcMap. In the Catalog window, expand the folder for GIS servers and click `Add ArcGIS Server`.

![t30-3.png]()

Make sure `Use GIS Services` is selected and click `Next` for the first window. Paste the following URL in the space for `Server URL`: https://gisservices.its.ny.gov/arcgis/rest/services and click `Finish`.

Make sure you have the Geocoding toolbar in your toolbars area or click `Customize` -> `Toolbars` -> and click `Geocoding`. Click the dropdown menu (where you see ArcGIS World Geocoding) and select `Manage Address Locators`.

![t30-4.png]()

In the `Address Locator Manager` dialog box, select `Add`. Navigate (from the `Look in:` dropdown menu) to GIS Servers -> arcgis on gisservices.its.ny.gov (user) -> the Locators folder. Select `Street and Address Composite`. Click `Add` then close the `Address Locator Manager` window.

![t30-5.png]()

Navigate to the DAYCARECENTERS_NYC_CLEAN.csv file in the Catalog window. Right click on the file and select `Geocode Addresses`. In the `Select Address Locator` window, make sure the composite locator that you just added is selected. Click `OK`. In the next window of the Geocode Addresses process, select `ADDRESS` for Street or Intersection and make sure `CITY` is selected for city and `ZIP` is selected for ZIP code.

![t30-6.png]()

Click `OK`. 93\% of addresses should match (1793 addresses total). About 3\% should tie or remain unmatched. That's fine for the purposes of this lab. In the Chapter 8 tutorial, you will learn how to rematch or fix addresses that don't match. Close the Geocode Addresses window. The results are saved as a shapefile called `Geocoding Results` in the same folder (you should see this shapefile in your Catalog window within your working directory, e.g. the folder you are working in). Add the NYC_TRACTS_2010 shapefile to your dataframe and then add the Geocoding Results shapefile to your data frame. Add the UnderFiveByTract.csv file to the table of contents window. We will visualize some Census data and compare the locations of daycare centers.

1. Join the UnderFiveByTract.csv file to the TRACTS shapefile (NOTE: you will have to convert the `ct2010` field in the TRACTS attribute table to a Long... which involves adding a new field as a long and calculating the new field as `ct2010` as a number). You can join the new field to the Geo_TRACT field in the UnderFiveByTract.csv table).





