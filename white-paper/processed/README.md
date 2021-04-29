# Overview
This repository contains processed flare observation data for major oil and gas areas in the Lower 48 states of the U.S.. Data includes processed VIIRS data, satellite-estimated Flaring Volumes, state-reported Flaring Volumes both volumetrically and in their CO<sub>2</sub> equivalents. This data has been created by synthesizing VIIRS measurements with cleaned well meta and production data sourced from public regulatory authorities in New Mexico, Texas, North Dakota and Colorado . 

**Note:** Ongoing data updates and refreshes will be pushed to this repo.

# Important Note About File Sizes
Some of these files are over 1M rows and will not open in Microsoft Excel. You should be prepared to edit very large files, or else write code to manipulate them.

Data files are loaded into a Postgres SQL database given Excel file size limitations.

# Files in Processed Repository  

| File Name                                           | Description                                                                                                                                                                                                                                                                                   |
| --------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| flaring_monitor_basin_stats.csv                     | Contains Flaring Monitor satellite-estimated Flaring Volumes and tons of equivalent CO<sub>2</sub> emitted for the Permian, Eagle Ford, Denver Julesburg – Niobrara (Colorado only) and Bakken (North Dakota only). Data is available from 2019 onwards and is aggregated at the Basin level. |
| flaring_monitor_company_stats_satellite_modeled.csv | Flaring Monitor satellite-estimated Flaring Volumes and tons of equivalent CO<sub>2</sub> emitted organized by Operator. The data is available for Operators in the states of Texas, New Mexico and North Dakota and is available from 2019 onwards.                                          |
| flaring_monitor_company_stats_reported.csv          | State reported flaring volumes and tons of equivalent CO<sub>2</sub> emitted for Texas, New Mexico, Colorado and North Dakota. The data is aggregated by Operator.                                                                                                                            |
| flaring_monitor_detailed_observations.csv           | Unprocessed satellite radiant heat measurements from VIIRS in MW hours, associated estimated flared volume and tons of equivalent CO<sub>2</sub> emitted by well cluster for operators in Texas, New Mexico and North Dakota. Data is available from 2019 onwards.                            |
