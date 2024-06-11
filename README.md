# Introduction to Machine Learning and Data Science
**The Academic Center Ruppin**

**Final Assignment**

## Authors:
- **Matan Shemesh** 
- **Ariel Cohen** 

## Table of Contents:
- [Part 1: Full Training of QDA Classifier](#part-1-full-training-of-qda-classifier)
- [Part 2: Training and Performance Evaluation of Classifier](#part-2-training-and-performance-evaluation-of-classifier)
- [Appendix: Prompts](#appendix-prompts)

## Part 1: Full Training of QDA Classifier

### Introduction
In this task, we trained a QDA (Quadratic Discriminant Analysis) classifier to recognize sign language from images. Solutions from our course's homework notebooks were utilized, with additional functions implemented as needed. Each image was represented as a square matrix and reshaped to the appropriate size. Efficiency was prioritized by writing short and efficient code, with comments and explanations added for complex calculations.

### Calculations and Comparisons
During the calculation, appropriate model values (sigma, inverse sigma, determinant, Gaussian) for each label were computed for use in the estimation calculation. We compared our calculated values (mu_ml, pi_ml, sigma_ml) with those from the sklearn API, noting additional operations performed by the API.

### Results
- **Training Accuracy:** 100%
- **Test Accuracy:** 92.4%
- **Confusion Matrix:** Values only on the main diagonal, indicating correct classifications without misclassifications.
- **Precision and Recall:** Both achieved a score of 1.0 in the training set, indicating perfect classification, but lower scores in the test set.

## Part 2: Training and Performance Evaluation of Classifier

### Introduction
We explored various semantic analysis models on the Huggingface website to choose the appropriate approach. Semantic analysis applies natural language processing (NLP) technologies to interpret text similarly to humans.

### Cross Validation
The `cross_validate` function from `sklearn.model_selection` was used to evaluate model performance on various metrics, returning accuracy percentages for the test and training series. Parameters such as `cv`, `shuffle`, and `random_state` were utilized to ensure consistent results.

### Classifier Testing
We created an array containing all classifiers and ran each separately with the best values found. Computation speed and accuracy were weighed to select the optimal classifier.

### Results
- **KNeighborsClassifier:** Test Accuracy Before: 70.302%, After: 73.434%
- **QuadraticDiscriminantAnalysis:** Test Accuracy Before: 74.068%, After: 74.068%
- **DecisionTreeClassifier:** Test Accuracy Before: 63.940%, After: 68.689%
- **RandomForestClassifier:** Test Accuracy Before: 76.014%, After: 76.015%
- **LinearDiscriminantAnalysis:** Test Accuracy Before: 80.316%, After: 80.487%
- **GaussianNB:** Test Accuracy Before: 70.739%, After: 70.757%

### Graphical Display
A bar graph was created to visualize accuracy for each classifier in the training and test series.

## Conclusions
The changes made to maximize results were detailed for each classifier, demonstrating significant improvements in most cases. The LDA classifier was chosen as the best for our semantic analysis model, with maximized test series accuracy and reduced overfitting.
