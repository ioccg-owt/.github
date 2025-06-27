## Data
Data for the examples were collated by Bror. The datasets are collected from different projects and harmonzied to one format. 
The goal has been to have datasets that are useful for students and other to play with clustering and water types + data that 
can be used for quick and dirty tests. They are not necessarily covering all use cases or domains. 


### File structure
Each dataset has at least the following structure:

#### Dimensions:

|name|descrition|
-----------------
| ID | row ID for the data point|
| wavelengths | wavelength for the data point |
-----------------------------------------------
 
#### Fields:
 
time (ID) - time as a pandas datetime object
lat (ID) - Latitude in decimal format
lon (ID) - Longitude in decimal format
Rrs(ID, wavelengths) - Remote sensing reflectances
 
### Datasets:
 
#### Open Ocean - Satellite
 
__IOCCG_OWT_OC-CCI_2003-2013.nc__ : Satellite based data from OC-CCI over the global ocean.
One randomly selected day each month from 2003 to 2023. Spatially stratified so that every Longhurst region has
at least 5 samples and each number is weighted to the areas of the regions. 

__IOCCG_OWT_OC-CCI_small_sample.nc__ : Satellite based data from OC-CCI over the global ocean. 
10 000 point subsample of  IOCCG_OWT_OC-CCI_2003-2013.nc spatially stratified over the Longhurst biomes so that each has at least 100 datapoints. 
 
__IOCCG_OWT_Valente_full.nc__ In-Situ data with global coverage from https://doi.org/10.5194/essd-11-1037-2019 and  https://doi.org/10.1594/PANGAEA.898188 .
 
 
#### Coastal Ocean - Satellite
 
__IOCCG_OWT_MSI-Tagus_2017-2023.nc__  : Satellite based data from MSI over the Tagus estuary in Portugal. One randomly selected day each month from 2017 to 2023. Spatially stratified so with more data points closer to shore.
 
__OCCG_OWT_MSI-Tagus_small-sample.nc__  : Satellite based data from MSI over the Tagus estuary in Portugal. 10 000 point subset of  IOCCG_OWT_MSI-Tagus_2017-2023.nc with the same spatial stratification
 
__IOCCG_OWT_ShunBi_hyper.nc__ and  __IOCCG_OWT_ShunBi_olci.nc__ in-situ data from https://doi.org/10.1002/lno.12606 and https://github.com/bishun945/pyOWT.
 
### Download 
http://monhegan.unh.edu/IOCCG_OWT/
 
Let me know what you think and if there are any issues! /Bror
 
