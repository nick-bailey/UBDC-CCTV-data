# UBDC-CCTV-data

This repository contains some examples of R code written to make use of data created by the Urban Big Data Centre (UBDC - https://www.ubdc.ac.uk) at University of Glasgow. UBDC uses object detection models on images from Glasgow City Council's CCTV system, producing hourly counts of the number of pedestrians, cyclists and vehicles for different locations across the city. The code downloads data via an API and shows how it can be processed to produce a range of urban indicators. 

* 'GALLANT' folder: code to extract data for a subset of cameras (listed in spreadsheet) and for a subset of dates. Processing first produces hourly counts, filling gaps by using rolling averages for hours either side (or for the same hour on same day in weeks before/after) in order to minimise problems with missing data. Then aggregates these to daily and monthly totals, and presents basic figures. 

### Update 2023
The API was updated in 2023 so older, redundant code has been placed in a separate folder ('Old API'). 
