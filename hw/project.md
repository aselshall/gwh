# [Term Project: Groundwater Supply Design](https://aselshall.github.io/gwh/hw/project)

*Modified from Finkel, M. (2008), Environmental Modelling 1 Lecture Notes, University of Tuebingen, Tuebingen.*

## 1. Data
### 1.1 Hydrogeological Settings
The investigated aquifer is situated within the alluvial complex of a river catchment. The sediments consist of sandy silts and locally of old buried river channels. The aquifer is unconfined throughout the catchment and lays on top of an aquitard (elevation of aquifer base: 90 m above sea level). Fig. 1 depicts the situation. The head in the river (width = 40 m) can be assumed to be constantly hriv = 100 m in along the area of interest.  A groundwater flow model shall be set up in order to support the planning of different facilities (water supply well, industrial area, landfill).

<img width="488" height="433" alt="image" src="https://github.com/user-attachments/assets/e079c870-2efe-4d09-889b-eb5c1847fe05" />
 
Fig. 1 Plan view and cross section of the area of investigation. (Remark: isolines are only schematically correct!)
	
### 1.2 Model Setup
The model shall span an area of 4500 m x 1500 m as is indicated in Fig. 1. The suggested spatial gridding is Δx = Δy = 50 m. The aquifer can be represented by a single model layer.

### 1.3 Recharge
The recharge rate of 0.8 mm/day in the model domain can be assumed constant. 

### 1.4 River 
The elevation of the riverbed bottom is 95 m. Thickness of riverbed sediments is 20 cm and the conductivity of riverbed sediments is 0.02 m/day.

### 1.5 Electrical Resistivity Profiling 
Geophysical survey as shown in Fig. 2 is available. 

<img width="834" height="482" alt="image" src="https://github.com/user-attachments/assets/de60e4c3-298d-48ec-894e-75275c88a75f" />

Fig. 2 Results of electrical resistivity profiling showing resistivity values in ohm-meter [Ω.m].

The resistivity logs give qualitative hints where sandy material and gravel can be expected. Based on our understanding the geology of the area, buried river sediments are expected to be present in the subsurface. In general, river sediments are often composed of coarser and more permeable materials such as sand and gravel, which can have higher hydraulic conductivity than finer-grained materials such as clay and silt. These river sediments can act as a preferential flow pathway for groundwater. Resistivity logs can be used to identify buried river sediments by analyzing the variations in resistivity values.  Variations in resistivity values can be used to identify boundaries between different types of sediments. Identifying areas with lower resistivity values and sudden changes in resistivity values could be indicative of buried river sediments. When an electrical current is applied to the subsurface through electrodes and the resulting voltage is measured, the resistivity of the subsurface materials can be determined. Resistivity [Ω.m], which is a fundamental specific property of a material, is a measure the electrical resistance of the material. In general, sandy and gravelly materials have higher electric resistivity than finer-grained materials such as clay and silt that have charged particles that conducts electricity. Thus, if resistivity logs indicate higher resistivity values in certain areas, it may suggest the presence of sandy or gravelly materials with higher hydraulic conductivity values.

### 1.6 Hydraulic Head Measurements
12 observation wells have been drilled. Table 1 shows the locations and head measurements. 
Tab. 1 Observation wells and head measurements 

| Observation Well | X (m) | Y (m) | Head Measurements (m) |
|------------------|-------|-------|------------------------|
| B1               | 450   | 1250  | 107.98                 |
| B2               | 1650  | 1050  | 105.93                 |
| B3               | 750   | 250   | 107.42                 |
| B4               | 1950  | 550   | 105.59                 |
| B5               | 2550  | 650   | 104.36                 |
| B6               | 2850  | 250   | 103.96                 |
| B7               | 4050  | 150   | 101.39                 |
| B8               | 3450  | 750   | 102.66                 |
| B9               | 3450  | 1350  | 102.72                 |
| B10              | 3450  | 950   | 102.60                 |
| B11              | 3150  | 850   | 103.18                 |
| B12              | 2850  | 1150  | 103.70                 |


