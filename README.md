# Supermarket Sustainability Advanced Analytics: Machine Learning for Profitability & Product Quality

## Executive Summary

Sustainable retailers must balance profitability, product quality, and customer satisfaction while making data-driven decisions across their operations. Using Python and machine learning, I analyzed sales transactions and product quality data from a sustainability-focused supermarket chain to identify opportunities for improving business performance and operational efficiency.

The project combines regression, classification, clustering, and forecasting techniques to address multiple business challenges, including profitability prediction, product quality assessment, customer satisfaction analysis, and revenue forecasting.

The results show that simpler models can often outperform more complex alternatives, product quality can be classified with high accuracy, and customer and inventory decisions can benefit from segmentation techniques that reveal hidden patterns in the data.

### Key Business Impact

* Analyzed 1,000 retail transactions and 4,000 product quality records
* Built and compared multiple machine learning models across four business use cases
* Identified the most effective model for product quality classification (F1-score > 0.80)
* Discovered hidden product segments through clustering analysis
* Generated recommendations for inventory management, supplier evaluation, and forecasting improvements

---

## Business Problem

A sustainability-focused supermarket chain needs to improve decision-making across several areas of the business.

Management wants to better understand:

* Which factors influence transaction performance and customer satisfaction
* How product quality can be automatically evaluated and monitored
* Whether products naturally group into different quality tiers
* How future revenue trends can be forecasted more effectively
* Which analytical models provide the most reliable business insights

The objective of this project was to leverage machine learning techniques to transform transactional and product quality data into actionable recommendations that support retail growth and operational efficiency.

---

## Methodology

### Data Preparation

* Cleaned and prepared supermarket sales data and apple quality data
* Performed exploratory data analysis and statistical profiling
* Applied feature engineering, encoding, and scaling where required

### Machine Learning Analysis

#### Profitability Prediction

* Linear Regression
* Polynomial Regression

#### Product Quality Classification

* Logistic Regression
* Decision Tree

#### Product Segmentation

* K-Means Clustering (2 clusters)
* K-Means Clustering (3 clusters)

#### Revenue Forecasting

* Time Series Linear Regression

### Model Evaluation

Models were evaluated using:

* MSE and MAE for regression
* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

---

## Skills

**Python:** Pandas, NumPy, Scikit-Learn, SciPy

**Machine Learning:** Regression Analysis, Classification Models, Decision Trees, Clustering, Forecasting, Model Evaluation

**Data Analysis:** Exploratory Data Analysis (EDA), Feature Engineering, Statistical Analysis, Customer & Product Segmentation

**Data Visualization:** Matplotlib, Seaborn

---

## Results & Business Recommendations

The analysis produced several actionable insights for retail operations and product management.

### Profitability Prediction

* Linear Regression outperformed Polynomial Regression, producing lower prediction errors and demonstrating that additional model complexity did not improve performance.
* Gross income distribution showed positive skewness, indicating that a relatively small number of transactions generate a disproportionate share of revenue.

### Product Quality Classification

* Decision Tree was the strongest classification model, achieving F1-scores above 0.80.
* Logistic Regression provided a useful baseline but generated more classification errors.
* Product quality can be reliably predicted using physical and chemical product characteristics.

### Product Segmentation

* K-Means clustering with three clusters revealed an intermediate quality segment not captured by traditional good/bad classifications.
* This additional segment creates opportunities for more nuanced product categorization and inventory management.

### Revenue Forecasting

* Linear regression showed limited forecasting performance on transactional time-series data.
* Results suggest that seasonality and non-linear patterns require more advanced forecasting approaches.

### Business Recommendations

Based on the findings, I would recommend:

* Implementing Decision Tree models as part of product quality monitoring processes.
* Introducing a three-tier quality classification system to better differentiate products and suppliers.
* Using quality clusters to optimize inventory allocation and pricing strategies.
* Monitoring high-revenue transaction patterns to better understand customer purchasing behavior.
* Evaluating supplier performance using quality prediction models and cluster assignments.
* Investing in more advanced forecasting solutions to improve demand planning and revenue projections.

These initiatives would improve operational visibility, support better inventory decisions, and help the supermarket maintain high product quality standards while driving sustainable growth.

---

## Next Steps

* Create supplier scorecards using quality predictions and cluster assignments.
* Expand the analysis to additional product categories beyond apples.
* Develop a recommendation framework for inventory optimization and quality control.


---

## Datasets
- [**Supermarket Sales Dataset**](https://drive.google.com/file/d/1rW6Av8bbWu1Lyo8SKjiaSRUMoHoWNK7F/view)— 1,000 transactional records including branch, city, customer type, gender, product line, payment method, unit price, gross income, and satisfaction rating.
- [**Apple Quality Dataset**](https://drive.google.com/file/d/1XnzAlIa8R9D_doy0ebSo1qf319Pg6mbf/view) — 4,000 records with physical and chemical apple features (Size, Weight, Sweetness, Crunchiness, Juiciness, Ripeness, Acidity) and a binary quality label (Good/Bad).

---

## Files in this Repository
| File | Description |
|------|--------------|
| `Advanced_Analytics_Project.ipynb` | Full Python notebook: EDA, preprocessing, all ML models, and time series analysis. |
| `README.md` | Project overview, methodology, insights, and model comparison. |
