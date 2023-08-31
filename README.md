# Calibrated Classifier: Is Logistic Regression Always Well Calibrated?

## Summary

This project aims to investigate the calibration of different classifiers, particularly focusing on the performance of logistic regression on non-linear and generative datasets. The primary goal is to assess whether logistic regression's calibration remains superior across various datasets or if its performance is contingent on the linear separability of the data.

## Rationale

The [Scikit-learn documentation example](https://scikit-learn.org/stable/auto_examples/calibration/plot_calibration_curve.html#sphx-glr-auto-examples-calibration-plot-calibration-curve-py) discusses the calibration of classifiers, comparing logistic regression against non-linear and generative classifiers. The example highlights that logistic regression often exhibits better performance in terms of the Brier score. However, this advantage is heavily influenced by the linear separability of the data. In scenarios where the data is not linearly separable, both performance metrics and calibration may not meet desired levels.

## Methodology

1. **Dataset:** The Kaggle "Give Me Some Credit" dataset, known for its lack of linear separability, will be used to train and evaluate different classifiers.

2. **Calibration Evaluation:** The Brier score, defined as the mean squared error of binary predictions, will be used to assess the calibration of the classifiers.

3. **Platt Scaling:** To explore the potential for improving calibration, Platt scaling will be applied to each tested classifier.

## Conclusions

This project delves into the critical aspect of classifier calibration, emphasizing the significance of reliable probability estimates that can serve as confidence indicators.

Key Findings:

- The assumption that linear models or models optimizing the log loss cost function always exhibit excellent calibration is not universally applicable.
- Calibration quality is intricately tied to overall model performance, making it imperative to consider both aspects in tandem.

By shedding light on the relationship between classifier type, calibration, and model performance, this project contributes to a better understanding of how different classifiers behave in real-world scenarios.





## Setup and Reproduction

To reproduce the analysis and results of this project, follow these steps:

1. **Clone the Repository:** Start by cloning this repository to your local machine using the following command:





2. **Environment Setup:** Make sure you have Python 3.x installed on your system. It's recommended to create a virtual environment to manage dependencies. You can create a virtual environment using `venv` or `conda`.

3. **Install Dependencies:** Navigate to the project directory and install the required Python packages by running:

