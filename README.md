# On-The-Margin

Project Overview
----------------
On the Margin is a student project exploring the impact of social media on
students' daily lives and well-being. It uses exploratory data analysis (EDA)
and a Support Vector Machine (SVM) classifier to predict the dataset's
Overall_Impact category. Logistic Regression is also trained as a comparison
model.

Dataset
-------
The notebook is designed to use the "Impact of Social Media on Life" dataset,
containing 4,500 student entries and 16 attributes.

Dataset source:
https://www.kaggle.com/datasets/harishyadav0506/impact-of-social-media-on-life

Place the dataset CSV file named:
Social_media_impact_on_life.csv

in the same directory as the notebook before running it.

Project Contents
---------------
- Social.ipynb
  Contains data understanding, cleaning, exploratory visualizations, model
  training, SVM kernel comparison, and Logistic Regression comparison.
- Social_media_impact_on_life.csv
  The dataset required by the notebook (download separately from the source
  above).

Methodology
-----------
1. Load and inspect the dataset.
2. Check missing values and duplicate rows; the notebook drops rows with
   missing values.
3. Explore distributions and relationships involving social media usage,
   sleep, stress, mental health, and academic performance.
4. Predict Overall_Impact using an SVM classifier.
5. Scale features and compare SVM kernels: linear, RBF, polynomial, and sigmoid.
6. Compare the selected SVM model with Logistic Regression using classification
   metrics and confusion matrices.

Model Details
-------------
- Target: Overall_Impact
- Train/test split: 80% training and 20% testing, stratified, random_state=42
- SVM evaluation includes accuracy, weighted precision, weighted recall,
  weighted F1-score, classification report, and confusion matrix.
- The notebook reports that the linear kernel performed best in its kernel
  comparison, with a weighted F1 score stated as approximately 95%.

Software Requirements
---------------------
- Python 3
- Jupyter Notebook or JupyterLab
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

How to Run
----------
1. Install Python and the required packages.
2. Download the dataset CSV from the Kaggle link above.
3. Put Social_media_impact_on_life.csv in the same folder as MiniProjectEda.ipynb.
4. Open MiniProjectEda.ipynb in Jupyter Notebook or JupyterLab.
5. Run the notebook cells in order.

Notes
-----
- Results depend on the dataset and the execution environment.
- The notebook includes a Logistic Regression comparison. Review its metrics
  alongside the SVM results rather than relying on accuracy alone.
- The dataset contains student-related well-being measures. Interpret observed
  relationships as associations; the analysis alone does not establish
  causation.

Project Name
------------
On the Margin
