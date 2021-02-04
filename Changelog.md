# Detailed Changelog 

# 2/3/2020 by Stephanie Ho
* Generally updated all data to work with FY22 org (thanks Surabhi!) ex. FY20 -> FY21
* Added a new asset (Wolf Point Plaza) that demos Data Gap Filling nicely
* Added a leading 0 to filenames so it sorts correctly in github
* Added a new file 21- optional CF PriorYear.csv so you can chain together the "Prior Year Carbon Footprint" on Carbon Footprints. I also added it to Junction Objects Load Helper.
### Data Updated 
Building Assets
* Added Wolf Point Plaza 

General Assets
* Time shifted 1 year (ex. FY20 -> FY21)

EUR - Comm Building 
* Time shifted 1 year
* Added EURs for Wolf Point Plaza

All other EURs 
* Time shifted 1 year

All Carbon Footprints
* Time shifted 1 year
* Data - Stage picklist: "Interpolation" -> "Data Gap Filling"
* Column - Extrapolation Status -> Data Gap Status
### Junction Objects Load Helper
* Time shifted 1 year
* Added new sheet PriorYear <date> and instructions on how to use it.
# 9/10/2020 by Stephanie Ho 
* Updated to work with 1.11

### Data Updated  

Building Assets 
* Changed column name Zip Code to Postal Code 

Vehicle Assets 
* Removed blank Zip Code and Facility ID columns  

EUR - Air Travel 
* Scope 3 Travel Factors → Air Travel Factors 

EUR - Fleet Vehicle 
* Scope 3 Travel Factors → Vehicle Emissions Factors 

EUR - Ground Travel 
* In Expense Type picklist... Personal Car Mileage → Personal Car Distance
* Scope 3 Travel Factors → Scope 3 Ground Travel - APAC/EMEA/AMER
* Changed column header Trip Amount in USD → Trip Cost
* Deleted Business Region and Country columns

EUR Hotel Stays 
* Scope 3 Travel Factors → Correct country travel factor 

EUR Rental Cars 
* Added columns Emissions Factors - Scope 3, Distance Unit, Trip Distance (but kept vendor provided emissions) 

Carbon Footprint - Travel
* Removed Allocation Status and Extrapolation Status columns

Carbon Footprint - Vehicles
* Removed Allocation Status and Extrapolation Status columns

# 8/24/2020 by Stephanie Ho
* Some pre-release field name fixes
* Synced w internal folder and other admin work to make it easier for myself
* changed this to a .md so my formatting actually shows up 

# 06/11/2020 by Stephanie Ho
*Should be working with 1.9 release*

* Added a Junction Objects Load Helper xls which should help with creating Carbon Footprint Report Items and Asset Contact Items. 
* Added an example of what an Asset Contact Item csv should look like

### Data Updated

EUR - Commercial Buildings

* 94061 - eGRID2016 → CAMX - eGRID2018
* General Conversion Factors → GeneralConversionFactors

EUR - DC 

* 80027 - eGRID2016 → RMPA - eGRID2018
* 10025 - eGRID2016 → NYCW - eGRID2018
* General Conversion Factors → GeneralConversionFactors

EUR - Private Jet 

* General Conversion Factors → GeneralConversionFactors