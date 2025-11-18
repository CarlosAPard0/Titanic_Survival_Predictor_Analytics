# 🚢 Titanic Survival Predictor: A Comprehensive Data Science Deep Dive

## ✨ Project Overview

This project provides an in-depth analysis of the infamous Titanic disaster, focusing on predicting passenger survival using a robust data science pipeline. It showcases a wide array of techniques, from advanced feature engineering and exploratory data analysis (EDA) to comparative machine learning modeling, including traditional algorithms and a Neural Network. The goal is to not only predict survival but also to uncover the underlying factors that influenced who lived and who perished.

**Key Skills Demonstrated:**

* **Data Acquisition & Cleaning:** Handling missing values, data type conversion.
* **Feature Engineering:** Creating impactful new features from raw data.
* **Exploratory Data Analysis (EDA):** Visualizing insights for executive decision-making.
* **Data Preprocessing:** Scaling, encoding, and preparing data for various ML models.
* **Machine Learning:** Implementation and comparison of:
    * Logistic Regression
    * Support Vector Machines (SVM)
    * Random Forest
    * XGBoost
    * Deep Learning (Neural Network with Keras/TensorFlow)
* **Model Evaluation:** Cross-validation, Accuracy, Confusion Matrices, ROC Curves.
* **Interpretability:** Feature Importance analysis for actionable insights.
* **Data Storytelling:** Communicating complex results through compelling visualizations.

## 🚀 Data Science Pipeline

The project follows a structured data science workflow, ensuring reproducibility and clarity:

1.  **Data Acquisition & Setup:** Downloading the dataset from Kaggle.
2.  **Initial Data Exploration:** Understanding the raw data structure and types.
3.  **Feature Engineering & Cleaning:** Creating new predictive features (`Title`, `FamilySize`, `IsAlone`, `Deck`) and handling missing values systematically.
4.  **Exploratory Data Analysis (EDA):** Visualizing relationships and survival patterns.
5.  **Data Preprocessing:** Scaling features for model compatibility.
6.  **Comparative Machine Learning Modeling:** Training and evaluating a diverse set of models.
7.  **Deep Learning Implementation:** Building and training a Neural Network.
8.  **Model Evaluation & Interpretation:** Comparing performance, understanding feature importance, and generating executive summaries.

## 📊 Key Findings & Visualizations

Here are some highlights from the analysis, demonstrating key insights and your visualization skills:

### 1. What Factors Decided Survival? (Feature Importance)

Understanding which features the models considered most important is crucial for real-world impact. This plot, derived from the Random Forest model, clearly shows the hierarchy of influence.

![Feature Importance Plot](https://github.com/CarlosAPard0/Titanic_Survival_Predictor_Analytics/blob/main/Figures/factores_influyentes.png) 


**Insight:** `Sex` and `Title` (derived from `Name`) were overwhelmingly the most critical factors, followed by `Fare` and `Pclass`. This strongly indicates that social status and gender played a dominant role in who survived.

### 2. Survival Probability by Class and Sex

This visualization directly addresses the question of whether "women and children first" was true, and how social class impacted survival rates.

![Survival by Pclass and Sex](https://github.com/CarlosAPard0/Titanic_Survival_Predictor_Analytics/blob/main/Figures/clase_y_sexo_vs_supervivencia.png)


**Insight:** Women in all classes had significantly higher survival rates than men. First-class passengers, particularly women, had the highest chances of survival, confirming socio-economic biases.

### 3. Model Performance Comparison

Comparing various models helps in selecting the most effective predictor. This bar chart summarizes the cross-validation accuracy of each algorithm.

![Model Comparison Plot](https://github.com/CarlosAPard0/Titanic_Survival_Predictor_Analytics/blob/main/Figures/comparativa_de_modelos.png)


**Insight:** The **Neural Network** and **XGBoost** models typically achieved the highest accuracy, demonstrating the power of advanced algorithms for tabular data prediction. This shows proficiency in selecting and implementing state-of-the-art techniques.

### 4. Correlation Matrix: Uncovering Relationships

A heatmap provides a quick overview of how each feature correlates with `Survived` and with each other. This is fundamental for initial data understanding.

![Correlation Matrix](https://github.com/CarlosAPard0/Titanic_Survival_Predictor_Analytics/blob/main/Figures/correlacion_matriz.png)


**Insight:** `Sex` has a strong positive correlation with survival (being female increases chances), while `Pclass` and `Age` show negative correlations (lower class and older age decrease chances).

## 🛠️ Technologies Used

* Python (Pandas, NumPy)
* Scikit-learn (Machine Learning Models, Preprocessing, Evaluation)
* XGBoost
* TensorFlow / Keras (Neural Networks)
* Matplotlib & Seaborn (Data Visualization)
* Jupyter Notebooks

## 👨‍💻 How to Run the Project

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/your-username/Titanic_Survival_Predictor_Advanced_Analytics.git](https://github.com/your-username/Titanic_Survival_Predictor_Advanced_Analytics.git)
    cd Titanic_Survival_Predictor_Advanced_Analytics
    ```
2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    (You'll need to create a `requirements.txt` file from your notebook's imports: `pip freeze > requirements.txt`)
3.  **Kaggle API Setup:**
    * Ensure you have a Kaggle account.
    * Download your `kaggle.json` API token from your Kaggle account settings.
    * Place `kaggle.json` in `~/.kaggle/` (or run the setup code in the notebook).
4.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook Titanic_Advanced_Analytics.ipynb
    ```
    Follow the cells sequentially to reproduce the analysis.

## 🤝 Contribution

Feel free to fork this repository, open issues, or submit pull requests.

---
