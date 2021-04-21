# Overview
This repository contains raw CSVs of VIIRS flare observation data are in the "raw" directory. These are used by the viirs-flare-code repository (*flaringmonitor/viirs-flare-code*) to produce Flaring Monitor satellite-estimated flare volumes organized by Operator and by Basin.

# Important Note About File Sizes
Some of these files are over 1M rows and will not open in Microsoft Excel. You should be prepared to edit very large files, or else write code to manipulate them.

Data files are loaded into a Postgres SQL database given Excel file size limitations.

# Files in Raw Repository  

| File name               | Description                                                                                                                                              |
|-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| flare_prod.csv.gz       | For a given API and month is well expected to be producing oil and/or gas                                                                                |
| flare_wells.csv.gz      | For a given API provides state, location, the most recent operator and operator ticker if available.                                                     |
| lower_48_basins.csv.gz  | EIA basin map                                                                                                                                            |
| mapping_combined.csv.gz | Mapping of ticker to name                                                                                                                                |
| reported_flares.csv.gz  | Monthly flaring as reported to state regulatory agencies. key_type and key provide a reference to the well or lease record in which this data was found. |
| states.csv.gz           | State map                                                                                                                                                |
| viirs.csv.gz            | VIIRS radiant heat data for our four states (North Dakota, New Mexico, Texas, Colorado) region of interest                                               |
