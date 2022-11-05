# Machine Learning Scikit-learn

Table of Contents

    Contents

    First look at the dataset

    EDA

        Checking for Missing Values

        Basic Statistical Details

        Correlation Heatmap

    Data Visualization
        Histogram

    Pre-Modeling Tasks
        Separating the independant and the dependant variable
        Splitting the dataset
        Feature Scaling

    Modeling
        Logistic Regression
        Gradient Boosting Classifier
        Random Forest Classifier
        Decision Tree Classifier
        KNeighbors Classifier
        XGB Classifier
        Suport Vector Machine

    Evaluation and comparision of all the models

        Classification Accuracy

        Confusion matrix

        Precision

        Recall

        classification_report

        ROC AUC Score

        Area under curve (AUC)

Look at the dataset

Attribute Information:

        ID number
        Diagnosis (M = malignant, B = benign)

Ten real-valued features are computed for each cell nucleus:

    a) radius (mean of distances from center to points on the perimeter)
    b) texture (standard deviation of gray-scale values)
    c) perimeter
    d) area
    e) smoothness (local variation in radius lengths)
    f) compactness (perimeter^2 / area - 1.0)
    g) concavity (severity of concave portions of the contour)
    h) concave points (number of concave portions of the contour)
    i) symmetry
    j) fractal dimension ("coastline approximation" - 1)

**Check the target variable:**

    Malignant = 1 (indicates prescence of cancer cells)

    Benign = 0 (indicates abscence)

**What is the difference between Malignant and Benign ?**

Differences Between a Malignant and Benign Tumor

How many Benign and Malignant do we have in our dataset?

df['diagnosis'].value_counts()

B    357
M    212
Name: diagnosis, dtype: int64

As we can see, we have 212 - Malignant, and 357 - Benign
