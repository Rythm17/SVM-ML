# PARAMETER OPTIMIZATION SVM
This project demonstrates the use of Nu-Support Vector Classifier (NuSVC) for digit classification using the digits dataset from sklearn. It employs GridSearchCV to optimize hyperparameters and evaluate model performance on a test set. Additionally, it visualizes the convergence of cross-validation accuracy during the search.

## Features
- Dataset: Utilizes the digits dataset from sklearn, which contains images of hand-written digits.
- Model: Implements the NuSVC classifier from scikit-learn for classification.
- Hyperparameter Tuning: Uses GridSearchCV to explore the best combination of parameters (nu, kernel, gamma, degree).
- Convergence Graph: Plots the cross-validation accuracy across iterations to visualize the optimization process.
- Results Export: Saves the optimization results and the convergence graph for further analysis.

## Dependencies
Ensure the following Python packages are installed:

numpy

pandas

matplotlib

scikit-learn

Install them using pip:
```bash
   pip install numpy pandas matplotlib scikit-learn
```

## Usage
Clone the repository:
```bash
   git clone https://github.com/your-username/parameter-optimization-svm.git
```
Navigate to the project directory:
```bash
   cd parameter-optimization-svm
```
Run the script:
```bash
   python svm_parameter_optimization.py
```
## Outputs
Optimal Hyperparameters: The best combination of NuSVC hyperparameters is identified and saved to a CSV file named optimized_svm_results.csv.

Convergence Graph: A plot of cross-validation accuracy across iterations is generated and saved as optimization_convergence_graph.png.

## Code Overview
1. Dataset: The digits dataset is used, containing features (data) and labels (target).
2. GridSearchCV:
   a. Parameter grid:
      ```python
     grid_parameters = {
    'nu': [0.1, 0.5, 0.9],
    'kernel': ['linear', 'poly', 'rbf', 'sigmoid'],
    'gamma': ['scale', 'auto'],
    'degree': [2, 3, 4],
     }
      ```
3. 5-fold cross-validation is used to find the optimal parameters.
4. Evaluation:
   a. Cross-validation accuracy and test set accuracy are calculated and saved.




