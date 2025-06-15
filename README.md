# Breast_Cancer_Diagnosis
Breast Cancer Diagnosis using Neural Networks This project uses neural network models (MLP, Perceptron, BAM, SOM, RBFN) on the Wisconsin dataset for breast cancer classification, clustering, and pattern association. The best MLP model achieved ~98.2% accuracy using Keras with Adam optimizer.

##  🧠 Breast Cancer Diagnosis Using Neural Networks
Early and accurate diagnosis of breast cancer can save lives. This project applies neural network models to the Breast Cancer Wisconsin (Diagnostic) Dataset to classify tumors as malignant or benign. Both supervised and unsupervised learning methods are used for classification, clustering, and associative recall.

## 📑 Table of Contents
1. Dataset Description
2. Preprocessing
3. Exploratory Data Analysis
4. Model Architectures
5. Regularization Techniques
6. Advanced Techniques
7. Model Comparison
8.Results & Conclusion
9. Potential Improvements
10. Installation
11. Contact

## 📂 Dataset Description
Dataset: Breast Cancer Wisconsin (Diagnostic)
Source: UCI Repository via Kaggle
Records: 569
Features: 30 real-valued features from FNA (fine needle aspirates)
Target: Diagnosis — M (malignant) or B (benign)

## 🧹 Preprocessing
Dropped irrelevant columns (ID)
Label encoding: M = 1, B = 0
Handled missing values (median/mode imputation)
Standardized features using StandardScaler
Categorical encoding and scaling

## 📊 Exploratory Data Analysis
Diagnosis distribution: ~62% benign, ~38% malignant
Correlation heatmaps for feature relationships
PCA for visualization
Boxplots and pairplots for feature separability

## 🧠 Model Architectures
Model	Optimizer	Accuracy	Notes
MLP (Keras)	Adam	~98.2%	Best performer, ReLU + Sigmoid, L2 + Dropout
MLP (Keras)	SGD	~95.6%	Slower, more sensitive to LR, good generalization
MLP (Scikit-learn)	Adam (default)	~98.2%	Simpler interface, quick prototyping
Perceptron	N/A	~97.3%	Single-layer, baseline model
BAM (Associative Memory)	N/A	~62.2%	Binary symptom-disease recall model

## 🛡 Regularization Techniques
L1 Regularization: Sparsity & feature selection
L2 Regularization: Stability & generalization
Dropout: Prevents overfitting (rate: 0.3–0.5)
Batch Normalization: Faster and more stable training

## 🚀 Advanced Techniques
###🔸 Self-Organizing Maps (SOM)
Clusters patients into risk groups
Topology-preserving 2D grid visualization
Clear separation between malignant and benign clusters

###🔸 Radial Basis Function Network (RBFN)
Gaussian activation, anomaly detection
Good for identifying rare or borderline cases

###🔸 Bidirectional Associative Memory (BAM)
Learns binary symptom-disease pairs
Can recall input from output and vice versa

## 📊 Model Comparison
Model	Accuracy	Convergence	Generalization	Flexibility
Perceptron	~97.3%	Fast	Low	Low
MLP (sklearn)	~98.2%	Moderate	Good	Medium
MLP (Keras, Adam)	~98.2%	Fast	Excellent	High
MLP (Keras, SGD)	~95.6%	Slow	Good	High
BAM	~62.2%	Slow	Low	Low

## 🏁 Results & Conclusion
Best model: MLP (Keras, Adam) — ~98.2% accuracy
SOMs revealed visually distinct patient clusters
BAM demonstrated pattern association ability
Feature importance: radius_mean, texture_mean, perimeter_mean
Regularization and scaling significantly improved performance

## 🔧 Potential Improvements
Use ensemble models for enhanced prediction
Apply GridSearchCV or Bayesian optimization
Deploy best model as a diagnostic web app
Incorporate time-series data for progression tracking

## 📥 Installation
1. Clone the repository
git clone https://github.com/your-username/breast-cancer-neural-networks.git
cd breast-cancer-neural-networks

2. Install required packages
pip install -r requirements.txt

📧 Contact
Muntaha Nishat
📬 Email: muntahanishat555@gmail.com
🔗 GitHub: github.com/muntaha585
