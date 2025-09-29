
# ❤️ Heart Disease Prediction with Decision Trees & Random Forest

This repository explores machine learning methods for predicting heart disease. The focus is on **Decision Trees** and **Random Forests**, with emphasis on model interpretability, overfitting control, and validation.

---

## 🔬 Methodology

1. **Data Preparation**
   - Loaded and preprocessed the heart disease dataset.
   - Split into train-test sets for fair evaluation.

2. **Decision Tree Classifier**
   - Implemented using `sklearn.tree.DecisionTreeClassifier`.
   - Visualized the decision tree with `plot_tree`.
   - Examined overfitting by varying `max_depth`.

3. **Overfitting Analysis**
   - Observed that deeper trees memorized training data.
   - Controlled overfitting using parameters:  
     - `max_depth`  
     - `min_samples_split`  
     - `min_samples_leaf`

4. **Random Forest Classifier**
   - Ensemble of decision trees trained on random subsets.
   - Compared performance with the single decision tree.
   - Showed improved test accuracy and reduced variance.

5. **Feature Importance**
   - Extracted `feature_importances_` from Random Forest.
   - Ranked features such as: age, cholesterol, blood pressure.

6. **Cross-Validation**
   - Applied `cross_val_score` for robust evaluation.
   - Provided a distribution of accuracy across folds.

---

## 📊 Results Summary

| Model              | Train Accuracy | Test Accuracy | Cross-Validation (mean) |
|--------------------|----------------|---------------|--------------------------|
| Decision Tree      | ~98%           | ~75%          | ~77%                     |
| Random Forest      | ~96%           | ~85%          | ~86%                     |

- Decision Tree showed signs of **overfitting**.  
- Random Forest achieved **higher generalization performance**.  
- Feature importance highlighted clinical indicators like **chest pain type** and **exercise-induced angina** as crucial predictors.  

---

## 📌 Tools & Libraries
- **Python 3.x**
- **Scikit-learn**
- **Matplotlib & Seaborn**
- **Pandas & NumPy**

---

## 🚀 Execution
```bash
git clone <repo-url>
cd heart-disease-prediction
pip install -r requirements.txt
python main.py
