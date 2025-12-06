# IBM Data Science Capstone Project  
## SpaceX Falcon 9 Landing Success Prediction

## Project Objective
The objective of this project was to analyze SpaceX Falcon 9 launch data and identify factors that influence first-stage landing success.  
Using machine learning, the goal was to predict whether a Falcon 9 booster would successfully land.

---

## Methodology (Step-by-Step)

### 1. Data Collection
- Collected launch data using the SpaceX REST API.  
  **Notebook:** [M1_api data collection.ipynb](https://github.com/Rajnish-28/IBM_capstone_project/blob/main/M1_%20api%20data%20collection.ipynb)
- Scraped Falcon 9 launch tables from Wikipedia using BeautifulSoup.  
  **Notebook:** [M1_data collection api with web scraping.ipynb](https://github.com/Rajnish-28/IBM_capstone_project/blob/main/M1_data%20collection%20api%20with%20web%20scraping.ipynb)
- Combined API and scraped data into a unified dataset.

### 2. Data Wrangling
- Filled missing values (e.g., payload mass).  
- Converted landing outcomes into numerical labels (0 = Fail, 1 = Success).  
- Cleaned and standardized the dataset.  
  **Notebook:** [M1_data wrangling.ipynb](https://github.com/Rajnish-28/IBM_capstone_project/blob/main/M1_%20data%20wrangling.ipynb)

### 3. Exploratory Data Analysis (EDA)
- Visualized important patterns, such as:
  - Flight number vs landing success  
  - Payload vs landing outcome  
  - Orbit type vs success rate  
  - Year-wise success trends  
- Performed SQL-based filtering, grouping, and ranking.  
  **Notebook (Visual EDA):** [M2 EDA with data visualization.ipynb](https://github.com/Rajnish-28/IBM_capstone_project/blob/main/M2%20EDA%20with%20data%20visualization.ipynb)
  **Notebook (SQL EDA):** [M2_EDA with SQL.ipynb](https://github.com/Rajnish-28/IBM_capstone_project/blob/main/M2_EDA%20with%20SQL.ipynb)

### 4. Interactive Visual Analytics
- Built an interactive Folium map showing launch sites and outcomes.  
  **Notebook:** [M3_Interactive Visual Analytics with Folium lab.ipynb](https://github.com/Rajnish-28/IBM_capstone_project/blob/main/M3_Interactive%20Visual%20Analytics%20with%20Folium%20lab.ipynb)
- Developed a Plotly Dash dashboard with:
  - Launch site dropdown  
  - Payload range slider  
  - Success vs failure charts  
  - Payload vs outcome scatter plot  
  **Dashboard App:** [M3_spacex-dash-app.py](https://github.com/Rajnish-28/IBM_capstone_project/blob/main/M3_spacex-dash-app.py)

### 5. Predictive Modeling
- Trained four ML models:
  - Logistic Regression  
  - SVM  
  - KNN  
  - Decision Tree  
- Tuned models using GridSearchCV.  
- Compared accuracy and selected the best model (Logistic Regression).  
  **Notebook:** [M4_predictive analysis.ipynb](https://github.com/Rajnish-28/IBM_capstone_project/blob/main/M4_predictive%20analysis.ipynb)

---

## Key Results
- Landing success depends on:
  - Flight number  
  - Payload mass  
  - Orbit type  
  - Launch site  
- Success rate increased significantly from 2010 to 2020.  
- KSC LC-39A had the highest landing success rate.  
- All ML models achieved ~83% test accuracy.  
- Logistic Regression performed the most consistently.

---

## What I Learned
- Using APIs and web scraping to collect real-world datasets.  
- Data cleaning and feature engineering techniques.  
- Performing EDA using Python plots and SQL queries.  
- Creating interactive dashboards using Plotly Dash and Folium.  
- Training, tuning, and evaluating machine learning models.  
- Understanding the complete end-to-end data science pipeline.

---

## ✔️ Project Status
Completed as part of the **IBM Data Science Professional Certificate – Capstone Project**.
