# Traffic_Monitoring_Guide_2001_R

Use this to import multiple files from the 2001 Traffic Monitoring Guide and Output them into a combined and more readable format.

## Description

The Traffic Monitoring Guide is a document published the Federal Department of Highways that provides guidance to State highway departments "about the policies, standards, procedures, reporting, and equipment utilized in a traffic monitoring program". The most recent edition can be found here:

- https://www.fhwa.dot.gov/policyinformation/tmguide/

The 2001 edition provided Traffic Monitoring Data Formats for Automatic Traffic Recorder Data as well as short-term class and volume counts.  This python script will take outputs in these formats and combine them into a more readable dataset.

The 2001 Traffic Monitoring Guide can be found here:

- https://www.fhwa.dot.gov/policyinformation/tmguide/2001_TMG_Chapter_6.pdf

The documentation of the fields below are mostly a reprint of the above document.

## To use this script

- After cloning the repo locally, create the following subdirectories<br>
  - input
    - volume
    - class
  - output

- Then place the appropriate files of each type in the input folder.

- Run the script.

- The files will be placed in the output directory.  Each type of output will be combined into one file.

## TRAFFIC CLASS DATA FORMATS

| Field | Columns | Length | Description |
| ---: | ---: | ---: | :--- |
| 1 | 1 | 1 | Record Type |
| 2 | 2-3 | 2 | FIPS State Code |
| 3 | 4-9 | 6 | Station ID |
| 4 | 10 | 1 | Direction of Travel Code |
| 5 | 11 | 1 | Lane of Travel |
| 6 | 12-13 | 2 | Year of Data |
| 7 | 14-15 | 2 | Month of Data |
| 8 | 16-17 | 2 | Day of Data |
| 9 | 18-19 | 2 | Hour of Data |
| 10 | 20-24 | 5 | Total Volume |
| 11 | 25-29 | 5 | Class 1 Count |
| 12 | 30-34 | 5 | Class 2 Count |
| 13 | 35-39 | 5 | Class 3 Count |
| 14 | 40-44 | 5 | Class 4 Count |
| 15 | 45-49 | 5 | Class 5 Count |
| 16 | 50-54 | 5 | Class 6 Count |
| 17 | 55-59 | 5 | Class 7 Count |
| 18 | 60-64 | 5 | Class 8 Count |
| 19 | 65-69 | 5 | Class 9 Count |
| 20 | 70-74 | 5 | Class 10 Count |
| 21 | 75-79 | 5 | Class 11 Count |
| 22 | 80-84 | 5 | Class 12 Count |
| 23 | 85-89 | 5 | Class 13 Count |
| 24 | 90-94 | 5 | Class 14 Count (optional) |
| 25 | 95-99 | 5 | Class 15 Count (optional) |



## TRAFFIC VOLUME DATA FORMATS
| Field | Columns | Length | Description |
| ---: | ---: | ---: | :--- |
| 1 | 1 | 1 | Record Type |
| 2 | 2-3 | 2 | FIPS State Code |
| 3 | 4-5 | 2 | Functional Classification |
| 4 | 6-11 | 6 | Station Identification |
| 5 | 12 | 1 | Direction of Travel |
| 6 | 13 | 1 | Lane of Travel |
| 7 | 14-15 | 2 | Year of Data |
| 8 | 16-17 | 2 | Month of Data |
| 9 | 18-19 | 2 | Day of Data |
| 10 | 20 | 1 | Day of Week |
| 11 | 21-25 | 5 | Traffic Volume Counted, 00:01 - 01:00 |
| 12 | 26-30 | 5 | Traffic Volume Counted, 01:01 - 02:00 |
| 13 | 31-35 | 5 | Traffic Volume Counted, 02:01 - 03:00 |
| 14 | 36-40 | 5 | Traffic Volume Counted, 03:01 - 04:00 |
| 15 | 41-45 | 5 | Traffic Volume Counted, 04:01 - 05:00 |
| 16 | 46-50 | 5 | Traffic Volume Counted, 05:01 - 06:00 |
| 17 | 51-55 | 5 | Traffic Volume Counted, 06:01 - 07:00 |
| 18 | 56-60 | 5 | Traffic Volume Counted, 07:01 - 08:00 |
| 19 | 61-65 | 5 | Traffic Volume Counted, 08:01 - 09:00 |
| 20 | 66-70 | 5 | Traffic Volume Counted, 09:01 - 10:00 |
| 21 | 71-75 | 5 | Traffic Volume Counted, 10:01 - 11:00 |
| 22 | 76-80 | 5 | Traffic Volume Counted, 11:01 - 12:00 |
| 23 | 81-85 | 5 | Traffic Volume Counted, 12:01 - 13:00 |
| 24 | 86-90 | 5 | Traffic Volume Counted, 13:01 - 14:00 |
| 25 | 91-95 | 5 | Traffic Volume Counted, 14:01 - 15:00 |
| 26 | 96-100 | 5 | Traffic Volume Counted, 15:01 - 16:00 |
| 27 | 101-105 | 5 | Traffic Volume Counted, 16:01 - 17:00 |
| 28 | 106-110 | 5 | Traffic Volume Counted, 17:01 - 18:00 |
| 29 | 111-115 | 5 | Traffic Volume Counted, 18:01 - 19:00 |
| 30 | 116-120 | 5 | Traffic Volume Counted, 19:01 - 20:00 |
| 31 | 121-125 | 5 | Traffic Volume Counted, 20:01 - 21:00 |
| 32 | 126-130 | 5 | Traffic Volume Counted, 21:01 - 22:00 |
| 33 | 131-135 | 5 | Traffic Volume Counted, 22:01 - 23:00 |
| 34 | 136-140 | 5 | Traffic Volume Counted, 23:01 - 24:00 |
| 35 | 141 | 1 | Restrictions |