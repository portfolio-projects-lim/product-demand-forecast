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

- Python Data Processing: Pandas, NumPy

- Time Series Baseline Forecast Models

- Machine Learning: sklearn, xgboost, prophet

- Visualization: Tableau, Matplotlib, Seaborn

- UI: tkinter, HTML

📌 Steps:

1️⃣ **Data Cleaning & EDA**

  - Load dataset

  - Clean + Aggregate

  - EDA & Initial visualization

    Product Demand Overview (2011 - 2016): Warehouse & Product Insights, Return Behavior.

    Summary published as INSIGHT.md in this project.
  
    [View EDA Initial Insight](https://github.com/portfolio-projects-lim/product-demand-forecast/commit/234c881b088d9c5888603c4557e44a7e628cb415)

    Tableau dashboard published (Overview & Initial Insights):

    [View Tableau Visualization - Warehouse, Product Insights, Return Behavior](https://public.tableau.com/views/ProductDemandForecast_17570459518060/Dashboard1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

2️⃣ **Train/test data split (Time-based)**

  - Train: 2011 - 2015

  - Test: 2016

3️⃣ **Baseline Models**
  
  - Naive Forecast, Moving Average, Holt-Winters Models Forecast

4️⃣ **Machine Learning Models**

  - Prophet, XGBoost
  
  - Feature engineering (lags + rollings)

  - Time series Cross-Validation & hyperparameter tuning

  - Retain best config on 2011 - 2015, forecast 2016

5️⃣ **Models Evaluation**

  - Calculate MAE, RMSE, MAPE, WMAPE for each model

  - Export to excel file (.csv)
  
  - Error Metrics Comparison published on Tableau:

    Initial High Errors Metric:
    [View Models Evaluation](https://public.tableau.com/views/ModelsEvaluationErrorMetrics/DashboardModelsEvaluation?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

    Optimization: Aggregate sales by Product_Category instead of Product_Code, smoothing outliers by z-score
    [View Improved Models Evaluation](https://public.tableau.com/views/ForecastModelsEvaluation-AfterOptimize/Dashboard1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
    
6️⃣ **Forecast using Best Model and Best Parameters**  

7️⃣ **Visualization**
 
- Application file (.exe) is generated for future forecast

  Forecast_Tools_v3: [Forecast_Tools_v3](https://drive.google.com/file/d/1i9gWT4bvGZju-zlKVRhkULH3FV8zTjPX/view?usp=drive_link)

  Sample input file: [Historical Product Demand.csv](https://drive.google.com/file/d/1iV2PplE7Pxa5b3BE8UFsXz0RfkAvJaLK/view?usp=drive_link)

  Sample forecast output files:
  [Product Demand Forecast Plots and HTML](https://drive.google.com/drive/folders/1gfbdDwhMgUggCn2y_3sg2VCVmV4zW4J-?usp=drive_link)
  [Product Demand Forecast excel](https://drive.google.com/drive/folders/1WC_IeXzIroL2-CPr_eNis_bAI9fedi2R?usp=drive_link)

  (1) User Input: Forecast Range (number of forecast months), browse save path and file name
  
  (2) User Input: Select Product Demand History excel file (which contains - columns: Product_Code, Warehouse, Product_Category, Date, Order_Demand)

  (3) Output: Generated forecast plots, excel files, html plots

  
📌 Further Improvement 
.
.
.
.
.

