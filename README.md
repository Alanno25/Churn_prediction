# Project Churn Prediction 

เป็นโปรเจคที่เขียนด้วย Python และใช้โมเดล Machine learning ในเพื่อหาคำตอบว่าปัจจัยใดที่มีผลต่อการเลิกใช้บริการ (Churn) ของผู้ใช้บรืการ เพื่อให้สามารถวางแผนวิธีแก้ไขสำหรับลดปัญหาการเลิกใช้บริการ และดำเนินการเพื่อรักษาลูกค้าไว้ได้

## Project Overview
โปรเจคนี้ใช้ข้อมูลจากเว็บไซต์ kaggle เพื่อใช้ทำการสร้างโมเดลทำนายการ Churn โมเดลนี้ช่วยให้สามารถระบุลูกค้าที่มีความเสี่ยงสูงเพื่อช่วยป้องกันการสูญเสียลูกค้า

## Problem Statement
* ปัญหาการสูญเสียลูกค้า (Customer Churn) ที่ส่งผลกระทบต่อรายได้ของบริษัท
* โปรเจคนี้มุ่งเน้นในการสร้าง Predictive Model เพื่อทำนายลูกค้าที่มีแนวโน้มที่จะยกเลิกบริการในอนาคต


## Methodology (ขั้นตอนในการทำงาน)

### 1. Data Preprocessing
การจัดการข้อมูลโดยการแปลงค่าของหัวข้อที่มีตัวเลือก(categorical) 2 อย่างให้เป็นตัวเลข(numerical) และ ใช้ One Hot Encoding ในการแปลงข้อมูลที่มีตัวเลือกมากกว่า 2 อย่าง


### 2. Exploratory Data Analysis 
วิเคราะห์ข้อมูลเบื้องต้นโดยนำข้อมูลที่แปลงค่าแล้วมาแสดงในรูปแบบต่างๆเพื่อหาความสัมพันธ์ที่เกี่ยวข้องกับปัญหา


### 3. Feature Engineering 
หา Feature ที่มีความสำคัญจากข้อมูลที่มีอยู่โดยการใช้ข้อมูลที่ได้จากการ Exploratory Data Analysis และ เทคนิค Feature Selection เพื่อนำไปสร้างโมเดล Machine Learning


### 4. Model Building
-   **Baseline Model:** เช่น Logistic Regression
    
-   **Advanced Models:** เช่น RandomForest, XGBoost , Gradient Boosting

### 5. Model Evaluation
ประเมินประสิทธิภาพของโมเดลด้วย Metrics ต่างๆเพื่อตัดสินใจในการเลือกโมเดลที่จะนำไปใช้

## Data Source

### Data Set 
```bash
WA_Fn-UseC_-Telco-Customer-Churn.csv
```


### Source

```bash

https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data

```

## **How to Run the Project**


1.  **Clone the repository:**
    ```
    git clone https://github.com/Alanno25/Churn_prediction.git
    
    ```
    
2.  **Install dependencies:**
    ```
    pip install -r requirements.txt
    
    ```
    
3.  **Run the notebook:**
    ```
    jupyter notebook Churn_Prediction_Notebook.ipynb
    
    ```
## **Results & Model Performance**

-   **Best Model:** XGBoost + ADASYN
    
-   **Accuracy:** 74%
    
-   **Precision:** 80%
    
-   **Recall:** 74%
    
-   **F1-Score:** 75%
    
-   **Confusion Matrix:**
```
    precision    recall  f1-score   support

           0       0.90      0.72      0.80      1035
           1       0.50      0.79      0.61       374

    accuracy                           0.74      1409
   macro avg       0.70      0.75      0.71      1409
weighted avg       0.80      0.74      0.75      1409
```

## Contact

-   **ชื่อ:** นาย ศุภณัฐ นฤนาทมนตรี  (Mr. Supanut Narunartmontree)
    
-   **Email:** supanut.narunartmontree@gmail.com
    
-   **LinkedIn:** https://www.linkedin.com/in/supanut-narunartmontree-98122a39b/ /รอแก้