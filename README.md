# 🌍 World Countries GDP Data Analysis

This project analyzes the GDP per capita of 227 countries using a publicly available dataset. The objective is to identify the key economic and social factors influencing GDP and build predictive models using various machine learning techniques.

## 📁 Project Structure

- `World Countries GDP Data Analysis.pdf` — Final formatted project report
- `GDP_Analysis_Notebook.ipynb` — Jupyter Notebook with all data analysis, modeling, and visualizations
- `README.md` — Project overview and instructions

## 📊 Objective

The primary goal is to analyze and predict GDP per capita using features such as:

- Region, population, area
- Birthrate, deathrate, net migration
- Infant mortality, literacy, phone usage
- Economic sectors (agriculture, industry, service)

## 🛠️ Steps Performed

1. **Data Cleaning**:

   - Renamed long columns for clarity
   - Converted incorrect data types
   - Imputed missing values with region-wise mean or reasonable estimates

2. **EDA & Visual Insights**:

   - Heatmaps for missing data
   - Correlation analysis
   - Regional breakdown of economic indicators
   - Country-level scatter plots and hexbin plots

3. **Feature Engineering**:

   - Created a new column: `Total_GDP = gdp_per_capita * population`
   - Transformed categorical 'region' using one-hot encoding
   - Selected key features based on correlation

4. **Modeling**:
   Four machine learning models were used:

   - **Linear Regression**
   - **K-Nearest Neighbors (KNN)**
   - **Decision Tree Regressor**
   - **Random Forest Regressor**

   Each model was tested with:

   - All features (with/without scaling)
   - Selected features (with/without scaling)

## 🧠 Model Highlights

| Model                 | Accuracy (MAE) | Precision (RMSE) | R² Score |
| --------------------- | -------------- | ---------------- | -------- |
| **Linear Regression** | 2328.85        | 2745.24          | 0.91     |
| **KNN (k=5)**         | 2519.57        | 3513.03          | 0.85     |
| **Decision Tree**     | 223.91         | 438.13           | 0.998    |
| **Random Forest**     | 200.56         | 464.14           | 0.997    |

📌 **Insight**: The Decision Tree and Random Forest models provided the best performance. Feature selection played a vital role, while scaling was helpful but not mandatory for tree-based models.

## 📈 Visualizations

The notebook contains 11+ visualizations including:

- Heatmaps
- Pair plots
- Hex plots
- GDP comparisons
- Regional distributions
- Stacked bar charts of economic sectors

## 📌 Key Findings

- **Strong correlation**: Literacy, infant mortality, phone access, and service sector contribute significantly to GDP per capita.
- **Migration & GDP**: Higher net migration is generally associated with higher GDP.
- **Total vs Per Capita GDP**: Countries like India and China rank higher in total GDP due to population, but not in per capita GDP.

## 🧾 Conclusion

This project demonstrates how combining data cleaning, EDA, feature engineering, and multiple ML models can provide a robust understanding of global economic indicators. The Random Forest Regressor with selected features stood out as the most effective model for predicting GDP per capita.

---

## 📎 Author

**Mohan Krishna Vallabhaneni**  
Bachelors of Computer Science at George Mason University
📧 [vmkrishna2022@gmail.com](mailto:vmkrishna2022@gmail.com)
