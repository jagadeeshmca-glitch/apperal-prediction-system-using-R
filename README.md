# Apparel Productivity Prediction and Analysis

An R-based data analytics and machine learning project for predicting garment worker productivity, analyzing production performance, and identifying factors that influence productivity in apparel manufacturing.

## 📌 Project Overview

The **Apparel Productivity Prediction and Analysis** project uses garment worker productivity data to predict actual productivity and classify whether production teams achieve their targeted productivity.

The project combines data preprocessing, exploratory data analysis, statistical testing, regression modeling, classification, and visualization to support data-driven decision-making in garment manufacturing.

## 🎯 Objectives

- Predict actual productivity for garment production teams.
- Classify whether teams meet their productivity targets.
- Identify the key factors affecting worker productivity.
- Compare multiple regression models using evaluation metrics.
- Generate charts, reports, and prediction outputs.
- Support production planning and productivity improvement.

## 📊 Dataset

**Dataset:** `garments_worker_productivity.csv`

The dataset contains production-related information, including:

- Quarter, department, day, and team
- Targeted productivity
- Standard Minute Value (SMV)
- Work in Progress (WIP)
- Overtime and incentives
- Idle time and idle workers
- Number of style changes
- Number of workers
- Actual productivity

## 🛠️ Technologies Used

**Programming Languages**
- R
- Python 3

**R Libraries**
- `ggplot2` – Data visualization
- `dplyr` and `tidyr` – Data cleaning and transformation
- `caret` – Model training and evaluation
- `ranger` – Random Forest modeling
- `rpart` – Decision Tree modeling
- `glmnet` – Ridge and Lasso Regression
- `corrplot` – Correlation visualization
- `car` and `lmtest` – Statistical analysis

**Python Libraries**
- `python-pptx` – PowerPoint presentation processing
- `Pillow` – Image processing

## ⚙️ Project Workflow

1. Load and validate the dataset.
2. Clean missing values and inconsistent data.
3. Perform exploratory data analysis (EDA).
4. Visualize productivity trends and variable relationships.
5. Conduct statistical tests and data diagnostics.
6. Train multiple regression models.
7. Evaluate models using RMSE, MAE, and R².
8. Train a Logistic Regression classifier for target achievement.
9. Generate predictions for new production scenarios.
10. Export plots, reports, predictions, and trained models.

## 🤖 Machine Learning Models

The project compares the following regression models:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regression
- Random Forest Regression
- Stepwise Regression

**Model evaluation metrics:**

- **RMSE:** Measures the magnitude of prediction errors.
- **MAE:** Measures the average absolute prediction error.
- **R² Score:** Measures how much variation in productivity is explained by the model.

The model with the lowest RMSE is selected as the preferred regression model. Random Forest is the intended final model in this project, subject to validation results.

A Logistic Regression model is also used to classify whether a production team meets its target productivity.

## 📈 Key Features

- Automated data cleaning and preprocessing
- Productivity analysis by department and working day
- Correlation analysis and statistical testing
- Actual-versus-predicted productivity plots
- Regression model comparison
- Feature importance visualization
- Target achievement classification
- Confusion matrix generation
- New production scenario predictions
- Exportable CSV reports and saved models
- PowerPoint plot integration

## 📁 Project Structure

```text
Apparel-Productivity-Prediction/
│
├── apparel_prediction.R
├── insert_plots.py
├── garments_worker_productivity.csv
├── requirements.txt
├── README.md
├── Apparel_Manufacturing_Prediction_R_Project_PPT.pptx
├── Final_PPT.pptx
│
└── outputs/
    ├── cleaned_garment_data.csv
    ├── model_comparison.csv
    ├── test_predictions.csv
    ├── new_order_predictions.csv
    ├── logistic_confusion_matrix.txt
    ├── best_random_forest_model.rds
    ├── logistic_model.rds
    │
    └── plots/
        ├── 01_target_distribution.png
        ├── 02_productivity_by_department.png
        ├── 03_productivity_by_day.png
        ├── 04_boxplots.png
        ├── 05_correlation_matrix.png
        ├── 06_incentive_vs_productivity.png
        ├── 07_decision_tree.png
        ├── 08_model_comparison.png
        ├── 09_feature_importance.png
        ├── 10_confusion_matrix.png
        └── Actual_vs_Predicted_Plots/
```

*Note: The actual output files and plot names depend on the project script.*

## 💻 Installation and Execution

### Prerequisites

Install the following software:

- R 4.5 or later
- Python 3
- RStudio (optional)
- Required dataset and project files

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY
```

Replace the placeholder URL with your actual GitHub repository URL.

### Step 2: Install Python Dependencies

```bash
python -m pip install -r requirements.txt
```

### Step 3: Run the R Analysis

```bash
Rscript apparel_prediction.R
```

The script processes the dataset, trains the models, generates visualizations, and saves the outputs in the `outputs/` directory.

### Step 4: Generate the Final Presentation

```bash
python insert_plots.py "Apparel_Manufacturing_Prediction_R_Project_PPT.pptx" outputs/plots "Final_PPT.pptx"
```

This command inserts the generated plots into the PowerPoint template and saves the final presentation.

## 📂 Output Files

| File | Description |
|---|---|
| `cleaned_garment_data.csv` | Preprocessed dataset |
| `model_comparison.csv` | Regression model evaluation results |
| `test_predictions.csv` | Predictions on test data |
| `new_order_predictions.csv` | Predictions for new scenarios |
| `logistic_confusion_matrix.txt` | Classification evaluation |
| `best_random_forest_model.rds` | Saved Random Forest model |
| `logistic_model.rds` | Saved Logistic Regression model |

## 🌟 Expected Outcomes

- Better understanding of garment production productivity.
- Identification of important production-related factors.
- Comparison of regression models for productivity prediction.
- Prediction of target achievement for production teams.
- Visual reports to support production analysis and planning.

Actual performance metrics should be obtained by running the project on the dataset and reviewing the generated evaluation results.

## 👨‍💻 Developer

**Jagadeesh M**

Developer of the Apparel Productivity Prediction and Analysis project.

**Areas of Interest:** R Programming, Data Analytics, Machine Learning, Predictive Modeling, and Data Visualization.

## 🎓 Project Purpose

This project is developed for academic and educational purposes as an R programming mini-project. It demonstrates the practical application of data analytics and machine learning techniques to apparel manufacturing productivity analysis.

## 📜 License

This project is intended for educational and academic use. Add a specific open-source license, such as the MIT License, if you want to permit reuse under its terms.
