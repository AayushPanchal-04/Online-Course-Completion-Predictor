# 🎓 Online Course Completion Predictor

An AI-powered machine learning application that predicts whether a student will complete an online course (MOOC) based on their engagement metrics, demographics, and learning behavior patterns.


## 🎯 Overview

This project addresses the critical challenge of student dropout rates in online learning platforms. By analyzing various engagement metrics and demographic factors, the model predicts course completion probability and provides actionable recommendations to improve student retention.

### Problem Statement

Online courses face high dropout rates (often 85-90%). Early identification of at-risk students enables timely interventions to improve completion rates.

### Solution

A Random Forest machine learning model that:
- Predicts completion probability with 85-90% accuracy
- Identifies key factors influencing course completion
- Provides personalized recommendations for struggling students
- Enables batch prediction for entire cohorts

## ✨ Features

### 🔮 Prediction Capabilities
- **Single Student Prediction**: Interactive form for individual predictions
- **Batch Prediction**: Upload CSV files for cohort-level analysis
- **Real-time Results**: Instant predictions with probability scores
- **Visual Analytics**: Interactive gauges and charts

### 📊 Analysis Features
- Comprehensive exploratory data analysis
- Feature importance visualization
- Model performance comparison
- ROC curve analysis
- Correlation heatmaps

### 💡 Intelligent Recommendations
- Personalized suggestions based on engagement gaps
- Specific action items for improvement
- Risk factor identification
- Success pattern recognition

### 🎨 User Interface
- Clean, professional Streamlit interface
- Interactive visualizations using Plotly
- Responsive design
- Easy-to-use navigation

## 🛠️ Tech Stack

**Machine Learning:**
- scikit-learn (Random Forest, Logistic Regression, Gradient Boosting)
- pandas & NumPy for data manipulation
- Model persistence with pickle

**Visualization:**
- Matplotlib & Seaborn for static plots
- Plotly for interactive visualizations
- Streamlit for web interface

**Development:**
- Jupyter Notebook for experimentation
- Python 3.8+


## 🚀 Usage

### Single Prediction

1. Navigate to the **Prediction** tab
2. Enter student demographics (age, gender, education)
3. Input engagement metrics (videos watched, assignments, etc.)
4. Click **Predict Completion**
5. View results, probability gauge, and recommendations

### Batch Prediction

1. Navigate to the **Batch Prediction** tab
2. Download the sample CSV template
3. Fill in student data following the template format
4. Upload your CSV file
5. Click **Predict All**
6. Download results with predictions

### Model Training

Open `course_completion_analysis.ipynb` in Jupyter to:
- Explore the dataset
- Perform feature engineering
- Train and compare multiple models
- Evaluate model performance
- Save the best model

## 📁 Project Structure

```
online-course-predictor/
│
├── course_completion_analysis.ipynb  # ML model development
├── course.py                            # Streamlit web application
├── README.md                         # Project documentation
│
│   course_data.csv              # Training dataset
│
├
│   course_completion_model.pkl  # Trained model
│
└── screenshots/                      # Application screenshots
    ├── prediction.png
    ├── batch.png
    └── dashboard.png
```

## 📊 Model Performance

### Performance Metrics

| Model | Accuracy | ROC-AUC | Precision | Recall |
|-------|----------|---------|-----------|--------|
| Random Forest | 89.2% | 0.94 | 0.87 | 0.91 |
| Gradient Boosting | 87.5% | 0.92 | 0.85 | 0.89 |
| Logistic Regression | 84.1% | 0.88 | 0.82 | 0.86 |

### Top Features (by importance)

1. **Assignments Completed** (23.5%)
2. **Quiz Scores Average** (18.2%)
3. **Days Active** (15.8%)
4. **Videos Watched** (13.4%)
5. **Time Spent Hours** (11.3%)

## 📊 Dataset

### Features Used

**Demographics:**
- Age
- Gender
- Education Level
- Previous Courses Completed

**Engagement Metrics:**
- Videos Watched
- Assignments Completed
- Forum Posts
- Login Frequency
- Days Active

**Performance Indicators:**
- Average Quiz Scores
- Total Time Spent
- Certification Goal

**Engineered Features:**
- Engagement Rate
- Assignment Completion Rate
- Average Time per Day
- Interaction Score

### Data Sources

This project uses a synthetic dataset for demonstration. For real-world applications, you can use:

- [Kaggle MOOC Datasets](https://www.kaggle.com/search?q=mooc)
- [Open University Learning Analytics](https://analyse.kmi.open.ac.uk/open_dataset)
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets.php)

