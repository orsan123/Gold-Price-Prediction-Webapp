

# Gold Price Prediction Web Application

## Summary

A **machine learning-powered web application** that predicts gold prices one year into the future using Facebook Prophet, **achieving 97% R² accuracy**. After comprehensive model comparison, **Prophet** was selected for its optimal balance of performance and deployment efficiency, with USDX integrated as a key regressor based on its strong inverse correlation with gold prices.





## Project Objectives

- Develop an accurate gold price prediction model using historical data from 1979-2025
- Conduct extensive model comparison (XGBoost, Random Forest, LSTM, Prophet)
- Identify and integrate the most influential economic indicators as regressors
- Create an intuitive web interface for real-time gold price forecasts
- Demonstrate full-stack data science capabilities from research to production


## About the Dataset

- **Sources:** Yahoo Finance, World Gold Council, Kaggle
- **Time Period:** 1979 - 2025
- **Records:** 11,700+ daily price observations
- **Key Features:** Date, Gold Price (USD), USDX (US Dollar Index)
- **Additional Indicators Considered:** Crude oil prices, S&P 500, NASDAQ, Dow Jones, interest rates
- **Data Quality:** Minimal cleaning required (formatting standardization, basic missing value handling)
## Data Transformation and Modeling

- **Aggregated** and **standardized** financial data from multiple reputable sources
- Conducted **feature importance** analysis using Random Forest, identifying USDX as the most significant regressor
- Performed comprehensive model comparison including **XGBoost, Random Forest, LSTM,** and **Facebook Prophet**
- Selected Facebook Prophet for final implementation due to superior **time series** handling and lightweight deployment
- Integrated USDX as an **external regressor**, leveraging Prophet's native support for additional variables
- Achieved **97% R² score** on validation data
- Generated **one-year future forecasts** with confidence intervals


## Key Insights

- **Model Performance:** Achieved exceptional **97% R² score** using **Facebook Prophet**, outperforming other models in time series forecasting
- **Feature Significance:** **USDX** emerged as the strongest predictor through Random Forest feature importance analysis, confirming its well-documented inverse relationship with gold
- **Research-Driven Approach**: Model selection and feature engineering informed by financial market research and empirical analysis
- **Practical Deployment:** Prophet's simplicity and lightweight characteristics proved ideal for web integration without sacrificing accuracy
## Technologies


**Python | Facebook Prophet | Flask | XGBoost | Random Forest | LSTM | Pandas | NumPy | Scikit-learn | Matplotlib | Seaborn | HTML5 | CSS3 | Jupyter Notebook**
## Tools Used

- **Machine Learning:** Facebook Prophet, XGBoost, Random Forest, LSTM, Scikit-learn
- **Data Processing:** Pandas, NumPy for data aggregation and manipulation
- **Visualization:** Matplotlib, Seaborn for exploratory analysis and model comparison
- **Backend:** Python Flask framework for web server development
- **Frontend:** HTML5, CSS3 for responsive and aesthetic user interface
- **Development:** Jupyter Notebook for model prototyping, VS Code for web development


## Key Skills Demonstrated

- **Data Cleaning:** Handling duplicates, standardizing data, and addressing null values
- **Business Analysis:** Translating data patterns into actionable business strategies
- **Data-Driven Decision Making:** Identifying what actually works versus what sounds good
- **Visual Communication:** Creating charts that clearly show which promotions perform best


## Structure

```
Gold-Price-Prediction/
├── app.py
├── README.md
├── .vscode/
│   └── extensions.json
├── data/
│   ├── processed/
│   │   └── forecast.csv
│   └── raw/
│       └── gold_and_usdx.csv
├── docs/
│   └── Gold_price_prediction_report.pdf
├── model/
│   └── prophet_model.pkl
├── notebooks/
│   └── gold_price_prediction.ipynb
├── static/
│   ├── about.css
│   ├── forecast.css
│   ├── index.css
│   ├── login.css
│   └── style.css
└── templates/
    ├── about.html
    ├── forecast.html
    ├── home.html
    ├── index.html
    └── login.html

```
## Project Documentation

For detailed technical analysis, methodology, and academic context, please refer to the complete project report:

[**📑 Gold Price Prediction - Comprehensive Project Report**](docs/Gold_price_prediction_report.pdf)

- Full academic methodology and literature review
- Detailed exploratory data analysis
- Comprehensive model comparison results
- Architecture diagrams and system design
- Future work and research directions
## How to Run This Application

**Prerequisites**

- Python 3.7+
- pip (Python package manager)

**Installation Steps**

- **Clone the repository**

        git clone https://github.com/orsan123/Gold-Price-Prediction-Webapp.git
        cd Gold-Price-Prediction-Webapp

- **Install required dependencies**

        pip install -r requirements.txt

- **Run the Flask application**

        python app.py


- Access the web application
- Open your web browser and navigate to http://localhost:5000
- The application will load with the gold price prediction interface


## Conclusion

This project demonstrates a comprehensive approach to financial forecasting, combining rigorous data analysis with practical deployment considerations. The research-driven selection of USDX as a regressor and Facebook Prophet as the modeling framework resulted in a highly accurate prediction system. The seamless web integration makes sophisticated gold price forecasts accessible through an elegant interface, showcasing the ability to transform complex data science into user-friendly applications.


