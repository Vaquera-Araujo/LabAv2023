# Exploring Exoplanets with Python

The goal of this project is to use data science techniques to analyze the information obtained by the Kepler satellite in its search for exoplanets: planets that orbit a star different than the Sun. Planets are defined as objects that, in addition to orbiting a star, are massive enough to be rounded by their own gravity, but not massive enough to cause internal thermonuclear fusion and become a star. Another requirement for an object to be considered as planet is that it must clear the region around its orbit of other objects such as asteroids, dust, and other visible inetrestellar material. In this project we apply data science techniques to describe the statistical properties of the objects detected by the Kepler satellite, we show that Kepler's third law governing planetary motion in our solar system is valid for exoplanets, and we use machine learning supervised algoritms to classify if an object is an exoplanet or a false positive, trying to reproduce the disposition of the object that is included in the database used. To achieve this, we analyze the NASA exoplanet dataset using different classification algorithms, and evaluate their performance in terms of precision, accuracy and recall. Finally, we use an unsupervised algoritm to classify the objects of interest with respect to their size and period.

## Exploratory Analysis and data Visualization

- Dataframe Cleanning and Filtering
- Estimators of Location, Variability and Bias
- Frequency Table
- Visualization of Numerical Data 


[kepler_exploratory_analysis_and_data_visualization.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Introduction%20to%20Data%20Science%20and%20Machine%20Learning/Kepler/kepler_exploratory_analysis_and_data_visualization.ipynb)

Challenge: Repeat The Analysis for the Period.

## Central Limit Theorem
- Illustration for the  Central Limit Theorem
- Bootstrap
- Standard Error
- Confidence Intervals

[kepler_central_limit_theorem.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Introduction%20to%20Data%20Science%20and%20Machine%20Learning/Kepler/kepler_central_limit_theorem.ipynb)

Challenge: Repeat The Analysis for the Period.

## Analysis of the Categorical Variables and A/B Tests
- Barplots and Violinplots
- A/B tests
- Null Hypothesis and Alternative Hypothesis
- p-value
- Variance test
- t Test

[kepler_categorical_variables_t_test.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Introduction%20to%20Data%20Science%20and%20Machine%20Learning/Kepler/kepler_categorical_variables_t_test.ipynb)

Challenge: Perform a Permutation Test to confirm the results.

## Kepler's Third Law From a Multiple Linear Regression
- Linear Regression
- Other Supervised Algorithms for Regression
- Overfitting
- Gravitational Constant Estimation

[kepler_linear.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Introduction%20to%20Data%20Science%20and%20Machine%20Learning/Kepler/kepler_linear.ipynb)

Challenge: Modify the Parameters of the single neuron and try to obtain a better model.

## Machine Learning: Supervised Classification Algorithms
- Logistic Regression
- Naïve Bayes
- Support Vector Machine
- Decision Trees
- Random Forest
- Multi-layer Perceptron
- Artificial Neural Network

[kepler_supervised_classification.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Introduction%20to%20Data%20Science%20and%20Machine%20Learning/Kepler/kepler_supervised_classification.ipynb)
  
Challenge: Modify the Parameters of the different classifiers and try to obtain a better model.

## Machine Learning: Unsupervised Classification
- K-means
- Elbow Method

[kepler_unsupervised_classification.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Introduction%20to%20Data%20Science%20and%20Machine%20Learning/Kepler/kepler_unsupervised_classification.ipynb) 

Challenge: Repeat The Analysis for two different variables.
