# 🥋 UFC Fight Outcome Predictor
This project utilizes a machine learning model to predict fight outcomes from previous UFC fights. Here I used Random Forest with RandomizedGridSearchCV for hyperparameter tuning to improve prediction accuracy.

## 🧠 Model Summary
**Model:** RandomForestClassifier
**Tuning:** GridSearchCV with 5-fold cross-validation
**Preprocessing:**
Imputation with `SimpleImputer`
Feature scaling using `StandardScaler`
I also used PCA but removed it because I realized that it was not necessary

### Hyperparameters Tuned
- n_estimators
- max_depth
- min_samples_leaf
- min_samples_split
- max_features

### Final Model Scoring
**Best Model** RandomForestClassifier(max_depth=13, min_samples_leaf=9, min_samples_split=6,n_estimators=250)
**Accuracy:** 0.6937
**F1-score:** 0.7483
**Precision:** 0.7170
**Recall Score:** 0.7825

#### Key Learnings/Improvements To Be Made
- PCA was not beneficial for Random Forest
- Remove more columns if the majority were NaN values
- Hyperparameter does not always improve model performance but only minimal
- 

