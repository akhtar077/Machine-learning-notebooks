Machine Learning Internship - Bahash.ai 🤖
This repository contains the projects, assignments, and code implemented during my Machine Learning internship at Bahash.ai. The work focuses on building a strong foundation in Machine Learning using Python, covering supervised and unsupervised learning algorithms, model evaluation, and data preprocessing techniques.

📌 Internship Overview
Organization: Bahash.ai
Focus Area: Machine Learning, Data Science, Python
Tools Used: Python, Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn

📂 Projects Implemented
During the internship, I developed the following key projects, applying various ML algorithms and techniques:
1. Student Performance Dataset:
Dataset Overview
The dataset, titled StudentPerformance.csv, contains records for 10,000 students and is used to predict a student's performance based on various academic and lifestyle factors. It includes the following features:
Hours Studied: The total number of hours a student spent studying.
Previous Scores: The student's scores from previous exams.
Extracurricular Activities: A categorical indicator (Yes/No) of whether the student participates in extracurriculars.
Sleep Hours: The average number of hours the student sleeps per night.
Sample Question Papers Practiced: The number of practice papers completed.
Performance Index: The target variable representing the student's overall performance.

Key Libraries Used
The project utilizes several essential Python libraries for data science and model development:
Pandas: Primary tool for data manipulation and loading the CSV dataset into a DataFrame.
NumPy: Used for numerical operations and handling arrays.
Scikit-learn (sklearn): The core machine learning library used for building the predictive model.
Seaborn & Matplotlib: Used for statistical data visualization and creating plots (e.g., pairplot, scatterplot) to analyze data distributions and relationships.
Joblib: Employed for model persistence, allowing the trained model to be saved and reloaded later.
Scipy: Used for residual analysis and generating probability plots.

Key Techniques and Algorithms
1. Data Preprocessing
Categorical Mapping: The Extracurricular Activities column was transformed from text ('Yes', 'No') into numerical values (1, 0) using a mapping function to make it compatible with the mathematical requirements of the algorithm.
Data Splitting: Although the final training step is not shown in the snippet, the notebook references the use of train_test_split to divide the data for training and evaluation.
2. Machine Learning Algorithm
Linear Regression: The primary algorithm used for this task is Multiple Linear Regression. This technique models the relationship between the multiple independent variables (study hours, sleep, etc.) and the single continuous dependent variable (Performance Index) by fitting a linear equation to the observed data.
3. Performance Evaluation
The notebook outlines several metrics to measure the model's accuracy and error:
Mean Absolute Error (MAE): Measures the average magnitude of errors in predictions.
Mean Squared Error (MSE): Measures the average of the squares of the errors.
Root Mean Squared Error (RMSE): The square root of MSE, providing error values in the same units as the target variable.
R² Score: Indicates how well the independent variables explain the variance in the performance index.

2.Mushroom Classification:
Dataset Overview
The dataset focuses on the classification of mushrooms, categorizing them as either edible (e) or poisonous (p) based on their physical characteristics. It consists of 8,124 rows and 23 columns, covering features such as:
Cap features: Shape, surface, and color.
Stem/Stalk features: Shape, root, and color above/below the ring.
Environment: Population and habitat.
Odor and Bruises: Key chemical and physical indicators.

Key Libraries Used
The project utilizes the standard Python data science stack for preprocessing and modeling:
Pandas: Used for data manipulation, reading the CSV file, and handling the DataFrame structures.
Scikit-learn (sklearn): The primary machine learning library used for:
Preprocessing: LabelEncoder to convert categorical text data into numerical values.
Model Selection: train_test_split for data partitioning and cross_val_score for performance validation.
Algorithms: A variety of classification models.

Techniques and Algorithms
1. Data Preprocessing
Label Encoding: Since the original data consists of strings (letters), the LabelEncoder was applied across all columns to translate these into integers so they could be processed by mathematical models.
Data Splitting: The data was split into a 70% training set and a 30% testing set to evaluate how well the models generalize to unseen data.
2. Machine Learning Algorithms
Several classifiers were trained and compared to find the most accurate model:
Decision Tree Classifier: Achieved a perfect 1.0 (100%) accuracy on the test set.
Random Forest Classifier: Also achieved 100% accuracy, demonstrating that ensemble methods are highly effective for this categorical dataset.
Support Vector Classifier (SVC): Performed strongly with approximately 98.9% accuracy.
Logistic Regression: A linear approach that reached about 95.1% accuracy.
Gaussian Naive Bayes: A probabilistic model that yielded about 92.1% accuracy.
3. Evaluation Technique
K-Fold Cross-Validation: The notebook used cross_val_score (with 3 folds) to ensure the models weren't just "lucky" on one specific split, providing a more robust measure of performance across different subsets of the data.

3.Drugs Classification:
Dataset Overview
The dataset contains information about patients and the specific drug that was prescribed to them based on their health metrics. It includes 200 rows and 6 columns with the following features:
Demographics: Age and Sex.
Health Indicators: Blood Pressure levels (BP) and Cholesterol levels.
Chemical Markers: Sodium-to-Potassium ratio (Na_to_K).
Target Variable: The specific drug assigned (Drug).

Key Libraries Used
The project relies on standard Python libraries for data processing and model evaluation:
Pandas: Used for loading the dataset from a CSV file and performing data manipulation.
Scikit-learn (sklearn): The core library for all machine learning tasks, including:
Preprocessing: LabelEncoder for transforming categorical text into numerical data.
Model Selection: train_test_split for dividing the data into training and testing sets.
Algorithms: Various classification models like Decision Trees and Random Forests.

Key Techniques and Algorithms
1. Data Preprocessing
Label Encoding: Categorical features (such as Sex, BP, and Cholesterol) were converted into numerical values using LabelEncoder to make them compatible with machine learning algorithms.
Train-Test Split: The data was partitioned into training and testing sets using a 70/30 split to evaluate model performance on unseen data.
2. Machine Learning Algorithms
The notebook compares several classification models to predict the correct drug:
Decision Tree Classifier: Achieved a perfect accuracy score of 1.0 (100%) on the test set.
Random Forest Classifier: Also achieved an accuracy of 1.0 (100%), indicating that tree-based models are highly effective for this dataset.
Support Vector Classifier (SVC): Performed with an accuracy of approximately 0.91 (91.67%).
Logistic Regression: Yielded an accuracy of approximately 0.91 (91.67%) after 1000 iterations.
Gaussian Naive Bayes: Resulted in an accuracy of approximately 0.88 (88.33%).
3. Validation Technique
Cross-Validation: The notebook utilizes cross_val_score to validate the models across different subsets of the data. This ensures the high accuracy scores are consistent and not a result of a specific data split.
