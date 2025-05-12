# **Wine Quality Classification with SVM and Neural Networks**
This project classifies wine quality into two classes (Good or Bad) using physicochemical properties of wines. Two types of models were implemented: Support Vector Machines (SVM) and Artificial Neural Networks (ANN) .

## **📌 Dataset**
File : WineQT.csv
Features : 11 chemical properties (e.g., alcohol, acidity, sulphates)
Target : Binary classification (quality ≥ 6 → Class 1, else Class 0)

## **🔧 Preprocessing**
No missing values or duplicates.
Selected top features based on correlation with target.
Scaled data for SVM.
Split into train/test sets (70/30).

## **⚙️ Models Used**
**SVM**
Tested with RBF, Linear, and Polynomial kernels.
Best model: Polynomial SVM (C=1, degree=3)
**Neural Network**
Architecture: 4 input → 32 → 16 → 1 output neuron
Activation functions tested: ReLU, Sigmoid, Tanh
Best model: Sigmoid

## **📈 Visualizations**
Correlation matrix, 
Confusion matrices, 
ROC curves, 
Training/validation loss & accuracy curves

## **📊 Results**

| Model             | Test Accuracy | F1 Score | AUC     |
|------------------|---------------|----------|---------|
| Polynomial SVM   | 77.26%        | 0.80     | 0.82    |
| Neural Network   | 74.34%        | 0.76     | 0.79    |
