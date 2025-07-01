Task 6: K-Nearest Neighbors (KNN) Classification

 Objective
Understand and implement KNN for classification problems using the Iris dataset.

 Tools Used
- Python (Pandas, NumPy)
- Scikit-learn
- Matplotlib 

Dataset

Kaggle dataset download

 Steps Followed

 Load and Preprocess Data
- Read ‘Iris.csv’ using Pandas
- Strip whitespace from column names
- Encode target labels (`Species`) into numeric values

 Feature & Target Separation
python
X = irisdata.drop("Species", axis=1)
y = irisdata["Species"]


Feature Scaling
Used ‘StandardScaler’ to normalize features.

Train-Test Split
python
X_train, X_test, y_train, y_test = train_test_split(X_scaled, y, test_size=0.3, random_state=42)


 KNN Model Training & Evaluation
- Tried values of K from 1 to 20
- Measured accuracy for each
- Plotted K vs Accuracy graph

 Confusion Matrix
Plotted confusion matrix for the best-performing K value.

. Decision Boundary Plot (2 Features)

- Used only ‘PetalLengthCm’ and ‘PetalWidthCm’
- Plotted decision boundaries using ‘contourf()’ and ‘scatter()’

 Learnings

- KNN is an instance-based learner
- Euclidean distance matters in scaled space
- K selection is crucial for balancing bias-variance

Author
BOKKETI PRANITHA