### 1.7 Pumping Test 
Results from aquifer tests provide ranges of K values at each observation wells (Table 2). 
Table 2. Pumping test results 
| Well | Low K | High K |
|------|-------|--------|
| B1   | 3     | 12     |
| B2   | 15    | 25     |
| B3   | 18    | 25     |
| B4   | 16    | 21     |
| B5   | 16    | 20     |
| B6   | 38    | 50     |
| B7   | 35    | 47     |
| B8   | 34    | 44     |
| B9   | 39    | 44     |
| B10  | 550   | 750    |
| B11  | 250   | 320    |
|B12	 | 280	 | 370    |

Note that no aquifer test could be made in vicinity to the river due to missing wells in this area. However, it can be assumed that highly permeable river sediments can be found along the river and beside it up to a distance of approximately 200 to 300 m.

## 2. Design Problem

### 2.1 Model Setup  (120 points)
Setup groundwater flow model in a steady-state. Follow the suggestions concerning the spatial extension and gridding that are made above. Remark: Make sure that the elevation of the top of the layer is large enough to guarantee unconfined conditions (i.e. the simulated hydraulic heads should not exceed the model’s top elevation 

### 2.2 Model Calibration (20 points) 
Calibrate the groundwater flow model such that the heads simulated at the 12 observation wells do not deviate from the measured head values more than 0.3 m. Remark: As all model parameters except the hydraulic conductivity K are given, the task is to find the appropriate spatial K distribution. First, inspect the given data/information carefully. Then consider possible zonation to start with based on the given data. Once the model is calibrated, you can proceed dealing with the problem described below (30 points)

### 2.3 Model Application (30 points)
Do any of the following two design problems.

#### 2.3.1 Municipal Water Supply Desgin: Nature-based Infrastructure
It is planned to install a municipal water supply well half way between observation well B10 and the river.  Also, a new industrial area is planned in the study area as show in Fig. 3 resulting in a complete sealing of the surface. For each of the following scenarios, what is the maximum rate of water than can be pumped if the drawdown of the water table should not exceed 1 m at any of the observation wells?

- Scenario 1: This is the pre-development condition without the industrial area.
- Scenario 2:  This scenario is the post-development condition with the industrial area. Industrial area is assumed to completely seal the surface, meaning no water recharge occurs below it.
- Scenario 3:  This scenario also represents the post-development condition with the industrial area, but with mitigation measures. Low-impact development (also known as nature-based solutions) are proposed to mitigate the impact of the development. A well-designed permeable pavement system over the industrial area given reasonable soil and climate conditions is estimated to result in 30% recharge relative to the original recharge (i.e., 0.8 mm/day). The remaining water will be collected and infiltrated along the Eastern side of the industrial area using stormwater ponds as shown in Fig.3. This is expected to result in an additional 50% recharge relative to the original recharge in the industrial area (i.e., 0.8 mm/day). In the report clearly state the new recharge values in the industrial area and infiltration area. Also, what recommendation would you give with respect to the location of the infiltration area. You can support your recommendation with a model simulation for bonus points.
 
For each scenario:
- Show the changes in hydraulic head distribution relative to the baseline scenario (i.e., calibrated model without pumping and without the industrial area).
- Express your final estimate of the maximum permissible pumping rate (Q) in million gallons per day (mgd). If this aquifer is in south Florida, estimate how many people this new well can supply with two significant digits. 
	 
<img width="683" height="230" alt="image" src="https://github.com/user-attachments/assets/33b3256e-0fcf-41a6-b047-f63d88d0b6c8" />

Fig. 3 Plan view of the model domain including the location of observation wells (B1 to B10), and the location of the planned industrial area.

Discuss your results given the information provided in [Elshall et al. 2020](https://iopscience.iop.org/article/10.1088/1748-9326/ab8e8c). 

#### 2.3.2 Municipal Water Supply Desgin: Capture Zone Delineation

It is planned to install a water supply well half way between observation well B10 and the river.
- What is the maximum rate of water than can be pumped if the drawdown of the water table should not exceed 50 cm at any of the observation wells
- Show the changes in hydraulic head distribution.
- Demarcate the capture zone of the well at this pumping rate with particle pathlines (“backward tracking”).

## 3. Modeling report (20 points)

### 3.1 Objective
Prepare a modeling report to document your model and results.  The report is the primary grading basis. Model files can be optionally submitted but are not required. Therefore, ensure the report includes all comprehensive information on model setup, calibration, and problem-solving. Describe and discuss all data; avoid figures and tables without context; aim for publication-quality visuals. 

### 3.2 Outline

Here’s a polished and more professional version of your outline and figures section. I’ve streamlined the language, improved consistency, and emphasized clarity while keeping it concise and actionable.

### 3.2 Report Outline

Suggested Structure and Content
1. Title
2. Abstract
3. Introduction
   * Provide background and objectives of the study.
   * Present the groundwater flow equation with explanations of terms and relevance to your work.
4. Hydrological Setting and Conceptual Model
   * Summarize available data and information (e.g., hydrogeology, recharge, pumping, boundary conditions).
   * Present the conceptual model developed from the data, including key assumptions and simplifications.
5. Numerical Model
   * Describe the setup of the flow model (domain, discretization, boundaries, initial conditions).
   * Explain the calibration process: objectives, calibration parameters, methods, and evaluation criteria.
   * Present calibration results, including fit to observed data and overall model performance.
6. Model Application
   * Define the problem(s) addressed using the model.
   * Describe modifications made for scenario analysis.
   * Present and discuss results for each scenario.
   * Provide actionable recommendations based on findings.
7. Conclusions and Limitations
   * Summarize key results.
   * Discuss limitations of the model and implications for interpretation.
8. References Cited
   * Use a consistent citation style.
   * Refer to exemplary reports (e.g., Oki, 2005; Swain et al., 2019).

> *Note: While Oki (2005) and Swain et al. (2019) provide detailed examples, your report should remain concise, well-structured, and focused on clear analysis with practical recommendations.*

### 3.3 Required Figures (Minimum)

General
* Diagram of the modeling process (adapted from *Lesson 17 GW Modeling 1: Model Setup* slides).
Model Setup
* Map showing observation wells, proposed pumping well, industrial area, and infiltration area.
* Head contour and hydraulic conductivity field before automatic calibration.
Model Calibration
* Head contour and hydraulic conductivity field after calibration.
* Plot of residuals (observed vs. simulated).
* Scatter plot: simulated vs. observed heads.
* Plot: residuals vs. observed heads.
  * (*See slides from “Model Calibration” for guidance on writing strong discussions of these results.*)

Model Application
* Design Problem 1: Head contour maps for different scenarios.
* Design Problem 1: Head contour map including your pumping well.
* Design Problem 1: Particle tracking figure.

These are the minimum required figures. Include additional figures where needed to better illustrate your design effectiveness and results.


## Reference
- Elshall, A.S., A.D. Arik, A. El-Kadi, S. Pierce, M. Ye, C. A. Wada, K.M. Burnett, ​L.L. Bremer, and G. Chun (2020), Groundwater sustainability : A review of the interactions between science and policy, Environmental Research Letters, 15 , 093004. https://doi.org/10.1088/1748-9326/ab8e8c
- Oki, D. S. (2005). Numerical Simulation of the Effects of Low-Permeability Valley-Fill Barriers and the Redistribution of Ground-Water Withdrawals in the Pearl Harbor Area, Oahu, Hawaii. U.S. Geological Survey, Scientific Investigations Report 2005-5253. Retrieved from https://pubs.usgs.gov/sir/2005/5253/
- Swain, E. D., Lohmann, M. A., & Goodwin, C. R. (2019). The hydrologic system of the south Florida peninsula—Development and application of the Biscayne and Southern Everglades Coastal Transport (BISECT) model (Report No. 2019–5045) (p. 126). Reston, VA. https://doi.org/10.3133/sir20195045

