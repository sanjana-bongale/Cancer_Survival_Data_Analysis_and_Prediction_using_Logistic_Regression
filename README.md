# 🧬 Cancer Survival Data Analysis and Prediction Using Logistic Regression

This project focuses on analyzing a dataset of cancer patients from China to understand patterns in diagnosis, treatment, and survival. We perform data cleaning, exploratory data analysis (EDA), and visualization to gain insights, followed by logistic regression modeling to predict survival outcomes.

## 📁 Project Structure

- `Part 1-4`: Data Loading, Cleaning, and Preprocessing
- `Part 5`: Data Visualization using Seaborn and Matplotlib
- `Part 6`: Logistic Regression Modeling

## 🧰 Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## 📦 Dataset

The dataset used (`cancer_patients_china.csv`) contains anonymized records of cancer patients, with various features and their corresponding data types:

- **Patient_ID**: Unique identifier for each patient (object)
- **Age**: Age of the patient at the time of diagnosis (int64)
- **Gender**: Gender of the patient (object)
- **Province**: The province in China where the patient resides (object)
- **Urban_Rural**: Indicates whether the patient lives in an urban or rural area (object)
- **Ethnicity**: Ethnic background of the patient (object)
- **Occupation**: The patient's occupation (object)
- **Insurance_Type**: The type of insurance the patient has (object)
- **Family_History**: Whether the patient has a family history of cancer (object)
- **Cancer_Type**: The type of cancer diagnosed (object)
- **Stage_at_Diagnosis**: The stage of cancer at the time of diagnosis (object)
- **Diagnosis_Date**: The date when the cancer was diagnosed (datetime64[ns])
- **Symptoms**: The symptoms the patient exhibited at diagnosis (object)
- **Metastasis_Sites**: The sites where cancer has spread (object)
- **Tumor_Size**: The size of the tumor (float64)
- **Treatment_Types**: Types of treatments the patient underwent (object)
- **Surgery_Date**: The date when the patient had surgery (datetime64[ns])
- **Chemotherapy_Drugs**: Drugs used during chemotherapy (object)
- **Radiation_Sessions**: The number of radiation therapy sessions (int64)
- **Immunotherapy**: Whether the patient underwent immunotherapy (object)
- **Targeted_Therapy**: Whether the patient underwent targeted therapy (object)
- **Survival_Status**: Indicates whether the patient survived or not (object)
- **Survival_Months**: The number of months the patient survived after diagnosis (float64)
- **Recurrence_Status**: Indicates whether the cancer recurred after treatment (object)
- **Smoking_History**: Patient’s smoking history (object)
- **Alcohol_Use**: Patient’s alcohol use history (object)
- **BMI**: Body Mass Index of the patient (float64)
- **Biomarker_1**: Presence of a specific biomarker (object)
- **Biomarker_2**: Presence of another biomarker (object)

📁 **Dataset Link:** [https://www.kaggle.com/datasets/ak0212/cancer-patient-dataset-china](https://www.kaggle.com/datasets/ak0212/cancer-patient-dataset-china)

## 📊 Key Visualizations

The project includes key visualizations such as the distribution of age, gender, cancer types, and diagnosis stage. It also highlights the comparison between urban and rural patients, survival patterns across provinces, and survival outcomes by cancer type and stage. Other visualizations cover treatment types used at different cancer stages, along with the average survival months for each stage. These visualizations help in understanding key trends in the data and the relationship between cancer characteristics and survival outcomes.

## 🔍 Logistic Regression Model

The logistic regression model is trained to predict the survival status of cancer patients based on various features in the dataset. We followed these key steps for the modeling process:

1. **Data Preparation**:
   - Categorical variables were encoded using Label Encoding.
   - Missing values were handled appropriately by either filling or dropping them, depending on the situation.
   - Feature scaling was performed to standardize numerical variables.

2. **Model Training**:
   - The dataset was split into training and testing sets (80-20 split).
   - A logistic regression model was trained on the training data using the `scikit-learn` library.

3. **Evaluation**:
   - Model performance was evaluated using metrics such as accuracy, precision, recall, and F1-score.
   - Confusion matrix was plotted to assess the model's prediction capability.
   - ROC curve and AUC score were also computed to evaluate the model's discriminative power.

4. **Prediction**:
   - The trained model was used to predict the survival status for the test set.
   - The final model can predict whether a patient will survive or not based on their medical and demographic features.

The logistic regression model allows for quick and interpretable predictions, which can be useful in real-world applications for early cancer diagnosis and survival predictions.
