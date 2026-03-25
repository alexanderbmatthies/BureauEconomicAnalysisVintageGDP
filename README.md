# BureauEconomicAnalysisVintageGDP

## UsGdpVint_002
create quarter date
Transfer to Dataframe
Assign column names
Data Cleaning:
    Split Release_Date into Release_Date and Note
    Change Release_Date into Date time
    Change Release_Date into Date time
    Drop NaT Release_Date. These Rows are not needed
    Change Data types of 'GDP','GDI','GDP_%_Change','GDI_%_Change'
    Create Quarter_Date column from Quarter.
    Reset Index
Create Valid_From and Valid_To
Build time series using validity intervals
time series are transfered as data frames into a dictionary


## UsGdpVint_001
First Branch Load File.
Define first Data cleaning steps