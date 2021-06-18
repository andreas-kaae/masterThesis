# masterThesis

This GitHub repository is made as a part of the master thesis for the degree of Master of Transportation and Logistics at the Technical University of Denmark (DTU). The thesis was prepared at the Section of Transport, DTU Management department of Technology, Management and Economics. The work was carried out between January 2021 and June 2021, under the supervision of Professor Francisco Camera Pereira (DTU) and Postdoc Inon Peled (DTU).

The repository contains all notebooks and data files used to construct the results presented in the thesis. As the work has been an iterative process for over 20+ weeks, the final naming conventions may differ between files and notebooks. Therefore a brief explanation of every file and notebook is showed below.

- `data` - folder containing all data files used throughout the thesis.
  - `Electric_Vehicle_Charging_Station_Energy_Consumption.csv` - Original raw data from Boulder.
  - `Electric_Vehicle_Charging_Station_Energy_Consumption_cleand_covid.csv` - Original raw data cleaned.
  - `poi_map` - POI map interests
  - `idle_times.pickle` - Idle times constructed from the plug-in times. OBS The file exceeds the size limit of GitHub. If the file is needed, reach out to me, and I will find a way to send it to you. 
  - `under_utilization_combinedStations.pkl` - Idle times with original features.
  - `under_utilization_combinedStations_laggedV5.pkl` - Idle times with original and activity features.
  - `ut_poiV6.pkl` - Idle times with original, activity, and spatial features.
  - `ut_V6_classification-4H.pkl` - Idle times with original, activity, and spatial features as well as a column specifying the classification prediction.
 
- `data_construction` - folder containing notebooks used to download, filter and construct the data used throughout the thesis.
  - `Boulder_data_clean-up.ipynb` - cleaning of raw plug-in data
  - `Boulder_data_idle_times.ipynb` - construction of idle-times.
  - `Boulder_data_set_construction.ipynb` - merging of original features with idle times.
  - `FeatureConstruction.ipynb` - construction of activity features.
  - `POI.ipynb` - construction of spatial features

- `dataExploration`- folder containing notebooks used to construct plots for the "Dataset for Case Study", "Data selection", "Feature construction and exploration" section. The notebook for the tilted loss function is also included here.
  - `inactivity_level_station.ipynb` - brief exploration of the inactivity level of station.
  - `kaplan_meier_plots.ipynb` - construction of different kaplan-meier plots.
  - `map_plotting.ipynb` - construction of the maps visualized in the thesis.
  - `plots_dataExploration_1.ipynb` - quantile TOD & DOW plots as well as horizontal bar plots.
  - `plots_dataExploration_2.ipynb` - histograms of idle-time and plug-in time and area plot.
  - `tiltedLoss.ipynb` - construction of tilted loss visualization
  - `traditional_reg_singleStep_8station.ipynb` - results for the traditional regression methods for the single-step approach with 8 station. 

- `results` - folder containing notebooks used to construct results and plot for the "Modeling strategy" and "Experiments and results" sections
  - `adding_a_nonexistent_station.ipynb` - results of fitting a nonexistent station to the models.
  - `analysis_of_particular_event.ipynb` - results of specific events.
  - `classifier.ipynb` - results of classifier used for the two-step approach.
  - `CPH_singelStep.ipynb` - results of the single-step approach for the CPH method.
  - `CPH_twoStep.ipynb` - results of the two-step approach for the CPH methods.
  - `CPH_visualization_singleStep.ipynb` - visualization of the CPH single-step approach for the TOD
  - `CPH_visualization_twoStep.ipynb` - visualization for the CPH two-step approach.
  - `DeepSurv_singleStep.ipynb` - results of the DeepSurv single-step approach.
  - `DeepSurv_twoStep.ipynb` - results of the DeepSurv two-step approach.
  - `modeling_with_another_existing_station.ipynb` - results from testing the models with a different station then the ones used for training.
  - `QR_GB_singleStep.ipynb` - results of the gradient boosting quantile regression for the single-step approach. A TOD visualization is also constructed here.
  - `QR_GB_twoStep.ipynb` - results of the gradient boosting quantile regression for the two-step approach.
  - `QR_LR_singleStep.ipynb` - results of the linear quantile regression for the single-step approach. 
  - `QR_LR_twoStep.ipynb` - results of the linear quantile regression for the two-step approach. 
  - `traditional_reg_perfectCLF.ipynb` - results of the perfect classifier for the traditional regression methods.
  - `traditional_reg_singleStage_modelSelection.ipynb` - results for the traditional regression methods for the single-step approach. Both the Baseline, Activity, Spatial and Full models are trained and tested.
  - `traditional_reg_twoStep.ipynb` - results for the traditional regression methods for the two-step approach.


- `visualizations` - folder containing visualizations constructed by the notebooks described above and used in the thesis.
