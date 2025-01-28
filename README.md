# ML-for-Fire-Fighters
README


1. Execution Sequence
1)	EDA
Script: 
Code/EDA/EDA.ipynb
Input: 
Data/incident_cleaned_final.csv

2)	ResourceAllocation
Script: 
Code/Resource Allocation/HeatMapsForResources.ipynb
Input:
Data/incident_cleaned_final.csv

Script: 
Code/Resource Allocation/InteractiveMaps.ipynb
Input:
RFD_Station_Locations files (shx, shp, prj, dbf, cpg, shp.xml, sbx, sbn): 
tl_2024_us_zcta520 (prj, cpg, shx, shp, dbf, shp.iso.xml, shp.ea.iso,xml): 
incident_cleaned_final.csv 
Output:
Map1_Average_Response_Time_and_Incident_Analysis_by_ZIP_2019-2024.html
Map2_Incident_Type_Distribution_and_Fire_Station_Workload_2019-2024.html
Script: 
Code/Map for Predicted Counts.ipynb
Input:
RFD_Station_Locations files (shx, shp, prj, dbf, cpg, shp.xml, sbx, sbn): 
data/Predicted Monthly Incident Counts/<station_name_historical_forecasted_values.csv 

3)	DataCleaning&Preparation
 Script: Code/incident_cleaning_final.ipynb
 Input: 
data/incident_report_dataset.csv
data/incident_cleaned_geocoded_v3.csv
data/RFD_Station_Locations.shp
 Output: data/incident_cleaned_final.csv
Script: Code/incident_counts_by_station.ipynb
Input: data/incident_cleaned_final.csv
Output: data/Per Station per Month/<station_name>_monthly.csv


4)	ModelBuilding
 Script: Code/Feature Selection & Forecasting Selected Independent Features.ipynb
 Input: data/Per Station per Month/<station_name>monthly.csv
 Output: data/Historical_Forecasted_Independent_Feat/<station_name>_past_future.csv
data/forecasted_indep_feat_validation_metrics/<station_name>_fc_val.csv

Script: Code/Improving Independent Features' Forecast and Predicting Monthly Counts.ipynb
Input:
data/Historical_Forecasted_Independent_Feat/<station_name>_past_future.csv
data/forecasted_indep_feat_validation_metrics/<station_name>_fc_val.csv
Output: data/Predicted Monthly Incident Counts/<station_name_historical_forecasted_values.csv



2. Folder Structure
ML-for-Fire-Fighters
 ├── Code/
 │ ├── DataCleaning&Preparation
 │ │ ├── incident_cleaning_final.ipynb
 │ │ ├── incident_counts_by_station.ipynb
 │ ├── EDA
 │ │ ├── EDA.ipynb
 │ ├── ModelBuilding
 │ │ ├── Feature Selection & Forecasting Selected Independent Features.ipynb 
 │ │ ├── Improving Independent Features' Forecast and Predicting Monthly Counts.ipynb 
 │ ├── ResourceAllocation
 │ │ ├── HeatMapsForResouce.ipynb
 │ │ ├── InteractiveMaps.ipynb
 │ │ ├── Map for Predicted Counts.ipynb
 ├── Data/
 │ ├── incident_cleaned_final.csv 
 │ ├── incident_cleaned_geocoded_v3.csv 
 │ ├── incident_cleaned_final.csv 
 │ ├── Per Station per Month/<station_name>_monthly.csv
 │ ├── Historical_Forecasted_Independent_Feat/<station_name>_past_future.csv
 │ ├── forecasted_indep_feat_validation_metrics/<station_name>_fc_val.csv 
 │ ├── Predicted Monthly Incident Counts/<station_name>_historical_forecasted_values.csv
 │ ├── RFD_Station_Locations.cpg
 │ ├── RFD_Station_Locations.dbf
 │ ├── RFD_Station_Locations.prj
 │ ├── RFD_Station_Locations.sbn
 │ ├── RFD_Station_Locations.sbx
 │ ├── RFD_Station_Locations.shp
 │ ├── RFD_Station_Locations.shp.xml
 │ ├── tl_2024_us_zcta520.cpg
 │ ├── tl_2024_us_zcta520.dbf
 │ ├── tl_2024_us_zcta520.prj
 │ ├── tl_2024_us_zcta520.shp
 │ ├── tl_2024_us_zcta520.shp.ea.iso.xml
 │ ├── tl_2024_us_zcta520.shp.iso.xml
 │ ├── tl_2024_us_zcta520.shx
 ├── Final Presentation/
 │ ├── Final Presentation.pdf
 │ ├── Final Presentation.pptx
 ├── Readme/
 │ ├── README
 ├── Report/
 ├── Report.pdf
 ├── RFD_InteractiveMaps
 │ ├── Map1_Average_Response_Time_and_Incident_Analysis_by_ZIP_2019-2024.html
 │ ├── Map2_Incident_Type_Distribution_and_Fire_Station_Workload_2019-2024.html
 │ ├── map_predictedCounts_2025
 │ ├── map_predictedCounts_2033
 ├── RFD_FinalPresentationForStakeholders
 │ ├── Presentation For Stakeholders.pdf
 │ ├── Presentation For Stakeholders.pptx

![image](https://github.com/user-attachments/assets/2f16bbbb-452d-4580-a7c2-d9d7e94d552e)
