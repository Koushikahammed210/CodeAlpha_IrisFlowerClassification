🌸 CodeAlpha – Iris Flower Classification
Task 1 of the CodeAlpha Data Science Internship.

📌 Objective
Build a machine learning model that classifies iris flowers into three species —setosa, versicolor, and virginica — based on their measurements(sepal length, sepal width, petal length, petal width).

📊 Dataset
Source: Built-in Iris dataset via sklearn.datasets.load_iris()
Samples: 150 flowers (50 per species — perfectly balanced)
Features (4): sepal length (cm), sepal width (cm), petal length (cm), petal width (cm)
Target (3 classes): setosa, versicolor, virginica
🛠️ Tools & Libraries
Python
Pandas, NumPy
Matplotlib, Seaborn (visualization)
Scikit-learn (model building & evaluation)
🔄 Workflow
Load & explore the dataset — checked class balance and feature distributions
Visualize with a pairplot to see how species separate across features
Preprocess — scaled features using StandardScaler, split 80/20 (train/test)
Train a Logistic Regression classifier
Evaluate using accuracy, classification report, and confusion matrix
📈 Results
Metric	Score
Model	Logistic Regression
Test Accuracy	93.33% (28/30 correct)
Confusion Matrix:

setosa	versicolor	virginica
setosa	10	0	0
versicolor	0	9	1
virginica	0	1	9
🔍 Key Insights
The pairplot shows setosa is completely separable from the other species(especially by petal length/width) — it was classified perfectly (10/10).
Versicolor and virginica overlap slightly in feature space, which explainsthe single misclassification in each direction.
Petal measurements are far more useful for classification than sepal measurements.
📁 Project Structure
CodeAlpha_IrisFlowerClassification/├── Iris_Classification.ipynb   # full code + outputs├── pairplot.png                # feature visualization├── confusion.png               # confusion matrix heatmap└── README.md
▶️ How to Run
Open the notebook in Google Colab or Jupyter and run all cells —the dataset loads automatically via scikit-learn (no download needed).
