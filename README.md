# product-demand-forecast
This project uses real-world manufacturing demand data to forecast future product demand with time series and machine learning models.

📦 Product Demand Forecasting

📌 Project Background

In manufacturing and supply chain management, demand forecasting helps companies to:

- Reduce inventory stockouts & overstocking

- Optimize production & inventory planning

- Improve supply chain efficiency & customer satisfaction

📌 Objectives

- Analyze historical data - demand trends and seasonality

- Build multiple forecasting models

- Compare model performance with error metrics

- Visualize actual vs forecasted demand - to support inventory and production decisions

📌 Dataset

- Kaggle: Historical Product Demand.csv

- Dataset from a manufacturing company with footprints globally

- 4 central warehouses to ship products within the region it is responsible for.

- Sample Fields: Product_Code, Warehouse, Product_Category, Date (to receive), Order_Demand (single order quantity)

📌 Skills

- Python: Pandas, NumPy, Matplotlib, Seaborn

- Database: SQLite

- Machine Learning & Time Series Forecast Models

- Visualization: Tableau, Matplotlib, Seaborn

📌 Steps:

1️⃣ **Data Cleaning & EDA**

  - Load dataset

  - Clean + Aggregate

  - Initial EDA

    Product Demand Overview (2011 - 2016): Warehouse & Product Insights, Return Behavior.

    Summary published as INSIGHT.md in this project.
  
    [View Initial EDA Insight](https://github.com/portfolio-projects-lim/product-demand-forecast/commit/234c881b088d9c5888603c4557e44a7e628cb415)

    Tableau dashboard published (Overview & Initial Insights):

    [View Tableau Visualization - Warehouse, Product Insights, Return Behavior](https://public.tableau.com/views/ProductDemandForecast_17570459518060/Dashboard1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

 - Train/test data split

   Train: 2011 - 2015

   Test: 2016

2️⃣ **Baseline Models**
  
  - Naive Forecast, Moving Average, Holt-Winters Models Forecast

3️⃣ **XGBoost Model**

  - Feature engineering (lags + rollings)

  - Time series Cross-Validation & hyperparameter tuning

  - Retain best config on 2011 - 2015

  - Forecast 2016

4️⃣ **Models Evaluation**

  - Calculate MAE, RMSE, MAPE for each model

5️⃣ **Export to CSV**  

  - For analysis and visualization: Model_Evaluation_Results.csv

📌 Visualization

📌 Further Possible Improvement
