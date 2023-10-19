# Energy Efficiency Enhancement Analysis

##  Background

The world heavily relies on various electrical devices, from small household bulbs to large industrial machines. The efficiency of these devices affects global energy consumption and individual energy bills. This analysis aims to categorize devices based on their power consumption and determine their efficiency, offering insights into better energy usage and potential improvements.

### Research Questions
1. How can electrical devices be categorized based on power consumption?
2. Which devices are the most energy-efficient and which ones need improvements?
3. How can energy providers and manufacturers improve the energy efficiency of these devices?

##  Data

### Description
This dataset offers detailed insights into the energy efficiency of various electrical devices.

- **Data sources:** Acquired from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php), a recognized resource for machine learning researchers and enthusiasts offering datasets for varied domains.
- **Data size:** Approximately 36 KB
- **Data shape:** 
  - **Rows:** 300
  - **Columns:** 4
- **Time period:** The dataset does not specify a distinct time span but offers a snapshot of device efficiencies at a particular point.
- **Each Row Represents:** Efficiency metrics and other pertinent details of an individual electrical device.


### Data Dictionary

| Column Name          | Data Type | Definition                                         | Potential Values   |
|----------------------|-----------|----------------------------------------------------|--------------------|
| device_name          | String    | Name of the electrical device.                     | Bulb, LED TV, etc. |
| min_consumption      | Float     | Minimum power consumption of the device in watts.  | N/A                |
| max_consumption      | Float     | Maximum power consumption of the device in watts.  | N/A                |
| device_age           | Integer   | Age of the device in years.                        | N/A                |
| input_power          | Float     | Synthetically generated input power in watts.      | N/A                |
| working_hours        | Integer   | Synthetically generated working hours of device.   | 0-24               |
| output_power         | Float     | Synthetically generated output power in watts.     | N/A                |
| Enhanced_efficiency  | Float     | Calculated efficiency of the device.               | 0-100%             |
| efficiency           | Float     | Efficiency based on minimum consumption.           | 0-100%             |

##  Exploratory Data Analysis (EDA)

This section involved analyzing the data to understand the distribution of variables, correlations, and patterns. 
### Correlation Heatmap

![Correlation Heatmap](https://github.com/alishaminj12/Energy-Efficiency-Enhancement-Analysis/blob/main/Correlation%20Heatmap.png)

This heatmap gives insights into the relationships between the variables.

### Data Distribution and Relationships

![Clusters of Consumption](https://github.com/alishaminj12/Energy-Efficiency-Enhancement-Analysis/blob/main/Clusters%20of%20Consumption.png)

The above visualization categorizes devices based on their power consumption, providing insights into efficiency patterns.

### Dendrogram Visualization

![Dendrogram](https://github.com/alishaminj12/Energy-Efficiency-Enhancement-Analysis/blob/main/Dendrogram.png)

The dendrogram showcases the hierarchical clustering process, offering an understanding of how different devices relate in terms of efficiency.

##  Model Implementation and Evaluation

Gradient Boosting Regressor was used to predict the 'Enhanced_efficiency' of devices based on their power consumption parameters. 

### Model Performance
- **Mean Squared Error**: 76.88
- **Mean Absolute Error**: 7.33

##  Conclusions

The analysis provided insights into power consumption patterns of different electrical devices. By understanding and categorizing these devices, energy providers and researchers can develop strategies for efficient power consumption.

### Future Recommendations
- Conduct similar analyses on newer models of devices to track efficiency improvements over time.
- Collaborate with manufacturers to understand the potential reasons for inefficiencies and devise solutions.

