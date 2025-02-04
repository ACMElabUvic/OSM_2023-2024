---
output:
  html_document: default
  pdf_document: default
---
# OSM_2023-2024
This repository contains data, R scripts and associated outputs, and other materials necessary for the Applied Conservation and Macro Ecology (ACME) lab's Oil Sands Monitoring project for the 2023-2024 season.

<hr>


### GENERAL INFORMATION

**Project Information**   
Details for the Oil Sands Monitoring Program study design can be found [here](https://open.alberta.ca/publications/9781460151341)  

Also visit the [ACME website](http://www.acmelab.ca/) more information about the OSM project and the ACME lab.

**Author Information (data):**  
 *Principal Investigator Contact Information*  
 Name: Jason T. Fisher, PhD   
 Institution: University of Victoria  
 Address: 3800 Finnerty Rd, Victoria, BC V8P 5C2  
 Email: [fisherj@uvic.ca](mailto:fisherj@uvic.ca) 

**Author Information (code):**  
*Data Analysis Contact Information*  
		Name: Marissa A. Dyck  
		Institution: University of Victoria   
		Address: 3800 Finnerty Rd, Victoria, BC V8P 5C2   
		Email: [marissadyck@uvic.ca](mailto:marissadyck@uvic.ca) 
		
*and*

Name: Aidan Brushett  
Institution: University of Victoria   
Address: 3800 Finnerty Rd, Victoria, BC V8P 5C2   
Email: [aidanbrushett@uvic.ca](mailto:aidanbrushett@uvic.ca)  
		
**Date of data collection:** 2023-2024

**Geographic location of data collection:** Alberta, Canada


### DATA & FILE OVERVIEW

**File List:**  

*Files in main folder*
		
* <span style = "color: #7B0F17;">**OSM_2023-2024.Rproj**</span>; R project to run code for data cleaning and analyses. 
* <span style = "color: #7B0F17;">**README**</span>; this README file with extension for viewing (.html) and editing (.md) 

*Files in data folder*

*/processed*  
This folder includes data for the current year (2023-2024) that has been cleaned and reformatted using scripts within this repository. It will eventually include some data from prior years (2021-2023) that was cleaned and formatted using similar scripts in a repository for that year. 

* <span style = "color: #7B0F17;">**OSM_timelapse_2023.csv**</span>;  contains cleaned **and error-checked** image data from program Timelapse for all species and LUs sampled in 2023-2024 (not formatted into independent detections).

* <span style = "color: #7B0F17;">**OSM_deployment-dates_2023.csv**</span>;  contains cleaned deployment start and end dates for all camera sites sampled in 2023-2024, including information about camera failures (early ends, datetime malfunctions).


*/raw*  
This folder includes raw data for the current year (2023-2024), and some for the previous years (2021-2023). 

* <span style = "color: #7B0F17;">**OSM_2023_timelapse_ddb_files.RData**</span>; contains a vector of all informative .ddb files in the ACME Netdrive containing the raw image data from image tagging. 


*Files in figures folder*   

This folder contains various plots generated in the scripts of this repository for the purposes of data visualization.  

* No files yet.


*Files in scripts folder* 

This file contains the various scripts needed for data formatting, visualization, and analysis.

* <span style = "color: #7B0F17;">**0_ACME_clean_timelapse_script_2025-01-17**</span>; .rmd file and knitted .html file that will gather all of the individual imagery folders from the Netdrive, clean and append them, flag errors for manual correction, then export a clean dataset to this repository *and* a location on the Netdrive. Also cleans the deployment data from the Netdrive and exports noteworthy wildlife photos to the Netdrive. 


## RAW DATA   

### DATA-SPECIFIC INFORMATION FOR: [<span style = "color: #7B0F17;"> OSM_2023_timelapse_ddb_files.Rdata</span>]  

* **Number of variables/columns:** 1  
* **Number of observations/rows:** 199  

**Variable List:**

* <span style = "color: #2274A5;">**OSM_2023_timelapse_ddb_files**</span>, A vector list of the location of source image tagging data on the Netdrive. Specifies full file paths to the .ddb files on the Netdrive. 


## PROCESSED DATA

### DATA-SPECIFIC INFORMATION FOR: [<span style = "color: #7B0F17;"> OSM_deployment-dates_2023.csv</span>]  

* **Number of variables/columns:** 5  
* **Number of observations/rows:** 199  

**Variable List:**

* <span style = "color: #2274A5;">**array**</span>, factor describing the landscape unit of a camera (i.e. LU09, LU16, LU14, or LU22).  

* <span style = "color: #2274A5;">**site**</span>, factor where the first element abbreviation describes the landscape unit and the second element describes the camera site.  

* <span style = "color: #2274A5;">**start_date**</span>, date indicating when the camera was deployed.   

* <span style = "color: #2274A5;">**end_date**</span>, date indicating when the camera was retrieved.  

* <span style = "color: #2274A5;">**camera_failure_details**</span>, character describing any issues with the camera during deployment. This may include cameras stopping recording early, or incorrect date and time records.


## PROCESSED DATA

### DATA-SPECIFIC INFORMATION FOR: [<span style = "color: #7B0F17;"> OSM_timelapse_2023.csv</span>]  

* **Number of variables/columns:** 41  
* **Number of observations/rows:** 285977  
* *Note: all timelapse files from previous years follow the same format.*  
* For more information on tagging details, consult the ACME OSM Image Tagging Protocol  

**Variable List:**

* <span style = "color: #2274A5;">**file**</span>, character with the name of the original camera image

* <span style = "color: #2274A5;">**relativepath**</span>, character with the relative path of the image compared to the .ddb file

* <span style = "color: #2274A5;">**datetime**</span>, datetime, the date and time the image was taken. A leading space has been added to prevent parsing issues in MS Excel.

* <span style = "color: #2274A5;">**array**</span>, factor describing the landscape unit of a camera (i.e. LU09, LU16, LU14, or LU22).  

* <span style = "color: #2274A5;">**camera**</span>, factor describing the identity of the camera site within an array  

* <span style = "color: #2274A5;">**site**</span>, factor where the first element abbreviation describes the landscape unit and the second element describes the camera site.  

* <span style = "color: #2274A5;">**classifier**</span>, character, the person who tagged the image data

* <span style = "color: #2274A5;">**snow**</span>, factor, the percent snow cover on the ground in the image

* <span style = "color: #2274A5;">**species**</span>, factor, the identity of the species present in the image

* <span style = "color: #2274A5;">**total**</span>, numeric, the total number of animals in the image

* <span style = "color: #2274A5;">**male**</span>, numeric, the total number of male animals in the image. Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**female**</span>, numeric, the total number of female animals in the image. Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**unknownsex**</span>, numeric, the total number of animals with unidentifiable sex in the image. Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**adult**</span>, numeric, the total number of adult animals in the image. Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**yly**</span>, numeric, the total number of yearling animals in the image. Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**yoy**</span>, numeric, the total number of young of year animals in the image. Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**unknownage**</span>, numeric, the total number of animals with unidentifiable age in the image. Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**group_count**</span>, numeric, the total number of animals in the event image sequence (see event column)

* <span style = "color: #2274A5;">**g_male**</span>, numeric, the total number of male animals in the event image sequence (see event column). Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**g_female**</span>, numeric, the total number of female animals in the event image sequence (see event column). Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**g_unknownsex**</span>, numeric, the total number of animals with unidentifiable sex in the event image sequence (see event column). Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**g_adult**</span>, numeric, the total number of adult animals in the event image sequence (see event column). Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**g_yly**</span>, numeric, the total number of yearling animals in the event image sequence (see event column). Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**g_yoy**</span>, numeric, the total number of young of year animals in the event image sequence (see event column). Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**gunknownage**</span>, numeric, the total number of animals with unidentifiable age in the event image sequence (see event column). Only for animals larger than coyotes.

* <span style = "color: #2274A5;">**event**</span>, factor, indicates the first and last image in an event. An "event" is a continuous sequence of images where fewer than 60 seconds pass between two successive images. Singleton events are not tagged.

* <span style = "color: #2274A5;">**empty**</span>, logical, whether an animal is present in the image

* <span style = "color: #2274A5;">**coatcolor**</span>, factor, the coat color of one of the animals in the image. Only for bears, wolves, and foxes.

* <span style = "color: #2274A5;">**leftantler**</span>, factor, the number of left antler tines for ungulates. Only for specific months (species specific)

* <span style = "color: #2274A5;">**rightantler**</span>, factor, the number of right antler tines for ungulates. Only for specific months (species specific)

* <span style = "color: #2274A5;">**lcount**</span>, factor, whether the left tine count is a total or minimum estimate.

* <span style = "color: #2274A5;">**rcount**</span>, factor, whether the right tine count is a total or minimum estimate.

* <span style = "color: #2274A5;">**comments**</span>, character, miscellaneous comments about the image

* <span style = "color: #2274A5;">**otherspecify**</span>, character, details when 'other' is entered for species or camera malfunction

* <span style = "color: #2274A5;">**cameramalfunction**</span>, factor, details about camera errors such as trigger malfunction or repositioning

* <span style = "color: #2274A5;">**noteworthy**</span>, logical, whether the photo is noteworthy and should be saved for reporting

* <span style = "color: #2274A5;">**fullpath**</span>, character, the filepath to the original image on the Netdrive

* <span style = "color: #2274A5;">**datasource**</span>, character, the filepath to the original .ddb on the Netdrive containing the image data

* <span style = "color: #2274A5;">**month**</span>, numeric, month the image was taken

* <span style = "color: #2274A5;">**day**</span>, numeric, day the image was taken

* <span style = "color: #2274A5;">**year**</span>, numeric, year the image was taken





