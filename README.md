# InstaFresh_DATA

This notebook helps to convert USDA database files into a JSON format. The database can be downloaded from: https://ndb.nal.usda.gov/ndb/

Note that the script is designed to work with ASCII files (for both SR Legacy and BFPD files).

Instructions:
1. Download the database from the above link and save it in a common folder. Make sure you download the ASCII versions.
2. First run the usdaDataToJsonConverter.ipynb notebook in the usdaToJson folder under scripts. This will create json 
files of nutrients and product data
3. Then, if needed, you can combine the nutrients and product data together to create a single json file by running
the usdaJsonProductNutrCombiner_BFPD.ipynb and usdaJsonProductNutrCombiner_SR.ipynb notebooks.
4. There is also a script called databaseUpdater. This is a node script that can help add this data to a firebase database.

Check out the images folder for the data structure of the exported json files
