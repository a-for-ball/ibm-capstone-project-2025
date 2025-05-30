# 🚀 SpaceX Launch Analysis & Prediction Dashboard

This project explores SpaceX Falcon 9 launch data to analyze trends, geographical insights, and build predictive models for launch success. It combines exploratory data analysis, interactive visualization using Dash, and classification modeling with scikit-learn.

---

## 🧭 Methodology Summary

1. **Data Cleaning & Preparation**
   - Merged multiple launch datasets
   - Created derived columns for success, orbit type, booster category, and geospatial markers

2. **Exploratory Analysis**
   - Used `folium` to visualize launch site locations and success distribution
   - Examined proximities to coastline, highways, and railways

3. **Interactive Dashboard**
   - Built with `Dash` and `Plotly`
   - Dropdowns and sliders allow filtering by site and payload range
   - Pie chart and scatter plot show success metrics and payload-outcome trends

4. **Predictive Modeling**
   - Trained Logistic Regression, SVM, Decision Tree, and KNN classifiers
   - Evaluated using test accuracy and cross-validation
   - Visualized confusion matrix for best-performing model

---

## 📊 Summary of Results

- **Geographic Insights**
  - All launch sites are near the coastline and clustered near the equator
  - CCAFS LC-40 is closest to a highway and railway

- **Dashboard Findings**
  - KSC LC-39A has the highest success ratio (76.9%)
  - Launches with medium payloads tend to succeed more often
  - Certain booster versions correlate strongly with success

- **Classification Results**
  - Logistic Regression and SVM achieved highest test accuracy (83%)
  - Cross-validation showed consistent performance (~80%)
  - Logistic Regression showed very few false negatives in its confusion matrix

- **Key Orbit Observations**
  - LEO success increases with launch frequency
  - No clear pattern found for success vs. flight count in GTO

---

## 🔍 Key Questions Answered

**Q1: Can we predict the price of a SpaceX launch using publicly available data?**  
Yes — to a reasonable extent. Factors like payload mass, orbit type, and launch site can serve as proxies for estimating launch costs. While exact pricing isn’t public, patterns in these variables enable approximate modeling.

**Q2: Can we accurately predict whether a Falcon 9 first stage will land successfully?**  
Yes. Classification models using historical data reached up to **83% accuracy** on test sets. Logistic Regression performed particularly well with minimal false negatives.

---

## 📷 Sample Visuals

- Interactive pie and scatter charts from Dash
- Folium maps showing launch outcomes by location
- Confusion matrix visualization for classification performance

---

## 🛠️ Tools & Libraries

- Python 3, pandas, numpy
- scikit-learn, matplotlib, seaborn
- Dash & Plotly
- Folium for map visualizations

---

## 📌 How to Run Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/a-for-ball/ibm-capstone-project-2025/tree/mai
   cd spacex-launch-analysis
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Dash app:
   ```bash
   python spacex_launch_dash.py
   ```

---

## 📄 License

This project is for educational and research purposes only. Not affiliated with SpaceX.
