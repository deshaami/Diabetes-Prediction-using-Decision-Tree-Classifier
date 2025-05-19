# Diabetes Prediction using Decision Tree Classifier

This project uses a **Decision Tree Classifier** to predict whether a patient is diabetic based on medical attributes. The model is trained and evaluated using the **PIMA Indian Diabetes dataset**.

---

## 📌 Project Description

The primary goal is to build an interpretable decision tree model that classifies patients as diabetic (`1`) or not (`0`) based on medical indicators such as glucose level, insulin, BMI, and more.

Steps followed in this project:
- Loading and preprocessing the dataset
- Splitting into training and testing datasets
- Building and training a Decision Tree Classifier
- Evaluating the model using accuracy
- Visualizing the decision tree structure for better interpretability

---

## 💡 Features Used

The model uses the following 7 key features:

- `Pregnancies`
- `Insulin`
- `BMI` (Body Mass Index)
- `Age`
- `Glucose`
- `BloodPressure`
- `DiabetesPedigreeFunction`

The target variable is `Outcome`, where:
- `0` → Non-diabetic
- `1` → Diabetic

---

## 🔧 Model and Evaluation

### Classifier Used
- `DecisionTreeClassifier` from `scikit-learn`
- Criterion: `"entropy"` (Information Gain)
- Max Depth: `3` (for the pruned and interpretable version)

### Evaluation Metric
- **Accuracy**: Computed using `accuracy_score()` from `sklearn.metrics`

### Visualization
- The trained decision tree is visualized using `export_graphviz()` and `pydotplus`
- The final tree is saved as a `.png` file and rendered inline using IPython

---

## 📊 Results and Insights

- The classifier achieves good accuracy on the test set.
- Visualization of the decision tree helps interpret the rules and logic behind the classification.
- Features like **Glucose**, **BMI**, and **Age** are significant in predicting diabetes.

---

## 🧠 Applications

- Can be extended into a decision-support tool for medical practitioners
- Useful as a case study in learning interpretable ML models
- Demonstrates how to use decision trees for binary classification

---

## 💻 Dependencies

- Python 3.x
- pandas
- scikit-learn
- matplotlib (optional for additional visualizations)
- pydotplus
- IPython (for rendering images in notebooks)

Install dependencies with:

```bash
pip install pandas scikit-learn pydotplus matplotlib
