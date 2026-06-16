# BureauEconomicAnalysisVintageGDP

This project uses U.S. GDP vintage data published by the U.S. Bureau of Economic Analysis (BEA). The BEA regularly releases Excel files containing advance estimates and subsequent revisions of quarterly U.S. GDP levels and GDP growth rates from Q1 2002 onward.

This repository includes the relevant source data file together with a Jupyter Notebook that extracts and cleans the data. It also adds "valid from" and "valid to" timestamps for each quarterly estimate and revision.

Using this processed dataset, the notebook generates time-series dictionaries and pandas DataFrames containing historical GDP vintages and growth rates.

This enables users to analyze U.S. GDP data exactly as it would have appeared on any given historical release date.

To illustrate these revisions over time, the notebook also creates charts and animations. An interactive user interface allows users to explore the evolution of GDP estimates in detail.

Steps:

- Publication Date and readme info extraction
- read excel file from sheet 'Vintage History' into data frame 'raw'
- Data cleaning:
    - Fill nan in first column with new column to create quarter date
    - Transfer to Dataframe and assign column names
    - Split Release_Date into Release_Date and Note
    - Change Release_Date into Date time
    - Drop NaT Release_Date. These Rows are not needed
    - Change Data types of 'GDP','GDI','GDP_%_Change','GDI_%_Change'
    - Create Quarter_Date column from Quarter
    - Reset Index
- Latest Release_Date for each Quarter
- Create Valid_From and Valid_To with checks
- Which quarters have been changed during the last release date?
- Which quarter has had the most revisions?
- At which release date were the most quarters revised?
- Basic statistics
- Aggregated Results of Quarter estimations/calculations
- Calculate GDP % Change Switch
- List those quarters were an estimation of economic contraction has changed to growth or vice versa
- Calculate diff of max and min gdp change
- Build time series using validity intervals
- The time series are transfered as data frames into a dictionary
- Alternatively transfer of the time series into single data frame
- Function to recieve most recent date
- plot Gdp and GDP_%_Change and specific timespot
- Plot ALL vintages on one chart (GDP only)
- Plot one Quarter GDP across vintages (revision path)
- Plot one Quarter GDP Growth Change across vintages (revision path)
- Animate GDP Vintage Evolution (matplotlib)
- Animate GDP growth Vintage Evolution (matplotlib)
- Animate GDP growth Vintage Evolution (BAR CHART)
- UI to create plot  

## UsGdpVint_010
Update Data to release 2026-05-28

## UsGdpVint_009
Which quarter has had the most revisions?
At which release date were the most quarters revised?
Calculate diff of max and min gdp change
previous estimate within each quarter
Which quarters have been changed during the last release date and how

## UsGdpVint_008
Readme discription

## UsGdpVint_007
Animate GDP growth Vintage Evolution (matplotlib)
New Data release 2026-04-09
Animate GDP growth Vintage Evolution (BAR CHART)



## UsGdpVint_006
UI with date picker

## UsGdpVint_005
Gdp and GDP_%_Change and specific timespot different colours
Animate GDP Vintage Evolution (matplotlib)


## UsGdpVint_004
unique dates
Function to recieve most recent date
plot Gdp and GDP_%_Change and specific timespot
Plot ALL vintages on one chart (GDP only)
Plot one Quarter GDP across vintages (revision path)
Plot one Quarter GDP Growth Change across vintages (revision path)

## UsGdpVint_003
Publication Date and readme info
Aggregated Results of Quarter estimations/calculations
Calculate GDP % Change Switch
List those quarters were an estimation of economic contraction has changed to growth or vice versa

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