# **Wildfire Prediction using AWS SageMaker & XGBoost**

## **Overview**
This project leverages **AWS SageMaker** and **XGBoost** to predict wildfire occurrences based on historical data. The model is trained to estimate future fire locations with high accuracy, achieving an **R² score of 0.85**. The pipeline automates data ingestion, preprocessing, training, and deployment using **AWS S3, Lambda, and SageMaker**, allowing real-time predictions via a REST API.

## **Tech Stack**
- **Machine Learning Algorithm:** XGBoost  
- **Cloud Services:** AWS SageMaker, AWS Lambda, AWS S3  
- **Deployment:** SageMaker Endpoint (REST API)  

## **Project Architecture**
1. **Data Storage:** Fire incident data is stored in an **AWS S3 bucket**.
2. **Preprocessing & Training:** A **Lambda function** triggers data preprocessing and model training on **SageMaker**.
3. **Model Deployment:** The trained XGBoost model is deployed as a **SageMaker Endpoint**.
4. **Real-time Predictions:** The API endpoint allows users to send input features and receive wildfire risk predictions with minimal latency.

## **Installation & Setup**
### **Prerequisites**
- AWS Account with access to **S3, SageMaker, and Lambda**
- Python 3.x
- AWS CLI configured with required permissions
- `boto3` and `sagemaker` Python SDKs

### **Step 1: Clone the Repository**
```bash
git clone https://github.com/your-repo/wildfire-prediction.git
cd wildfire-prediction
