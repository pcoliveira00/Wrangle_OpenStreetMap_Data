# Wrangle_OpenStreetMap_Data

# Choose any area of the world from https://www.openstreetmap.org, and download a XML OSM dataset. The dataset should be at least 50MB in size (uncompressed). We recommend using one of the following methods to download a dataset:

Use the Overpass API to download a custom square area. Explanation of the syntax can found in the wiki. In general you will want to use the following query:(node(minimum_latitude, minimum_longitude, maximum_latitude, maximum_longitude);<;);out meta; e.g. (node(51.249,7.148,51.251,7.152);<;);out meta; the meta option is included so the elements contain timestamp and user information.
You can use the Open Street Map Export Tool to find the coordinates of your bounding box. Note: You may not be able to use the Export Tool to actually download the data, the area required for this project is too large. After selecting a region, you can try clicking the Overpass_API link down the tool bar to perform the export and download.

Thoroughly audit and clean your dataset, converting it from XML to JSON format. Then import the cleaned .json file into a MongoDB database.
