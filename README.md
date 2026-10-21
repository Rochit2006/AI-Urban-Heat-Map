# AI Urban Heat Map – Pune

## 1. Project Overview
AI Urban Heat Map is an Artificial Intelligence and Machine Learning (AIML) project that analyzes urban heat patterns in Pune using satellite-derived environmental data. It uses Google Earth Engine to study Land Surface Temperature (LST) and environmental indices to understand how vegetation, built-up areas, and water features relate to urban heat.

The project applies Linear Regression and Random Forest Regression to estimate land surface temperature and classifies locations into different heat-risk categories.

## 2. Objectives
- Analyze land surface temperature in Pune.
- Study the relationship between temperature and environmental indices.
- Use machine learning to predict land surface temperature.
- Classify areas into Low, Medium, and High heat-risk levels.
- Demonstrate how AI and satellite data can support urban planning.

## 3. Technologies Used
- Python
- Google Earth Engine
- Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Git and GitHub

## 4. Environmental Parameters
- **LST (Land Surface Temperature):** Measures the temperature of the land surface.
- **NDVI (Normalized Difference Vegetation Index):** Indicates vegetation presence and density.
- **NDBI (Normalized Difference Built-up Index):** Helps identify built-up areas.
- **NDWI (Normalized Difference Water Index):** Helps identify water-related features.

## 5. Machine Learning Algorithms

### Linear Regression
Linear Regression models the relationship between environmental features and land surface temperature. It provides a simple baseline for temperature prediction.

### Random Forest Regression
Random Forest combines multiple decision trees to predict land surface temperature. It can model more complex relationships between environmental variables and temperature.

### Heat-Risk Classification
Predicted or analyzed temperature values are grouped into Low, Medium, and High heat-risk categories according to the project's defined thresholds.

## 6. Study Area
The study area is Pune, Maharashtra, India. Google Earth Engine is used to process satellite-derived information for the selected geographic region.

## 7. Workflow
1. Select the study area in Google Earth Engine.
2. Obtain and process satellite-derived data.
3. Calculate LST and environmental indices.
4. Prepare the dataset for machine learning.
5. Clean the data and select relevant features.
6. Train Linear Regression and Random Forest models.
7. Evaluate model performance.
8. Visualize temperature patterns and heat-risk categories.

## 8. Results
The project compares Linear Regression and Random Forest Regression using the coefficient of determination (R²).

The current experimental results recorded during development were:
- Linear Regression R²: 0.4724
- Random Forest Regression R²: 0.5138

The Random Forest model performed better than Linear Regression in this experiment. These values should be verified against the final notebook before submission.

Recorded feature importance values for the Random Forest model:
- NDBI: 0.506
- NDWI: 0.297
- NDVI: 0.197

The recorded heat-risk distribution was:
- High: 1,699 samples
- Medium: 1,649 samples
- Low: 1,652 samples

These counts describe the analyzed samples, not necessarily the total number of geographic locations in Pune.

## 9. Installation and Setup
Install Python and Git, then clone the repository:

```bash
git clone https://github.com/Rochit2006/AI-Urban-Heat-Map.git
cd AI-Urban-Heat-Map
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

If the project uses Google Earth Engine Python APIs, install the relevant package and configure authentication as required:

```bash
pip install earthengine-api
```

## 10. Running the Project
1. Open the project folder.
2. Start Jupyter Notebook:

```bash
jupyter notebook
```

3. Open the project's `.ipynb` notebook.
4. Run the cells in order.
5. Review the data analysis, model evaluation, and visualizations.

Google Earth Engine authentication and access may be required if the notebook retrieves or processes data directly from Earth Engine.

## 11. Applications
- Urban heat analysis
- Environmental monitoring
- Sustainable city planning
- Identification of potentially heat-prone areas
- Data-driven urban environmental research

## 12. Future Scope
- Develop an interactive heat-map dashboard.
- Use additional satellite dates to analyze seasonal changes.
- Improve model performance with more features and validation.
- Compare heat patterns across different urban areas.
- Integrate the results into a planning-support tool.

## 13. Limitations
Predictions depend on data quality, geographic coverage, selected features, and model assumptions. Land Surface Temperature is not the same as near-surface air temperature. Heat-risk categories are analytical labels and should not be treated as official health warnings.

## 14. Author
**Rochit Kumar Singh**  
B.Tech – Information Technology  
Bharati Vidyapeeth College of Engineering, Pune

## 15. License
Add a license if you intend to permit others to reuse or modify the project. Confirm the licenses and attribution requirements of any external datasets used.
