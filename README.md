# Analysis and Visualization of Solitary Household Death Risk Data in Seoul ⚠️

Using public data provided by the Seoul Data Hub, this project analyzes and visualizes the status of single-person households and the risk of solitary deaths by district in Seoul.
Through data analysis and visualization, the project analyzes single-person households and welfare facilities by district in Seoul with the goal of making policy proposals.
</br>
  
  
## 🚀 Project Objectives

*   Visualize the distribution of single-person households and welfare facilities by district in Seoul on a map.
*   Identify correlations among various variables to explore factors affecting the number of single-person households.
*   Group districts with similar characteristics of single-person households through clustering analysis and derive the characteristics of each group.
</br>
  
  
## 📊 Data Used

|No.|Dataset Name|Source|
|:--:|:--:|--|
|1|Households by Number of Members in Seoul – Eup/Myeon/Dong (years ending in 0 or 5), Si/Gun/Gu (other years)|[Link](https://data.seoul.go.kr/dataList/10996/S/2/datasetView.do)|
|2|Rate of Long-Term Hospitalization Experience among Registered Members of Mental Health Welfare Centers (by district)|[Link](https://data.seoul.go.kr/dataList/OA-20334/A/1/datasetView.do?utm_source=chatgpt.com)|
|3|List of Social Welfare Facilities (Senior Leisure Welfare Facilities) in Seoul|[Link](https://data.seoul.go.kr/dataList/OA-20412/S/1/datasetView.do?utm_source=chatgpt.com)|
|4|Number of Mental Health Promotion Institutions by Institution Type (by district)|[Link](https://data.seoul.go.kr/dataList/OA-20328/S/1/datasetView.do?utm_source=chatgpt.com)|
|5|2021 Study on the Status of Solitary Death Risk in Seoul|[Link](http://kodocsi.or.kr/)|
|6|Seoul_District_Boundary_2017.geojson|[Link](https://github.com/datainworld/administrative_district/blob/master/3_%EC%84%9C%EC%9A%B8%EC%8B%9C_%EC%9E%90%EC%B9%98%EA%B5%AC/%EC%84%9C%EC%9A%B8_%EC%9E%90%EC%B9%98%EA%B5%AC_%EA%B2%BD%EA%B3%84_2017.geojson)|
</br>
  
  
## 🔬 Analysis Details

This project consists of three Jupyter Notebook files, and the analysis contents of each file are as follows.

1.  **Map Visualization (`Seoul Data Hub Visualization_Map Visualization.ipynb`)**
    *   Combines GeoJSON files with single-person household data to display the number of single-person households by district on a Seoul map using a choropleth map.
    *   This allows intuitive identification of areas with high concentrations of single-person households.

2.  **Scatter Plot and Correlation Analysis (`Seoul Data Hub Visualization_Scatter Plot and Correlation.ipynb`)**
    *   Visualizes relationships among various variables, such as the number of single-person households by age group and total population, using scatter plot matrices (pair plots).
    *   Analyzes the strength of relationships between variables using correlation heatmaps.

3.  **Clustering and Visualization (`Seoul Data Hub Visualization_Clustering and Visualization.ipynb`)**
    *   Uses clustering algorithms (K-Means, K-Medoids, DBSCAN, Hierarchical) to cluster districts with similar characteristics related to single-person households into several groups.
    *   Analyzes the characteristics of each cluster (group) and visualizes clustering results on a map to examine spatial distributions by group.
</br>
  
  
## 📁 Folder Structure

```
Data Analysis and Visualization Outputs/
├── data/
│   ├── Seoul_District_Boundary_2017.geojson         # Seoul district boundary map data
│   ├── Seoul_District_AgeGroup_SingleHouseholds.csv # Single-person household data by district and age group
│   └── Final_Dataset.csv                            # Final processed dataset for analysis
├── Seoul Data Hub Visualization_Map Visualization.ipynb
├── Seoul Data Hub Visualization_Scatter Plot and Correlation.ipynb
└── Seoul Data Hub Visualization_Clustering and Visualization.ipynb
```
</br>
