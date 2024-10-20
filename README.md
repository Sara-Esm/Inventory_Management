# **Intelligent Inventory Management for Retail - Walmart Sales Forecasting**

## **Overview**
This project focuses on building a machine learning model to predict **retail sales** for Walmart stores, enabling **intelligent inventory management**. By forecasting sales, we can optimize stock levels, reducing overstock and stockouts, thus improving the efficiency of inventory operations.

## **Problem Statement**
The primary objective is to predict **Weekly Sales** for different Walmart stores. Accurate sales predictions help ensure optimal inventory levels, improve supply chain operations, and minimize costs related to under- or over-stocking.

## **Data Source**
The dataset used in this project is from **Walmart Store Sales Forecasting**, which includes historical data such as:
- Store ID
- Department ID
- Weekly Sales
- Date
- Store Type
- Holiday Information

## **Project Workflow**

### **1. Data Loading and Preprocessing**
- **Data Loading**: The dataset is loaded and explored for insights.
- **Missing Data Handling**: Missing values in numeric features are filled with the mean, and missing values in categorical features are filled with the mode.
- **Feature Inspection**: Key features are analyzed for consistency and relevance.

### **2. Feature Engineering**
- **Date Features**: The `Date` column is transformed into `Year`, `Month`, and `Day` features for better time-based analysis.
- **One-Hot Encoding**: Categorical features like `StoreType` are converted into numerical values using one-hot encoding.
  
### **3. Modeling**
- **Train-Test Split**: The data is split into training (80%) and testing (20%) sets.
- **Model Selection**: A **Random Forest Regressor** is used to predict sales based on the engineered features.
- **Hyperparameter Tuning**: Fine-tuning of model parameters to improve performance.

### **4. Evaluation**
- **Root Mean Squared Error (RMSE)**: A metric used to measure prediction error.
- **R-Squared (R²)**: A metric that explains the variance in the predicted values.
- **Feature Importance**: Identifying which features are most influential in predicting sales.

### **5. Model Saving**
- The trained model is saved using `joblib` for future use and deployment.

## **Key Features**
- **Random Forest Model**: Utilizes an ensemble learning method for regression tasks.
- **Feature Engineering**: Transforming and optimizing data for better predictive performance.
- **Feature Importance**: Understanding key factors driving sales predictions through model interpretability.

## **Results**
- **RMSE on test set**: 21786.298600351474
- **R-Squared**: -0.3413115964648241
- **Feature Importance Plot**: A visual representation of the most important features driving the predictions.

## **Future Improvements**
- **Hyperparameter Optimization**: Further tuning to improve model performance.
- **Additional Features**: Include data like holidays, promotions, and external economic factors to enhance predictions.
- **Model Deployment**: Deploy the model in a cloud environment (AWS, GCP) for real-time sales predictions.
- **API Development**: Create an API for serving real-time predictions to inventory management systems.

## **Conclusion**
This project demonstrates how machine learning can be applied to forecast retail sales, offering insights into how intelligent inventory management can reduce inefficiencies and optimize operations.

