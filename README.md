# Machine-Learning
This is a selection of exercises for Machine learning. Projects relating to classifiers and regressions, and the tuning thereof. It is important to note that the focus of this course was the **mathematical basis of models and methods, and understanding the workings thereof**. The focus of the next half, **data mining focused on implentation**. Following concepts is a breakdown of each project.


Models used in this module:
1) **Naive Bayes**
2) **SVC**: Support Vector Classification
3) **SVM**: Support Vector Machine
4) **PCA**: Principal Component Analysis
5) Decision Trees, sort of
6) **Random Forest**

Topics covered within this module: 
1) **Classification Models**
   Using **SVC**
   Using **Random Forest**
   Running **classification**, **clustering** and **regression** analysis on featurized texts
   
3) Data preparation
    - **Encoding**
      - **Time Series encoding**
      - **One hot** encoding
      - **Ordinal** encoding
      - **Label** encoding
      - **Dummy** encoding
    - **Feature reduction**
    - **Correlation** via heatmap
    - **PCA**: Principal Component Analysis
    - Normalization
    - Scaling(**StandardScaler**)
    - Oversampling, via **S**ynthetic **M**inority **O**versampling **Te**chnique(SMOTE)
      
  4) **Model Training and Tuning**
     -  Training and testing data, and tradeoffs.
    - Resampling training and test data
    - Via **GridSearchCV** and **Pipeline**
 


  5) **Confustion Matrix**, importance of highlighting true/false positives and true/false negatives
    - **MultiLayer Perceptron**
 
  6) **Unsupervised Learning**
     - via **PCA**
       
  7) **Supervised Learning**
     - via **Random Forest**
     - via **SVC**
     - via **Linear Regression**
       
  8) **Evaluation Metrics**
     - Models' performances are evaluated based on **R-squared** metrics and **P-Values**
    

**In "Multi_classes_feature.ipynb":**

Data Reading and Examination:

- Reading a dataset from a CSV file.
- Checking the dataset's structure and information using data.info().

Data Preprocessing:
- Encoding categorical variables ('quality') into numerical values.
- Dropping unneeded columns ('quality') to prepare data for classification.

Data Splitting:
- Splitting the dataset into feature set (X) and label set (Y).

Data Normalization:
- Standardizing features (X) using StandardScaler.

Random Forest Classifier:
- Implementing a Random Forest Classifier.
- Tuning hyperparameters using Grid Search to optimize the number of trees ('n_estimators').
- Evaluating classifier performance based on precision.

Feature Importance:
- Extracting feature importances from the best model.
- Principal Component Analysis (PCA):
- Applying PCA to reduce dimensionality.
- Transforming features using PCA for dimensionality reduction.
- Training a Random Forest Classifier on the PCA-transformed features.

**In "LR.ipynb":**

Data Reading and Examination:
- Reading a dataset from a CSV file.
- Checking dataset characteristics using data.info().

Data Preprocessing:
- Encoding categorical variables ('CentralAir' and 'PavedDrive') to numeric values.
- Preparing data for linear regression.

Data Splitting:
- Splitting the dataset into feature set (X) and label set (Y).

Data Normalization:
- Standardizing features (X) using StandardScaler.

Linear Regression (LR):
- Implementing a Linear Regression model.
- Hyperparameter tuning using Grid Search for learning rate ('eta0') and maximum iterations ('max_iter').
- Evaluating the model's performance based on R-squared.

Regularization:
- Applying L2 regularization (Elastic Net) by using the 'alpha' and 'l1_ratio' parameters.

**In "SVM1.ipynb":**

Data Reading and Examination:
- Reading a dataset from a CSV file.
- Checking the dataset's structure and information using data.info().

Data Preprocessing:
- Encoding categorical variables ('PastEmployee', 'OverTime', 'Gender') into binary values.
- Preparing data for SVM classification.

Data Splitting:
- Splitting the dataset into feature set (X) and label set (Y).

Data Normalization:
- Standardizing features (X) using StandardScaler.

Support Vector Classifier (SVC):
- Implementing a Support Vector Classifier (SVC) model.
- Hyperparameter tuning using Grid Search for the kernel type and regularization parameter ('C').
- Evaluating the model's performance based on accuracy and confusion matrix.

**In "Encoding MultiClass, SVR and RFReg.ipynb":**

Data Reading and Examination:
- Reading a dataset from a CSV file.
- Checking the dataset's structure and information using data.info().

Data Preprocessing:
- Encoding categorical variables ('Status') into binary values.
- Preparing data for regression analysis.

Data Analysis:
- Calculating and visualizing the correlation between features using a heatmap.

Feature Selection:
- Dropping unneeded columns ('infant deaths', 'percentage expenditure') from the dataset.

Data Splitting:
- Splitting the dataset into feature set (X) and label set (Y).

Target Encoding:
- Applying target encoding to the 'Country' column using the TargetEncoder from the category_encoders library.

Data Normalization:
- Standardizing features (X) using StandardScaler.

Random Forest Regression:
- Implementing Random Forest Regression.
- Hyperparameter tuning using Grid Search for the number of trees ('n_estimators').
- Evaluating the regression model's performance based on R-squared.
- Extracting feature importances from the best model.

Support Vector Regression (SVR):
- Applying Support Vector Regression (SVR).
- Hyperparameter tuning using Grid Search for the kernel type and regularization parameter ('C').
- Evaluating the regression model's performance based on R-squared.
