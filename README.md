# SVM Optimization on Dry Bean Dataset

This project demonstrates the optimization of Support Vector Machine (SVM) on the Dry Bean dataset obtained from the UCI Machine Learning Repository. The dataset contains instances of seven different varieties of dry beans, with 16 features describing each instance.

## Dataset

The Dry Bean dataset consists of 13611 instances, with each instance having 16 features. The dataset is divided into 10 different samples for training and testing.

## Implementation

### Loading the Dataset

The dataset is loaded from a CSV file using the pandas library.

### Splitting the Dataset

The dataset is split into training and testing sets with a 70-30 ratio, repeated 10 times to get 10 different samples.

### Optimizing SVM

SVM is optimized for each sample using cross-validation with 100 iterations. GridSearchCV is used to find the best hyperparameters.

### Recording Results

The best parameters and accuracies are recorded for each sample. The sample with maximum accuracy is identified.
| Sample | Best Accuracy | Best Kernel | Best Nu | Best Epsilon |
|--------|---------------|-------------|---------|--------------|
| 0      | 0.35          | linear      | 4.03    | 1.98         |
| 1      | 0.47          | poly        | 6.81    | 0.76         |
| 2      | 0.39          | poly        | 8.59    | 0.99         |
| 3      | 0.53          | poly        | 2.37    | 0.81         |
| 4      | 0.59          | linear      | 5.21    | 0.45         |
| 5      | 0.59          | linear      | 3.90    | 3.46         |
| 6      | 0.41          | linear      | 4.17    | 0.79         |
| 7      | 0.34          | linear      | 1.23    | 8.34         |
| 8      | 0.53          | poly        | 9.90    | 8.39         |
| 9      | 0.53          | linear      | 1.83    | 0.66         |

### Convergence Graph

A convergence graph is plotted for the sample with the maximum accuracy, showing how the training and testing accuracies change over iterations during the optimization process.

## Files Included

- `dry_bean_data.csv`: CSV file containing the Dry Bean dataset.
- `parameter_optimization.ipynb`: Jupyter Notebook containing the Python code for the project.
- `README.md`: This README file providing an overview of the project.

## Requirements

- Python 3.x
- Required libraries: pandas, scikit-learn, matplotlib

## Acknowledgments

- UCI Machine Learning Repository for providing the Dry Bean dataset.
- Scikit-learn and pandas libraries for their functionalities in data preprocessing and machine learning.
