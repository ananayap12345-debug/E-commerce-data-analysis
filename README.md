#  AI-Powered Fashion Recommendation System

##  Project Overview

The **AI-Powered Fashion Recommendation System** is a machine learning project designed to provide personalized fashion recommendations based on customer preferences, body measurements, occasions, seasons, and sustainability factors.

The project uses machine learning models to predict suitable clothing sizes and clothing types. It also incorporates sustainability information to help identify environmentally preferable fashion alternatives.

##  Project Objectives

- Predict clothing sizes using customer information and body measurements.
- Recommend clothing categories and dress types based on customer preferences.
- Analyze fashion trends and customer characteristics using Exploratory Data Analysis (EDA).
- Evaluate environmental factors such as eco-score, carbon footprint, water usage, and fabric waste.
- Identify more sustainable alternatives to clothing products when suitable alternatives are available.
- Develop an integrated system combining fashion recommendations with sustainability insights.

##  Dataset Description

The project uses an AI fashion recommendation dataset containing customer, clothing, and sustainability-related information.

Important dataset features include:

| Category | Features |
|---|---|
| Customer Information | Age, Gender, Region |
| Body Measurements | Height, Weight, BMI, Chest, Waist, Hip |
| Body Characteristics | Body Shape, Preferred Fit |
| Fashion Preferences | Favorite Color, Budget, Brand |
| Clothing Information | Product Category, Dress Type, Fabric |
| Seasonal Information | Season, Occasion |
| Size Information | Recommended Size |
| Sustainability Information | Eco Score, Carbon Footprint, Water Usage, Fabric Waste |

*Note: The dataset file must be included in the repository or its source must be documented separately.*

##  Technologies Used

- **Python** – Programming language
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical computations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical data visualization
- **Scikit-learn** – Machine learning and model evaluation
- **XGBoost** – Gradient boosting
- **LightGBM** – Gradient boosting
- **Joblib** – Saving trained machine learning models
- **Google Colab / Jupyter Notebook** – Development environment

##  Project Workflow

### 1. Data Loading
Load the fashion dataset into a Pandas DataFrame for analysis and model development.

### 2. Data Preprocessing
Inspect the dataset, examine missing values and duplicate records, and prepare numerical and categorical features for machine learning.

### 3. Exploratory Data Analysis (EDA)
Perform data analysis and visualization to understand:

- Gender distribution
- Age distribution
- Clothing size distribution
- Fabric and seasonal patterns
- Relationships between body measurements and clothing sizes
- Relationships among sustainability indicators

### 4. Clothing Size Prediction
Train a Random Forest classifier to predict the recommended clothing size using features such as age, gender, height, weight, BMI, body shape, chest, waist, hip, and preferred fit.

### 5. Clothing Type Prediction
Train a machine learning model to predict product category and dress type using customer preferences, occasion, budget, season, fabric, brand, and other relevant features.

### 6. Model Evaluation
Evaluate model performance using training and testing accuracy and classification metrics.

Additional experiments use XGBoost and LightGBM to explore model performance and generalization.

### 7. Sustainable Fashion Recommendations
Use product and sustainability information to identify alternative clothing options with higher sustainability scores when suitable alternatives are available.

### 8. Integrated Recommendation System
Combine size prediction, clothing recommendations, and sustainability information to generate personalized fashion recommendations.

##  Machine Learning Models

The project includes the following machine learning approaches:

- **Random Forest Classifier:** Used for clothing size and clothing type prediction.
- **XGBoost Classifier:** Explored for fashion prediction and model evaluation.
- **LightGBM Classifier:** Explored as an alternative gradient boosting approach.

Categorical features are encoded, and preprocessing is integrated with machine learning pipelines where applicable.

##  Expected Outcomes

The system aims to:

- Predict suitable clothing sizes from customer features.
- Recommend clothing categories and dress types.
- Provide insights into fashion preferences and product distributions.
- Compare clothing products using available sustainability indicators.
- Suggest more sustainable alternatives when suitable options exist.
- Demonstrate how machine learning can support personalized and sustainability-aware fashion recommendations.

Actual prediction performance should be reported using the results obtained by running the notebook.

##  Project Structure

A suggested GitHub repository structure is:

```text
AI-Powered-Fashion-Recommendation-System/
│
├── NTCC_PROJECT.ipynb
├── fashion_dataset.csv
├── size_model.pkl
├── clothing_model.pkl
├── requirements.txt
└── README.md
```

**Important:** Include the dataset and trained model files only if you intend to distribute them and have permission to do so. The notebook currently saves the dataset as `fashion_dataset.csv` and the trained models as `size_model.pkl` and `clothing_model.pkl`. Make sure the filenames in the repository match the actual files you upload.

## ⚙️ Installation and Setup

### Step 1: Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
```

### Step 2: Navigate to the Project Folder

```bash
cd AI-Powered-Fashion-Recommendation-System
```

### Step 3: Install the Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib xgboost lightgbm
```

### Step 4: Open the Notebook

Open `NTCC_PROJECT.ipynb` in Google Colab or Jupyter Notebook.

### Step 5: Load the Dataset

Upload the fashion dataset when prompted, or update the notebook to use the dataset's actual location.

### Step 6: Run the Notebook

Execute the cells in order to perform data analysis, train the machine learning models, evaluate predictions, and explore the integrated recommendation system.

**Note:** The notebook contains Google Colab-specific commands. Some cells may need modification before running locally in Jupyter Notebook or VS Code.

##  Future Enhancements

- Develop a web application using Streamlit.
- Create an interactive interface for customer inputs.
- Add personalized recommendations based on shopping history.
- Improve model evaluation and handling of imbalanced target classes.
- Integrate product images and visual search.
- Enhance sustainability comparisons using verified environmental data.
- Connect the system to a real fashion product catalog.

##  Limitations

- Prediction quality depends on the dataset and its representativeness.
- Recommended clothing sizes may vary between brands.
- Sustainability scores and environmental indicators depend on the quality of the available data.
- The project provides recommendations based on learned patterns and available product information; it does not guarantee clothing fit or independently verify environmental claims.

##  Project Information

**Project Title:** AI-Powered Fashion Recommendation System  
**Project Type:** Machine Learning and Data Analysis  
**Application Domain:** Fashion Technology and Sustainable Fashion  
**Purpose:** Academic project for the NTCC programme.

## 👩‍💻 Author

**Developed as an academic project using Python, data analysis, and machine learning.**
