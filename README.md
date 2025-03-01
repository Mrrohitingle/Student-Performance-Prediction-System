# Student Academic Performance Prediction System

## 📌 Overview
Managing and predicting student performance is crucial for enhancing academic outcomes in educational institutions. This project introduces a **Student Performance Prediction Management System (SPPMS)** that leverages data mining and machine learning techniques to forecast student performance. The system integrates various data sources, including **academic records, demographic information, and extracurricular activities**, to build comprehensive student profiles.

## 📑 Project Lifecycle
1. **Understanding the Problem Statement**
2. **Data Collection & Warehousing**
3. **Data Preprocessing & Integration**
4. **Exploratory Data Analysis (EDA)**
5. **Feature Engineering**
6. **Predictive Model Training & Evaluation**
7. **Selecting the Best Model for Deployment**

## 📊 Dataset
- **Source:** [Kaggle - Student Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977)
- **Size:** 1000 rows × 8 columns
- **Features:**
  - `gender` (Male/Female)
  - `race_ethnicity` (Group A-E)
  - `parental_level_of_education` (Education level)
  - `lunch` (Standard/Free-reduced)
  - `test_preparation_course` (Completed/None)
  - `math_score` (Target Variable)
  - `reading_score`, `writing_score`

## 🛠 Required Libraries & Dependencies
```sh
pip install numpy pandas matplotlib seaborn scikit-learn catboost xgboost
```

## 📥 Data Preprocessing
- **Data Cleaning:** Handling missing values and duplicates (None found in the dataset).
- **Feature Engineering:** One-hot encoding categorical variables and scaling numerical data.
- **Data Warehousing:** Integrated various sources of student data into a centralized system.

## 🤖 Predictive Modelling
### **Algorithms Used:**
1. **Linear Regression**
2. **Lasso Regression**
3. **Ridge Regression**
4. **K-Neighbors Regressor**
5. **Decision Tree Regressor**
6. **Random Forest Regressor**
7. **XGBRegressor**
8. **CatBoost Regressor**
9. **AdaBoost Regressor**

### **Model Performance (R² Score on Test Data)**
| Model | R² Score |
|--------|----------|
| Ridge | **0.8806** |
| Linear Regression | **0.8803** |
| AdaBoost Regressor | 0.8519 |
| CatBoost Regressor | 0.8516 |
| Random Forest Regressor | 0.8509 |
| XGBRegressor | 0.8278 |
| Lasso | 0.8253 |
| K-Neighbors Regressor | 0.7838 |
| Decision Tree | 0.7414 |

## 📈 Best Model Selection
- **Ridge Regression** achieved the highest R² score of **88.06%**.
- Linear Regression followed closely with **88.03%**.
- Ridge Regression was selected as the final model for prediction.

## 📊 Visualization & Insights
- **Demographic & Performance Analysis:**
  - Female students performed better overall, but males had higher math scores.
  - Students from Groups A & B had lower scores compared to Groups D & E.
- **Influencing Factors:**
  - Students with **standard lunch** performed significantly better.
  - **Test preparation course completion** improved student scores.

## 🚀 Installation & Usage
```sh
# Clone the repository
git clone https://github.com/your-username/Student-Performance-Indicator.git
cd Student-Performance-Indicator

# Install dependencies
pip install -r requirements.txt

# Run the model
python train_model.py
```

## 🔥 Results & Predictions
- The final model's **predictions vs actual values** were visualized using scatter plots and regression plots.
- **Error Metrics:**
  - **MAE:** 4.21
  - **RMSE:** 5.39
  - **R² Score:** 88.06%

## 📜 Research Paper
For a detailed explanation of the methodology and results, refer to the research paper: [Student Performance Prediction Research Paper](https://drive.google.com/file/d/1Rz9M1vqcSuHBFKhh5Hyc44opzDOOqPIK/view?usp=sharing)


## 🤝 Contributing
Pull requests are welcome! If you'd like to improve the project, open an issue to discuss your ideas.

## 📧 Contact
For inquiries, reach out at: [your-rohitngle2912@gmail.com](mailto:rohitingle2912@gmail.com)


