---
output:
  html_document: default
  pdf_document: default
---

# OSM_2023-2024

This repository contains data, R scripts and associated outputs, and other materials necessary for the Applied Conservation and Macro Ecology (ACME) lab's Oil Sands Monitoring project for the 2023-2024 season.

### GENERAL INFORMATION

**Project Information**\
Details for the Oil Sands Monitoring Program study design can be found [here](https://open.alberta.ca/publications/9781460151341)

Also visit the [ACME website](http://www.acmelab.ca/) more information about the OSM project and the ACME lab.

**Author Information (data):**\
*Principal Investigator Contact Information*\
Name: Jason T. Fisher, PhD\
Institution: University of Victoria\
Address: 3800 Finnerty Rd, Victoria, BC V8P 5C2\
Email: [fisherj\@uvic.ca](mailto:fisherj@uvic.ca)

**Author Information (code):**\
*Data Analysis Contact Information*\
Name: Marissa A. Dyck\
Institution: University of Victoria\
Address: 3800 Finnerty Rd, Victoria, BC V8P 5C2\
Email: [marissadyck\@uvic.ca](mailto:marissadyck@uvic.ca)

*and*

Name: Aidan Brushett\
Institution: University of Victoria\
Address: 3800 Finnerty Rd, Victoria, BC V8P 5C2\
Email: [aidanbrushett\@uvic.ca](mailto:aidanbrushett@uvic.ca)

**Date of data collection:** 2023-2024

**Geographic location of data collection:** Alberta, Canada

### DATA & FILE OVERVIEW

**File List:**

*Files in main folder*

-   [**OSM_2023-2024.Rproj**]{style="color: #7B0F17;"}; R project to run code for data cleaning and analyses.
-   [**README**]{style="color: #7B0F17;"}; this README file with extension for viewing (.html) and editing (.md)

*Files in data folder*

*/processed*\
This folder includes data for the current year (2023-2024) that has been cleaned and reformatted using scripts within this repository. It will eventually include some data from prior years (2021-2023) that was cleaned and formatted using similar scripts in a repository for that year.

-   [**OSM_covariates_2021.csv**]{style="color: #7B0F17;"}; contains cleaned HFI and land cover data from LUs sampled in 2021-2022

-   [**OSM_covariates_2022.csv**]{style="color: #7B0F17;"}; contains cleaned HFI and land cover data from LUs sampled in 2022-2022

-   **OSM_covariates_2023.csv**; contains cleaned HFI and land cover data from LUs sampled in 2022-2023

-   [**OSM_covariates_grouped_2021_2022_2023.csv**]{style="color: #7B0F17;"}; contains cleaned HFI and land cover data that have also been grouped based on feature similarity from LUs sampled in 2021-2022, 2022-2023, and 2023-2024

-   [**OSM_covariates_merged_2021_2022_2023.csv**]{style="color: #7B0F17;"}; contains cleaned HFI and land cover data from LUs sampled in 2021-2022, 2022-2023, and 2023-2024 (*Note these have not been grouped yet*)

-   **OSM_deployment_2021.csv**; contains cleaned deployment start and end dates for all camera sites sampled in 2021-2022, including information about camera failures (early ends, datetime malfunctions).

-   **OSM_deployment_2022.csv**; contains cleaned deployment start and end dates for all camera sites sampled in 2023-2024, including information about camera failures (early ends, datetime malfunctions).

-   **OSM_deployment_2023.csv**; contains cleaned deployment start and end dates for all camera sites sampled in 2023-2024, including information about camera failures (early ends, datetime malfunctions).

-   [**OSM_ind_det_2021.csv**]{style="color: #7B0F17;"}; contains independent detections for species detected on cameras from LUs sampled in 2021-2022

-   [**OSM_ind_det_2022.csv**]{style="color: #7B0F17;"}; contains independent detections for species detected on cameras from LUs sampled in 2022-2023

-   **OSM_ind_det_2023.csv**; contains independent detections for species detected on cameras from LUs sampled in 2022-2023

-   [**OSM_proportional_detections_2021.csv**]{style="color: #7B0F17;"}; contains proportional monthly presence/absences data for a subset of mammals detected on cameras from LUs sampled in 2021-2022

-   [**OSM_proportional_detections_2022.csv**]{style="color: #7B0F17;"}; contains proportional monthly presence/absences data for a subset of mammals detected on cameras from LUs sampled in 2022-2023

-   **OSM_proportional_detections_2023.csv**; contains proportional monthly presence/absences data for a subset of mammals detected on cameras from LUs sampled in 2023-2024

-   [**OSM_timelapse_2021.csv**]{style="color: #7B0F17;"}; contains cleaned image data from program Timelapse for all species and LUs sampled in 2021-2022 (not formatted into independent detections)

-   [**OSM_timelapse_2022.csv**]{style="color: #7B0F17;"}; contains cleaned image data from program Timelapse for all species and LUs sampled in 2022-2023 (not formatted into independent detections)

-   [**OSM_timelapse_2023.csv**]{style="color: #7B0F17;"}; contains cleaned **and error-checked** image data from program Timelapse for all species and LUs sampled in 2023-2024 (not formatted into independent detections).

-   [**OSM_total_detections_2022.csv**]{style="color: #7B0F17;"}; contains total independent detections for all species and LUs sampled in 2022-2023

-   **OSM_total_detections_2023.csv**; contains total independent detections for all species and LUs sampled in 2023-2024

-   [**OSM_total_presence_absence_2022.csv**]{style="color: #7B0F17;"}; contains binary presence/absences (0s, 1s) for all species and LUs sampled in 2022-2023

-   **OSM_total_presence_absence_2023.csv**; contains binary presence/absences (0s, 1s) for all species and LUs sampled in 2023-2024

*/raw*\
This folder includes raw data for the current year (2023-2024), and some for the previous years (2021-2023).

-   **landscape_unit_land_use_classifications.csv**; contains land-use type classifications (reference, mine, in situ, pre-in situ) for each Landscape Unit in the OSM monitoring program.
-   [**OSM_2023_timelapse_ddb_files.RData**]{style="color: #7B0F17;"}; contains a vector of all informative .ddb files in the ACME Netdrive containing the raw image data from image tagging.
-   **OSM_LU09_LU14_LU16_LU22_HFI_2023_20250209.csv**; contains raw data on Human Footprint Inventory (HFI) for each site sampled in 2023-2024 at varying buffer distances.
-   **OSM_LU09_LU14_LU16_LU22_VEG_2023_20250209.csv**; contains raw data on land cover for each site sampled in 2023-2024 at varying buffer distances.

*Files in figures folder*

This folder contains various plots generated in the scripts of this repository for the purposes of data visualization.

-   **2023_indv_det_graph.jpeg;** plot depicting the total number of independent detections of each species across all camera sites monitored in 2023-2024.

/array_specific_detections_occupancy

This sub-folder contains figures for each Landscape Unit's total independent detections (*[array]\_independent_detections.png*) by species and naive occupancy (*[array]\_naive_occupancy.png*) by species. The plots are not listed here.

*Files in scripts folder*

This file contains the various scripts needed for data formatting, visualization, and analysis.

-   [**0_ACME_clean_timelapse_script_2025-01-17**]{style="color: #7B0F17;"}; .rmd file and knitted .html file that will gather all of the individual imagery folders from the Netdrive, clean and append them, flag errors for manual correction, then export a clean dataset to this repository *and* a location on the Netdrive. Also cleans the deployment data from the Netdrive and exports noteworthy wildlife photos to the Netdrive.

## RAW DATA

### DATA-SPECIFIC INFORMATION FOR: [[OSM_2023_timelapse_ddb_files.Rdata]{style="color: #7B0F17;"}]

-   **Number of variables/columns:** 1
-   **Number of observations/rows:** 199

**Variable List:**

-   [**OSM_2023_timelapse_ddb_files**]{style="color: #2274A5;"}, A vector list of the location of source image tagging data on the Netdrive. Specifies full file paths to the .ddb files on the Netdrive.

## PROCESSED DATA

### DATA-SPECIFIC INFORMATION FOR: [[OSM_covariates_2023.csv]{style="color: #7B0F17;"}]

*Information on exact methods for data extraction and more specific variable descriptions can be found on the [ABMI human footprints wall to wall data download website for Year 2021](https://abmi.ca/home/data-analytics/da-top/da-product-overview/Human-Footprint-Products/HF-inventory.html)* **OR** *in the relevant_literature folder of this repository (HFI_2021_v1_0\_Metadata_Final.pdf)*.

-   **Number of variables/columns:** 119
-   **Number of observations/rows:** 3100
-   *Note: all covariate files from previous years follow the same format.*

**Variable List:**

This csv contains combined variables from the HFI and VEG raw data files ( 'OSM_LU01_LU13_LU15_LU21_HFI_2022.csv' & 'OSM_LU01_LU13_LU15_LU21_VEG_2022.csv'). Variable descriptions are the same as above except the variables names are in lowercase type and the HFI variables no longer contain the prefix 'FEATURE_TY'.

### DATA-SPECIFIC INFORMATION FOR: [[OSM_covariates_merged_2021_2022_2023.csv]{style="color: #7B0F17;"}]

-   **Number of variables/columns:** 118
-   **Number of observations/rows:** 8640
-   Note: all covariate files from previous years follow the same format.

**Variable List:**

This csv contains the combined data from OSM_covariates_2023.csv, [OSM_covariates_2022.csv]{style="color: #7B0F17;"}, and [OSM_covariates_2021.csv]{style="color: #7B0F17;"}

### DATA-SPECIFIC INFORMATION FOR: [[OSM_covariates_grouped_2021_2022_2023.csv]{style="color: #7B0F17;"}]

This csv contains data from [OSM_covariates_merged_2021_2022_2023.csv]{style="color: #7B0F17;"}, where individual features have been grouped with similar features to simplify the number of potential variables and ensure enough data to use them in a modeling framework. Additionally, features not needed for the analysis or with too few data that could not be grouped, were removed. Grouped features are defined below, and the individual features that were included within each group are provided.

*Information on specific variable descriptions can be found on the [ABMI human footprints wall to wall data download website for Year 2021](https://abmi.ca/home/data-analytics/da-top/da-product-overview/Human-Footprint-Products/HF-inventory.html)* **OR** *in the relevant_literature folder of this repository (HFI_2021_v1_0\_Metadata_Final.pdf)*.

-   **Number of variables/columns:** 21
-   **Number of observations/rows:** 8640
-   Note: all covariate files from previous years follow the same format.

**Variable List:**

-   [**array**]{style="color: #2274A5;"}, a factor with 6 levels where the first element abbreviation describes the project (e.g. OSM for Oil Sands Monitoring) and the second describes the landscape unit.

-   [**site**]{style="color: #2274A5;"}, a factor with where the first element abbreviation describes the landscape unit and the second element describes the camera site.

-   [**buff_dist**]{style="color: #2274A5;"}, a numeric measurement in meters ranging from 250 - 5000, of the buffer radius around the camera for which the proportion of associated human factors variables were calculated.

-   [**harvest**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of timber harvest within the buffer. Harvest is defined as, Areas where forestry operations have occurred (clear-cut, selective harvest, salvage logging, etc.) and includes, Harvest-area and Harvest-area-white-zone.

-   [**pipeline**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of pipelines within the buffer. Pipelines are defined as, a line of underground and overground pipes, of substantial length and capacity, used for the conveyance of petrochemicals. The physical clearing that contains underground and above-ground high pressure pipelines and were not grouped with any other variables.

-   [**roads**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of roads within the buffer. Roads are defined as, non-vegetated, impermeable surfaces used for motorized vehicle or aircraft transportation or access and includes, Airp-runway, Interchange-ramp, Ris-airp-runway, Ris-road, Road-gravel-1L, Road-gravel-2L, Road-paved-1L, Road-paved-2L, Road-paved-3L, Road-paved-4L, Road-paved-5L, Road-paved-6L, Road-paved-7L, Road-paved-div, Road-paved-undiv-1L, Road-paved-undiv-2L, Road-unclassified, Road-unimproved, Road-unpaved-1L, Road-unpaved-2L, Road-winter, and Transfer station.

-   [**seismic_lines**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of seismic lines within the buffer. Seismic lines are defined as, cleared corridors created during hydrocarbon exploration with a 3-meter buffer (6-meter total width), and were not grouped with any other variables.

-   [**seismic_lines_3D**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of 3D seismic lines (also called low-impact seismic lines) within the buffer. 3D seismic lines are defined as, cleared corridors created during hydrocarbon exploration with a 1.5-meter buffer (3-meter total width), and were not grouped with any other variables.

-   [**trails**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of trails within the buffer. Trails are defined as, cleared corridors surfaced with dirt or low vegetation for human/vehicle access, and include Trail, and Truck-trail.

-   [**transmission_lines**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of transmission lines within the buffer. Transmission lines are defined as, cleared corridors designated for the location of power transmission line infrastructure, and include Transmission-line and Ris-transmission-line.

-   [**veg_edges**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of vegetated edges within the buffer. Vegetated edges are defined as, disturbed vegetation alongside road edges, railway edges including ditches, and other industrial features, and include Vegetated-edge-railways, Vegetated-edge-roads, and Surrounding-veg.

-   [**wells**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of wells within the buffer. Wells are defined as, ground cleared for an oil/gas well pad, and include Well-abandoned, Well-bitumen, Well-cased, Well-cleared-not-confirmed, Well-cleared-not-drilled, Well-gas, Well-oil, Well-other, and Well-unknown.

-   [**lc_grassland**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of grassland within the buffer. This was renamed from LC_class110 to be more informative and was not grouped with any other variables.

-   [**lc_coniferous**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of coniferous forest within the buffer. This was renamed from LC_class210 to be more informative and was not grouped with any other variables.

-   [**lc_broadleaf**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of broadleaf forest within the buffer. This was renamed from LC_class220 to be more informative and was not grouped with any other variables.

-   [**lc_mixed**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of mixed forest within the buffer. This was renamed from LC_class230 to be more informative and was not grouped with any other variables.

-   [**lc_developed**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of developed land within the buffer. This was renamed from LC_class34 to be more informative and was not grouped with any other variables.

-   [**lc_shrub**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of shrubland within the buffer. This was renamed from LC_class50 to be more informative and was not grouped with any other variables.

-   [**osm_industrial**]{style="color: #2274A5;"}, a numeric measurement representing the proportion of various industrial features and clearings within the buffer. This includes, borrowpits (i.e., Borrowpit-dry, Borrowpit-wet, Borrowpits, Ris-borrowpits, Dugout, Lagoon, and Sump), clearings (i.e., Clearing-unknown, Clearing-wellpad-unconfirmed, Ris-clearing, Ris-clearing-unknown, and Runway), facilities (i.e., Camp-industrial, Facility-other, Facility-unknown, Mill, Misc-oil-gas-facility, Oil-gas-plant, Ris-camp-industrial, Ris-facility-operations, Ris-facility-unknown, Ris-plant, Ris-tank-farm, Ris-utilities, and Urban-industrial), and mines (i.e., Grvl-sand-pit, Mines-oilsands, Mines-pitlake, Open-pit-mine, Peat, Ris-drainage, Ris-mines-oilsands, Ris-oilsands-rms, Ris-overburden-dump, Ris-reclaim-ready, Ris-soil-salvaged, Ris-tailing-pond, Ris-waste, and Tailing-pond).

### DATA-SPECIFIC INFORMATION FOR: [[OSM_deployment_2023.csv]{style="color: #7B0F17;"}]

-   **Number of variables/columns:** 5
-   **Number of observations/rows:** 199
-   *Note: all deployment date files from previous years follow the same format.*

**Variable List:**

-   [**array**]{style="color: #2274A5;"}, factor describing the landscape unit of a camera (i.e. LU09, LU16, LU14, or LU22).

-   [**site**]{style="color: #2274A5;"}, factor where the first element abbreviation describes the landscape unit and the second element describes the camera site.

-   [**start_date**]{style="color: #2274A5;"}, date indicating when the camera was deployed.

-   [**end_date**]{style="color: #2274A5;"}, date indicating when the camera was retrieved.

-   [**camera_failure_details**]{style="color: #2274A5;"}, character describing any issues with the camera during deployment. This may include cameras stopping recording early, or incorrect date and time records.

### DATA-SPECIFIC INFORMATION FOR: [OSM_ind_det_2023.csv]

-   **Number of variables:** 8
-   **Number of cases/rows:** 34,540
-   *Note: each row corresponds to a new independent detection.*
-   *Note: all independent detection files from previous years follow the same format.*

**Variable List:**

-   **array;** a factor with 10 levels describing the landscape unit (eg., LU01)
-   **camera;** a factor with 430 levels describing the camera site
-   **site;** a factor with 430 levels where the first element abbreviation describes the landscape unit and the second element describes the camera site.
-   **species;** species present in the independent event
-   **event_start;** independent detection start date/time, format: YYYY-MM-DD HH:MM:SS
-   **event_end;** independent detection end date/time, format: YYYY-MM-DD HH:MM:SS
-   **year:** year in which the independent event was captured
-   **month;** month in which the independent event was captured (1 to 12).

### DATA-SPECIFIC INFORMATION FOR: [[OSM_proportional detections_2023.csv]{style="color: #7B0F17;"}]

This csv contains proportional monthly detection data for **selected species of interest** from all sites during 2023. There are columns for each species that total the number of months the species was detected, and columns that total the number of months the species was not detected - when these two columns are combined for each species that is used as our proportional binomial response variable.

-   **Number of variables/columns:** 28
-   **Number of observations/rows:** 198
-   *Note: all 'proportional detection' files from previous years follow the same format.*

**Variable List:**

-   [**site**]{style="color: #2274A5;"}, a factor with where the first element abbreviation describes the landscape unit and the second element describes the camera site.

-   [**black_bear - caribou**]{style="color: #2274A5;"}, each of these columns is a numeric integer representing the number of months (when a camera was active for \>=0.5 month) that a species was detected (controlling for hibernation months for black bears by removing Dec-March).

-   [**absent_black_bear - absent_caribou**]{style="color: #2274A5;"}, each of these columns is a numeric integer representing the number of months (when a camera was active for \>=0.5 month) that a species was **not** detected (controlling for hibernation months for black bears by removing Dec-March).

### DATA-SPECIFIC INFORMATION FOR: [[OSM_timelapse_2023.csv]{style="color: #7B0F17;"}]

-   **Number of variables/columns:** 41
-   **Number of observations/rows:** 285977
-   *Note: all timelapse files from previous years follow the same format, but do not have a fullpath or datasource columns.*
-   For more information on tagging details, consult the ACME OSM Image Tagging Protocol

**Variable List:**

-   [**file**]{style="color: #2274A5;"}, character with the name of the original camera image

-   [**relativepath**]{style="color: #2274A5;"}, character with the relative path of the image compared to the .ddb file

-   [**datetime**]{style="color: #2274A5;"}, datetime, the date and time the image was taken. A leading space has been added to prevent parsing issues in MS Excel.

-   [**array**]{style="color: #2274A5;"}, factor describing the landscape unit of a camera (i.e. LU09, LU16, LU14, or LU22).

-   [**camera**]{style="color: #2274A5;"}, factor describing the identity of the camera site within an array

-   [**site**]{style="color: #2274A5;"}, factor where the first element abbreviation describes the landscape unit and the second element describes the camera site.

-   [**classifier**]{style="color: #2274A5;"}, character, the person who tagged the image data

-   [**snow**]{style="color: #2274A5;"}, factor, the percent snow cover on the ground in the image

-   [**species**]{style="color: #2274A5;"}, factor, the identity of the species present in the image

-   [**total**]{style="color: #2274A5;"}, numeric, the total number of animals in the image

-   [**male**]{style="color: #2274A5;"}, numeric, the total number of male animals in the image. Only for animals larger than coyotes.

-   [**female**]{style="color: #2274A5;"}, numeric, the total number of female animals in the image. Only for animals larger than coyotes.

-   [**unknownsex**]{style="color: #2274A5;"}, numeric, the total number of animals with unidentifiable sex in the image. Only for animals larger than coyotes.

-   [**adult**]{style="color: #2274A5;"}, numeric, the total number of adult animals in the image. Only for animals larger than coyotes.

-   [**yly**]{style="color: #2274A5;"}, numeric, the total number of yearling animals in the image. Only for animals larger than coyotes.

-   [**yoy**]{style="color: #2274A5;"}, numeric, the total number of young of year animals in the image. Only for animals larger than coyotes.

-   [**unknownage**]{style="color: #2274A5;"}, numeric, the total number of animals with unidentifiable age in the image. Only for animals larger than coyotes.

-   [**group_count**]{style="color: #2274A5;"}, numeric, the total number of animals in the event image sequence (see event column)

-   [**g_male**]{style="color: #2274A5;"}, numeric, the total number of male animals in the event image sequence (see event column). Only for animals larger than coyotes.

-   [**g_female**]{style="color: #2274A5;"}, numeric, the total number of female animals in the event image sequence (see event column). Only for animals larger than coyotes.

-   [**g_unknownsex**]{style="color: #2274A5;"}, numeric, the total number of animals with unidentifiable sex in the event image sequence (see event column). Only for animals larger than coyotes.

-   [**g_adult**]{style="color: #2274A5;"}, numeric, the total number of adult animals in the event image sequence (see event column). Only for animals larger than coyotes.

-   [**g_yly**]{style="color: #2274A5;"}, numeric, the total number of yearling animals in the event image sequence (see event column). Only for animals larger than coyotes.

-   [**g_yoy**]{style="color: #2274A5;"}, numeric, the total number of young of year animals in the event image sequence (see event column). Only for animals larger than coyotes.

-   [**gunknownage**]{style="color: #2274A5;"}, numeric, the total number of animals with unidentifiable age in the event image sequence (see event column). Only for animals larger than coyotes.

-   [**event**]{style="color: #2274A5;"}, factor, indicates the first and last image in an event. An "event" is a continuous sequence of images where fewer than 60 seconds pass between two successive images. Singleton events are not tagged.

-   [**empty**]{style="color: #2274A5;"}, logical, whether an animal is present in the image

-   [**coatcolor**]{style="color: #2274A5;"}, factor, the coat color of one of the animals in the image. Only for bears, wolves, and foxes.

-   [**leftantler**]{style="color: #2274A5;"}, factor, the number of left antler tines for ungulates. Only for specific months (species specific)

-   [**rightantler**]{style="color: #2274A5;"}, factor, the number of right antler tines for ungulates. Only for specific months (species specific)

-   [**lcount**]{style="color: #2274A5;"}, factor, whether the left tine count is a total or minimum estimate.

-   [**rcount**]{style="color: #2274A5;"}, factor, whether the right tine count is a total or minimum estimate.

-   [**comments**]{style="color: #2274A5;"}, character, miscellaneous comments about the image

-   [**otherspecify**]{style="color: #2274A5;"}, character, details when 'other' is entered for species or camera malfunction

-   [**cameramalfunction**]{style="color: #2274A5;"}, factor, details about camera errors such as trigger malfunction or repositioning

-   [**noteworthy**]{style="color: #2274A5;"}, logical, whether the photo is noteworthy and should be saved for reporting

-   [**fullpath**]{style="color: #2274A5;"}, character, the filepath to the original image on the Netdrive

-   [**datasource**]{style="color: #2274A5;"}, character, the filepath to the original .ddb on the Netdrive containing the image data

-   [**month**]{style="color: #2274A5;"}, numeric, month the image was taken

-   [**day**]{style="color: #2274A5;"}, numeric, day the image was taken

-   [**year**]{style="color: #2274A5;"}, numeric, year the image was taken

### DATA-SPECIFIC INFORMATION FOR: [[OSM_total_detections_2023.csv]{style="color: #7B0F17;"}]

This csv contains the total number of independent detections for all species and sites during 2022.

-   **Number of variables/columns:** 37
-   **Number of observations/rows:** 199
-   *Note: all 'total detection' files from previous years follow the same format.*

**Variable List:**

-   [**site**]{style="color: #2274A5;"}, a factor with where the first element abbreviation describes the landscape unit and the second element describes the camera site.

-   [\*\*Blackbear - Canada goose\*]{style="color: #2274A5;"}, each of these columns is a numeric integer representing the number of independent detections (images taken at least 30-min apart) for each species at each site during the entire study period.
