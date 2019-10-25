# Geocoding Address Data in ArcMap

*This tutorial will guide you through the process of geocoding address data in ArcMap 10.6.1*

The data for this tutorial is [Day Care Centers](https://github.com/alisaalias/gis_tutorials/blob/alisaalias-patch-1/data/Tutorial_30_Data.xlsx) in New York City. The data have been cleaned (e.g. the column headers have been adjusted to remove spaces and redundant columns have been removed). However, there is still some work to do in Excel before the data can be geocoded in ArcMap. This is often the case with datasets that contain address data and no other location information. Addresses are often contained within one column and delimited with a variety of separators (e.g. comma, tab, space, etc.).  

1. Open the dataset (DAYCARECENTERS_NYC_CLEAN.csv) in Excel. Insert a new column between STREETNAME and ZIP. Type `ADDRESS` as the column header for the new column (i.e. in cell D1).
2. We need to combine columns B and C (HOUSENUMBER and STREETNAME) in order to have a street address with number and street name in one cell. In D2 (or the second row cell in the ADDRESS column), type the formula as depicted in the image below (note there is a space between the quotation marks):

![t30-1.png]()

3. Copy the forumla down the entire ADDRESS column
4. Select the address column and COPY it (control C on a PC, or click on the `D` to select the column and right click in the selection and select `Copy`). Paste the column back into the same column (column D) by right clicking and selecting Paste Values in the Paste options (the clipboard with the 123). See below.

![t30-2.png]()
