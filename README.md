# Inventory Management and Demand Forecasting Dashboard

## Problem Statement
Large retail enterprises face significant challenges in managing inventory levels, often resulting in substantial financial losses due to both understocking and overstocking. Understocking can lead to missed sales opportunities and diminished customer satisfaction, while overstocking incurs high holding costs and potential waste of unsold goods. The National Retail Federation reports that stockouts and overstocks can result in financial losses of approximately $1.75 trillion annually for retailers. This issue stems from inaccurate demand forecasting and a failure to predict demand at the category level, impacting customer experience and profitability.

## Solution Overview
To address these challenges, we developed a comprehensive dashboard designed for real-time inventory monitoring and precise demand forecasting. Our solution enables business holders to:

- **Monitor Inventory**: Provides up-to-date visibility into inventory levels and sales performance across various stores and departments.
- **Forecast Demand**: Utilizes a machine learning model to predict weekly sales at a category level, incorporating historical sales data, holidays, seasonal variations, store-specific factors (e.g., size and type), and economic indicators (e.g., unemployment, CPI).
- **Analyze and Optimize**: Offers insights on top-performing stores and departments, identifies potential stock surpluses or deficits, and supports informed decision-making.

By providing a clear view of current stock and accurate demand predictions, our dashboard helps retailers allocate funds efficiently, improve inventory management, and enhance overall profitability.

## Tech Stack
- **Tableau**: Used for creating an interactive dashboard that enables real-time inventory monitoring and demand forecasting with advanced data visualization and integration capabilities.
- **SQL Database**: Manages data storage, including weekly sales and current stock levels, ensuring robust and scalable data handling with real-time updates.
- **Python & Jupyter Notebook**: Employed for developing the Elastic Net regression model for demand forecasting. Python’s libraries support accurate model training, while Jupyter Notebook offers an interactive development environment.

## Implementation Details
### Data Handling and Feature Engineering
- **Data Collection & Preprocessing**: Utilized an anonymized dataset from Kaggle with historical sales data from 45 stores, preprocessed and stored in a SQL database.
- **Feature Engineering**: Extracted features such as historical sales, store attributes, and economic indicators to enhance model performance.

### ML Model Building
- Developed an Elastic Net regression model using Python and Jupyter Notebook, combining Lasso and Ridge techniques. The chosen model achieved a Testing R² of 0.6522 and an MAE (Mean Absolute Error) of 8034.855.

### Integration with Tableau
- Integrated the ML model with Python scripts via TabPy to enable real-time predictions within Tableau.

### Dashboard Interaction
- User-selected parameters in Tableau interact with the SQL database to fetch and display real-time data, with dynamic updates for current stock levels and sales forecasts.

## Results and Impact
- **Informed Decision-Making**: Provides predictive insights and real-time data for better inventory management, staff allocation, and planning.
- **Improved Accuracy**: Helps avoid understocking and overstocking, reducing financial losses.
- **Increased Efficiency**: Enhances operations with dynamic updates, leading to greater efficiency and improved customer satisfaction.

## Development Challenges and Resolutions
- **Model Accuracy**: The initial model had limited accuracy. Addressed through iterative tuning and evaluation, selecting the model with the best performance metrics.
- **Forecasting Granularity**: Initially limited to category-level forecasting. Future plans include expanding to granular, product-level forecasting and integrating advanced ML techniques for enhanced accuracy.



