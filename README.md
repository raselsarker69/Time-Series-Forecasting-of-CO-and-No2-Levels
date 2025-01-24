# Time-Series Forecasting of Carbon Monoxide (CO) and Nitrogen Dioxide (NO₂)
---

## **Project Overview**
This project focuses on the time-series forecasting of Carbon Monoxide (CO) and Nitrogen Dioxide (NO₂) concentrations to monitor air quality and predict future trends. Using advanced time-series analysis and machine learning models, we aim to:

- Identify seasonal trends and patterns.
- Forecast pollutant levels to enable proactive environmental monitoring.
- Evaluate and optimize models for accurate predictions.

---

## **Dataset Description**
The dataset consists of historical air quality measurements, including:

- **Date** and **Time**: Timestamp of each observation.
- **CO (GT)**: Ground truth concentration of Carbon Monoxide (mg/m³).
- **NO₂ (GT)**: Ground truth concentration of Nitrogen Dioxide (µg/m³).
- **Other Variables**:
  - **Temperature (T)**: Ambient temperature (°C).
  - **Relative Humidity (RH)**: Percentage of relative humidity.
  - **Absolute Humidity (AH)**: Absolute humidity values.

### **Data Preprocessing**
1. **Handling Missing Data**: Interpolation was used to fill missing values.
2. **Normalization**: Variables were scaled using MinMaxScaler.
3. **Correlation Analysis**: Explored relationships between variables to identify key features affecting pollutant levels.
4. **Seasonality Analysis**: Seasonal trends were extracted using decomposition techniques.

---

## **Exploratory Data Analysis (EDA)**
1. **Correlation Matrix**:
   - Positive correlation between **CO** and **NO₂** levels.
   - Significant impact of **Temperature (T)** and **Relative Humidity (RH)** on pollutant concentrations.

2. **Seasonality Insights**:
   - Monthly and daily seasonality patterns identified for both pollutants.
   - Peak NO₂ levels observed during colder months.

---

## **Models Implemented**
The following models were evaluated for forecasting:

1. **SARIMAX** (Seasonal Auto-Regressive Integrated Moving Average with Exogenous Variables):
   - Effective for capturing linear trends and seasonality.

2. **LSTM (Long Short-Term Memory)**:
   - A deep learning model designed for sequential data.
   - Captures long-term dependencies and nonlinear relationships.

3. **Baseline Models**:
   - Naive forecasting for comparison.

---

## **Model Performance**

| **Pollutant**  | **Model** | **MAE**   | **RMSE**  | **R²**   |
|----------------|-----------|-----------|-----------|-----------|
| **CO (GT)**    | SARIMAX   | 0.06      | 0.08      | 0.76      |
|                | LSTM      | 0.05      | 0.07      | 0.82      |
| **NO₂ (GT)** | SARIMAX   | 0.12      | 0.18      | 0.15      |
|                | LSTM      | 0.10      | 0.16      | 0.28      |

### **Findings**
- **SARIMAX** is effective for interpretable and seasonal patterns but struggles with nonlinear relationships.
- **LSTM** outperforms SARIMAX for CO forecasting with better generalization to complex patterns.

---

## **Key Insights**
1. **CO Levels**:
   - Strong correlation with temperature.
   - LSTM achieved the highest accuracy for predicting CO levels.

2. **NO₂ Levels**:
   - Seasonal trends dominate NO₂ levels.
   - Both SARIMAX and LSTM require further tuning to improve performance.

3. **Feature Importance**:
   - Temperature (T) and Humidity (RH) significantly impact pollutant concentrations.

---

## **Visualization**
1. **Correlation Heatmap**:
   - Visualized relationships between pollutants and meteorological variables.

2. **Seasonality Analysis**:
   - Plots showed monthly and daily pollutant variations.

3. **Model Predictions**:
   - Comparison of actual vs. predicted values demonstrated LSTM’s superiority for CO.

---

## **How to Run the Project**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo-name/time-series-air-quality.git
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Preprocess the Data**:
   - Run `data_preprocessing.py` to clean and prepare the data.

4. **Train Models**:
   - Use `train_model.py` to train SARIMAX and LSTM models.

5. **Generate Forecasts**:
   - Run `forecast.py` to predict future pollutant levels.

6. **Visualize Results**:
   - Use `visualizations.py` to generate plots for analysis.

---


## **Future Work**
1. **Hyperparameter Optimization**:
   - Tune SARIMAX and LSTM parameters for better performance.

2. **Advanced Models**:
   - Explore transformer-based architectures for time-series forecasting.

3. **Deployment**:
   - Develop a web-based dashboard for real-time air quality monitoring.

---


## Contributing

Contributions are welcome! If you have ideas to improve this repository or want to add more projects, please feel free to:

1. Fork the repository.
2. Make your changes.
3. Submit a pull request.

---

## License
This repository is licensed under the MIT License. Feel free to use and modify the code as needed.

---

## Author
**Md. Rasel Sarker**  
Email: [rasel.sarker6933@gmail.com](mailto:rasel.sarker6933@gmail.com)  

<br>
<h1 align="left">
 <h2><img src = "https://media2.giphy.com/media/QssGEmpkyEOhBCb7e1/giphy.gif?cid=ecf05e47a0n3gi1bfqntqmob8g9aid1oyj2wr3ds3mg700bl&rid=giphy.gif" width=30px valign="bottom"> 🌐 Connect with Me:</h2>
</h1>

<p align="center">
  <a href="mailto:rasel.sarker6933@gmail.com"><img src="https://img.shields.io/badge/Email-rasel.sarker6933@gmail.com-blue?style=flat-square&logo=gmail"></a>
  <a href="https://github.com/raselsarker69"><img src="https://img.shields.io/badge/GitHub-%40Raselsarker-lightgrey?style=flat-square&logo=github"></a>
  <a href="https://www.linkedin.com/in/rasel-sarker-405160227/"><img src="https://img.shields.io/badge/LinkedIn-Rasel%20Sarker-blue?style=flat-square&logo=linkedin"></a>
  <a href="https://www.facebook.com/mdrasel.sarker.7773631"><img src="https://img.shields.io/badge/Facebook-%40Raselsarker-blue?style=flat-square&logo=facebook"></a>
  <a href="https://www.kaggle.com/mdraselsarker"><img src="https://img.shields.io/badge/Kaggle-%40Raselsarker-blue?style=flat-square&logo=kaggle"></a>
  <a href="https://www.youtube.com/@raselsarker69"><img src="https://img.shields.io/badge/YouTube-Rasel%20Sarker-red?style=flat-square&logo=youtube"></a>
  <a href="https://www.facebook.com/groups/832585175685301"><img src="https://img.shields.io/badge/Facebook%20Group-Rasel%20Sarker%20Group-blue?style=flat-square&logo=facebook"></a>
  <br>
  <img src="https://img.shields.io/badge/Phone-%2B8801581528651-green?style=flat-square&logo=whatsapp">
</p>
 

---

<div align="center">

Thank you for visiting my repository. I hope these projects inspire and guide your learning journey!

---

Feel free to explore, learn, and build upon these projects. Happy coding!<br>

&copy; 2025 Machine Learning Projects

</div>
