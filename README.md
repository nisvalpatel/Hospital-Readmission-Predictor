# **Predicting Hospital Readmissions Using Machine Learning**  

## **Overview**  
This project analyzes **100,000+ patient records** from the **UCI Diabetes 130-US Hospitals dataset (1999–2008)** to predict hospital readmissions. The objective was to identify key factors contributing to readmissions and develop a robust predictive model. The project involved extensive **data preprocessing, feature engineering, machine learning model development, and performance evaluation**.  

Using **Decision Tree, Random Forest, and Logistic Regression models**, I achieved **78% recall and 72% precision** in predicting readmissions. Feature engineering techniques, including aggregating visit history and categorizing diagnoses, improved model performance and interpretability.  

## **Objectives**  
- Conduct **exploratory data analysis (EDA)** to identify trends in hospital readmissions.  
- Engineer and select **meaningful features** to improve model performance.  
- Train and evaluate **machine learning models** to predict readmissions.  
- Optimize models using **hyperparameter tuning and cross-validation**.  
- Interpret model outputs and extract actionable insights.  

## **Dataset**  
📌 **Source**: [UCI Machine Learning Repository – Diabetes 130-US Hospitals](https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008)  
📌 **Size**: 100,000+ patient records with over 50 features  
📌 **Key Features**:  
- **Demographics**: Race, age, gender  
- **Hospital Visit Information**: Admission type, discharge reason, length of stay, number of previous visits  
- **Medical Information**: Primary diagnosis (ICD-9 codes), lab test results, prescribed medications  
- **Feature Engineering**: Aggregated outpatient, emergency, and inpatient visits into **total_visits**; consolidated individual medications into **treatments_taken**  

## **Approach**  
### **1️⃣ Data Preprocessing & Feature Engineering**  
- Cleaned and standardized data, handling missing values and categorical encoding.  
- Engineered new features to capture **visit history, diagnosis categories, and medication use patterns**.  
- Removed **low-importance features** based on Random Forest feature selection.  

### **2️⃣ Model Development & Optimization**  
- Implemented **Decision Tree, Random Forest, and Logistic Regression** models using Scikit-Learn.  
- Applied **cross-validation and hyperparameter tuning** to enhance model generalization.  
- Optimized recall and precision, balancing sensitivity in identifying high-risk patients.  

### **3️⃣ Results & Insights**  
- **Achieved 78% recall and 72% precision**, prioritizing recall to reduce false negatives.  
- Identified **length of stay, total visits, and medication changes** as top predictors of readmission.  
- Feature engineering improved model performance, increasing accuracy by **10%**.  
- The study highlights the importance of **visit history and medication adherence** in predicting readmissions.  

## **Technologies Used**  
- **Programming**: Python (Pandas, NumPy, Scikit-Learn)  
- **Machine Learning**: Decision Tree, Random Forest, Logistic Regression  
- **Data Visualization**: Matplotlib, Seaborn  
- **Feature Engineering**: Aggregation, categorical encoding, statistical analysis  

## **How to Run the Project**  
### **1️⃣ Install Dependencies**  
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```
### **2️⃣ Clone the Repository**  
```bash
git clone https://github.com/yourusername/hospital-readmission-prediction.git
cd hospital-readmission-prediction
```
### **3️⃣ Run the Jupyter Notebook or Python Script**  
```bash
jupyter notebook
# OR
python train_model.py
```
