# Introduction
In today's world, crime rates have surged, posing complex challenges for law enforcement globally. To tackle these issues head-on, the integration of advanced technologies and data analysis is crucial. This case study delves into how crime data analysis can elevate the effectiveness of law enforcement in a major city.
# Problem statement
1. Identify and understand crime patterns and trends.
2. Identify potential crime hotspots based on data-driven insights.
3. Enhance proactive crime prevention strategies.
# Data sourcing 
The 'Police recorded crime open data tables, year ending March 2013 onwards' release is a top-tier statistical output adhering to professional standards. Produced by Home Office statisticians\; John Flatley, it ensures objectivity and complies with the Code of Practice for Statistics.
For further information about police recorded crime statistics, please email: CrimeandPoliceStats@homeoffice.gov.uk
[Data source](https://assets.publishing.service.gov.uk/media/65afb470bc0de3000d187340/prc-pfa-mar2013-onwards-tables-250124.ods)
# Data transformation and cleaning
To make our dataset suitable for analysis, we need to clean and transform dataset by:
Creating a year column by extracting the year from the Financial year column and renamikng the column to be "YEAR"
Creating a Quarter-Year column by combining the financial quarter column and newly created year column, Change the data type of Quarter-Year to text data type.
Creating a Financial Month Column, Change data type of Financial Month to Text data type
Bring in the data set for geographical location
If the columns are missing headers, we can use the first row as the headers.
## Datasets before cleaning and transformation
<img width="907" alt="Screenshot 2024-02-23 140809" src="https://github.com/Barbiespec/criminal-record/assets/158063327/694cfefd-e6bc-46f9-9c7d-48b22137d5bd">
<img width="421" alt="Screenshot 2024-02-23 141007" src="https://github.com/Barbiespec/criminal-record/assets/158063327/3773df7a-39dc-4950-9cfd-057f1117401f">

## Datasets after cleaning and transformation
The datasets are now suitable for analysis and easy visualisation after cleaning and transforming the dataset
<img width="625" alt="Screenshot 2024-02-24 191432" src="https://github.com/Barbiespec/criminal-record/assets/158063327/103d53fe-2aee-4ae8-9fb0-794dce2fedbb">

# Data modeling
The datas in our tables have a one to many relationship, where one record from the fact table (the fact table contains the quantitative and measurable data) is linked to many record on the dimension table ( The dimension table provide context for analysis) using a unique identifier. The star schema model was used for the conceptual design.
<img width="671" alt="Screenshot 2024-02-24 191858" src="https://github.com/Barbiespec/criminal-record/assets/158063327/ae63c4c2-aaf2-4f25-973d-e6657044af5e">





