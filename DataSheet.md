# Datasheet

## Motivation

- The dataset 'london_weather.csv' was created by Klein Tank, A.M.G. and Coauthors for the ECA&D project. For all information on the motivation behind the project, please see the Rationale section in https://knmi-ecad-assets-prd.s3.amazonaws.com/documents/ECAD_datapolicy.pdf.

 
## Composition

- Each instance in the dataset represents a day. The data comprises on information on the date, the cloud cover, sunshine, global radiation, the maximum temperature, the mean temperature, the minimum temperature, precipitation, pressure and snow depth
- There are 15,341 instances
- There is missing data, particularly in the snow_depth variable. To handle this, the snow_depth was ignored and any rows with missing data in other columns were removed.

## Collection process

- The ECA dataset contains series of daily observations at meteorological stations throughout Europe and the Mediterranean
- Only a portion of the larger data set has been made available for public use. 
- The dataset contains data from the start of 1979 through to the end of 2020.

## Preprocessing/cleaning/labelling

- The jupiter notebook contains some preprocessing. This involves replacing the date with the month that it represents, removing the snow_depth variable and then removing any rows that are left that contain missing data. 
 
## Uses

- This data could be used for plenty of other purposes, such as predictive modelling of future london weather. 

## Distribution

- The dataset can be found on kaggle: https://www.kaggle.com/datasets/emmanuelfwerr/london-weather-data?resource=download. It is not subject to any copyright claims as it is a subset of a larger dataset that has been made available for public use.

