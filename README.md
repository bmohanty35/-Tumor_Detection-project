# -Tumor_Detection-project

Tumor Detection - Summary of Project
1. Approach
The goal of this project is to develop a machine learning model that can accurately classify tumors as malignant (M) or benign (B) based on a set of features extracted from medical imaging data.

2. Methodology
- Data Preprocessing:
Dataset: A CSV file (Tumor_Detection.csv) was loaded.

Cleaning:

Dropped the id column (not useful for modeling).

Verified data types and null values.

Mapped the diagnosis labels: 'M' → 1, 'B' → 0.

- Feature Engineering:
Features were grouped into three categories:

Mean (feature_mean)

Standard error (feature_se)

Worst case (feature_worst)

- Exploratory Data Analysis:
Count plot to show class distribution of diagnosis.

Summary statistics (.describe())

Correlation heatmap for all numerical features.

- Train/Test Split:
Input features (X) and target variable (y) were defined.

Data was split into training (70%) and testing (30%) sets.

- Feature Scaling:
StandardScaler was used to normalize feature values.

3. Analysis Process
- Model Used:
Random Forest Classifier (from sklearn.ensemble)

Trained on the scaled training data.

Prediction performed on the test set.

- Evaluation:
Model performance evaluated using accuracy score from sklearn.metrics.

4. Key Findings
The model successfully classified tumors with high accuracy (exact value shown in output, e.g., ~92% depending on split).

The dataset was well-prepared with distinct separation between benign and malignant classes.

Correlation heatmap helped visualize feature relationships, supporting model robustness.
