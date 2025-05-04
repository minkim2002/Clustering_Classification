# 🌸 Iris Classification using KNN and K-Means

This repository contains two notebook implementations for classifying the Iris dataset using:
- ✅ **K-Nearest Neighbors (KNN)**
- 🔁 **K-Means Clustering**

Each model processes CSV files with Iris flower data and produces predictions and visualizations.

---

## 📁 Project Structure

├── KNN.ipynb # KNN classification implementation
├── K_means.ipynb # K-Means clustering and t-SNE visualization
├── KNN_train.csv # Training data for KNN
├── KNN_test.csv # Test data for KNN
├── KNN_valid.csv # Validation data for KNN
├── K_means_train.csv # Training data for K-Means
├── K_means_test.csv # Test data for K-Means
├── K_means_valid.csv # Validation data for K-Means
├── KNN_test_predict3.csv # Output: KNN predicted labels for test set
├── K_means_test_predict2.csv # Output: K-Means predicted labels for test set

yaml

---

## ⚙️ Requirements

Install required Python packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
🧠 1. KNN Classifier (KNN.ipynb)
📌 Description
Classifies Iris flowers using the K-Nearest Neighbors algorithm.

Calculates Euclidean distance manually.

Evaluates predictions on the validation set.

Outputs predictions for the test set to KNN_test_predict3.csv.

▶️ How to Run
bash
jupyter notebook KNN.ipynb
Steps performed:

Read KNN_train.csv, KNN_valid.csv, and KNN_test.csv.

Predict labels for validation set (K=50) and compare with ground truth.

Predict labels for test set (K=60) and write to KNN_test_predict3.csv.

🔁 2. K-Means Clustering (K_means.ipynb)
📌 Description
Unsupervised clustering of Iris data using K-Means.

Initializes 3 random centroids and iteratively updates them.

Validates clusters using the validation set.

Labels test set and writes results to K_means_test_predict2.csv.

Visualizes training data in 2D using t-SNE + seaborn scatter plot.

▶️ How to Run
bash
jupyter notebook K_means.ipynb
Steps performed:

Read K_means_train.csv, K_means_valid.csv, and K_means_test.csv.

Randomly initialize centroids and perform K-Means until convergence.

Assign predicted cluster labels to validation/test sets.

Output predictions to K_means_test_predict2.csv.

Visualize clusters using t-SNE.

📊 Sample Output
KNN (Validation Match)
python-repl
Result of KNN: Iris-setosa     Answer from KNN Valid: Iris-setosa
...
K-Means (Validation)
python-repl
validation test: cluster_3 matches original: cluster_1 = invalid
...
t-SNE Visualization
Color-coded 2D visualization of clusters using t-SNE.

📌 Notes
Validation in both approaches helps verify correctness.

K-Means uses cluster labels like cluster_1, cluster_2, etc.

Ensure .csv files are formatted correctly and placed in the working directory.
