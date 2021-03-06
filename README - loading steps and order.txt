Data loading steps:

First, choose if you will load using the Data Import Wizard (highly recommended for this work) or the Data Loader (more of a pro tool and can be faster, but for this work you'll probably spend more time getting the dates and Record Type ID's formatted correctly than it's worth). **These instructions are specifically for the Data Import Wizard.** If you're a power user of the Data Loader and want to use that, you can use these notes as a guideline.

0- Yes, there are a lot of data loading files. That's because there are a lot of record types in the app and in the Data 
Import Wizard you will need to load data sets one Record Type at a time. 

1- Copy all of these files to your local machine. It is recommended to add all of the loaded recordID's back to the csv files once loaded (you will get the new recordID's from the 'success' file).

2- Load files in order indicated by file name (i.e. load the “1- Building Assets load.csv” file first). In the wizard, associate the lookups with record name, not ID (the pick lists in the middle "What do you want to do?" column). 

3- For EUR records, do not load the Carbon Footprint Name column; that column is to make it easier to come back and associate the EUR and CF records (step 5). You will get the 'success' file from clicking the View Result link on the Bulk Data Load Jobs page.

4- For the most part, all fields should map automatically. If you see an unmapped field here or there (especially when loading the Carbon Footprint records) it is probably expected and intentional. 

5- Associate the loaded Energy Use Record (EUR) record with the loaded Carbon Footprint (CF) record via the loaded recordID in the Carbon Footprint Report Item (CFRI) object (this is the junction object that joins the EUR and CF records). Be careful about this. You need to visually match the EUR and CF records by their record names and types, but using the VLOOKUP formula in Excel can help with this greatly. Use the "18- CFRI load example.xlsx" file as an example/template. Keep in mind that while you can have a many-to-many mapping between CF and EUR records in the app, for this data loading project it's always 1:many between CF:EUR. If you line up all EUR and CF recordID's in one file, you should have 2115 rows in the file (2114 records and one header row). In the wizard, use the "Salesforce.com ID" choice as your lookup match instead of the record name as you did in the above steps.

** steph note: if this is confusing, check out the Junction Objects Load Helper spreadsheet! 