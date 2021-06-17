# masterThesis

This GitHub repository is made as a part of the marter thesis for the degree of Master of Transportation and Logistics at the Technical University of Denmark (DTU). The thesis was prepared at the Section of Transport, DTU Management department of Technology, Management and Economics. The work was carried out between the Janurary 2021 and June 2021, under the supervision of Professor Francisco Camera Pereira (DTU) and Postdoc Inon Peled (DTU).

The repository contains all notebooks and datafiles used to construct the results presented in the thesis. As the work have been an iterative process over 20+ weeks the final naming conventions may differ from file and notebook names. Therefore a brief explanation of every file and notebook is showed below.

- `data` - folder containing all datafiles used throughout the thesis.
  - `Electric_Vehicle_Charging_Station_Energy_Consumption.csv` - Original raw data from Boulder.
  - `Electric_Vehicle_Charging_Station_Energy_Consumption_cleand_covid.csv` - Original raw data cleaned.
  - `poi_map` - POI map interests
  - `idle_times.pickle` - Idle times constructed from the plug-in times.
  - `under_utilization_combinedStations.pkl` - Idle times with original features.
  - `under_utilization_combinedStations_laggedV5.pkl` - Idle times with original and activity features.
  - `ut_poiV6.pkl` - Idle times with original, activity and spatial features.
  - `ut_V6_classification-4H.pkl` - Idle times with original, activity and spatial features as well as column specifying the classification prediction.
 
- `data_construction` - folder containing notebooks used to download, filter and construct the data used through out the thesis.
  - `Boulder_data_clean-up.ipynb` - cleaning of raw plug-in data
  - `Boulder_data_idle_times.ipynb` - construction of idle-times.
  - `Boulder_data_set_construction.ipynb` - merging of original features with idle times.
  - `FeatureConstruction.ipynb` - construction of activity features.
  - `POI.ipynb` - construction of spatial features

- `dataExploration`- folder containing notebooks used to contruct plots for the "Dataset for Case Study", "Data selection", "Feature construction and exploration" section.
  - `inactivity_level_station.ipynb` - brief exploration of the inactivity level of station.
  - `kaplan_meier_plots.ipynb` - construction of different kaplan-meier plots.
  - `map_plotting.ipynb` - construction of the maps visualized in the thesis.
  - `plots_dataExploration_1.ipynb` - quantile TOD & DOW plots as well as horizontal bar plots.
  - `plots_dataExploration_2.ipynb` - histograms of idle-time and plug-in time and area plot.

- `results` - folder containing notebooks used to construct results and plot for the "Modeling strategy" and "Experiments and results" sections
  - 


- `visualizations` - folder containing all visualizations used in the thesis.
