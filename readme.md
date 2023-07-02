# Water Stress Predictions

As almost 17 countries in the world are facing high levels of water stress, it is really important to understand the basic factors that cause this water stress in the areas and how these simple factors relate to water stress. In this project, we have leveraged machine learning models to gain insights into this issue.

## Introduction

Water stress is a pressing global issue affecting numerous countries. This project aims to explore the factors contributing to water stress and predict its levels using machine learning techniques. By understanding the underlying causes and patterns of water stress, we can develop effective strategies for water resource management and mitigate its impact.

## Data Source

The primary data source for this project is the [Food and Agriculture Organisation of the United Nations (FAO) Aquastat](https://www.fao.org/aquastat/statistics/query/index.html). Aquastat provides comprehensive water-related data on various aspects of water and irrigation for countries around the world. The data covers a wide range of variables that can impact water security.

## Supervised Learning

In the supervised learning part of our project, we focused on establishing a relationship between various factors and water stress values. We collected data from the FAO Aquastat database, selecting relevant features that could impact water security. The selected features were then extracted along with the corresponding water stress values for all countries.

To ensure data quality, we performed preprocessing steps, including handling missing values. Variables with significant missing data were dropped from the analysis. We also removed observations with missing water stress values, as water stress served as the predictor variable.

Given the absence of direct linear correlations between the variables and water stress, we employed a Neural Network model built using TensorFlow. The data was scaled using the min-max method, and the model was trained on an 80% training set. The performance of the model was evaluated on a separate 20% test set. Furthermore, we extrapolated the values of the variables for 2022 using linear regression to predict water stress for that year.

## Unsupervised Learning

In the unsupervised learning section of our project, we aimed to analyze the behavior of cities in terms of water stress using unsupervised machine learning techniques. We utilized the Urban Environment Social Inclusion Index (UESI) Data, which provides valuable information on urban environmental issues.

The UESI data includes indicators related to water stress, such as water resource management and wastewater treatment. We leveraged unsupervised learning techniques, particularly clustering analysis, to identify similarities between cities and explore the patterns of water stress in different clusters.

To prepare the data, we performed data cleaning by eliminating variables with a high percentage of missing values. Principal Component Analysis (PCA) was then applied to condense the information of the index variables into a few representative components. This aided visualization and analysis.

K-means clustering and spectral clustering were employed to group cities based on their water stress characteristics. Spectral clustering yielded satisfying results with 9 clusters, enabling us to identify groups of cities with similar water stress behaviors. This information was utilized to build visualizations for the Water Security application, allowing users to explore similarities between cities and assess water stress distribution within clusters.

## Future Work

This project serves as a starting point for further research and exploration of water stress predictions and urban environmental issues. Some potential avenues for future work include:

- Incorporating additional data sources and indicators to enhance the models' predictive capabilities and gain a deeper understanding of water stress dynamics in urban areas.
- Expanding the clustering analysis to identify more refined clusters and uncover more nuanced patterns in water stress behavior among cities.
- Integrating the findings of this project into the Water Security application to provide real-time updates and recommendations for water stress mitigation strategies in different cities.
- Collaborating with domain experts, city managers, and policymakers to ensure the practical application of the project's findings in urban planning and decision-making processes.

## References

[1] "Food and Agriculture Organisation of the United Nations" - [Website](https://www.fao.org/home/en/)

[2] Urban Environment Social Inclusion Index (UESI) Data

The link for the app is https://watersecurityapp.herokuapp.com/
