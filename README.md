# `Portfolio project:` Predicting Heart Failure 

## DESCRIPTION
Cardiovascular diseases (CVDs) are the number one cause of death globally, taking an estimated 17.9 million lives each year, which account for 31% of all deaths worldwide. Approximately 4/5 CVD deaths are due to heart attacks and strokes, and one-third of these deaths occur prematurely in people under 70 years of age. 

Heart failure is a common event caused by CVDs and this dataset contains 11 features that can be used to predict a possible heart disease.

## DATA
Dataset: Heart failure <br>
Source Kaggle URL: https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction/data


1. **Age:** Age of the patient [years]
2. **Sex:** Sex of the patient [M: Male, F: Female]
3. **ChestPainType:** Chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
4. **RestingBP:** Resting blood pressure [mm Hg]
5. **Cholesterol:** Serum cholesterol [mm/dl]
6. **FastingBS:** Fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
7. **RestingECG:** Resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
8. **MaxHR:** Maximum heart rate achieved [Numeric value between 60 and 202]
9. **ExerciseAngina:** Exercise-induced angina [Y: Yes, N: No]
10. **Oldpeak:** Oldpeak = ST [Numeric value measured in depression]
11. **ST_Slope:** The slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
12. **HeartDisease:** Output class [1: heart disease, 0: Normal]

## MODELS 
This work demonstrates the use of classification models: Logistic Regression, Decision Tree, Random Forest, and Support Vector Machine. 

1. **Logistic Regression:**
   - **Type:** Supervised learning algorithm.
   - **Purpose:** Used for binary classification problems (predicting outcomes with two classes).
   - **Model:** It models the probability that an instance belongs to a particular class.
   - **Algorithm:** It uses the logistic function (sigmoid) to transform a linear combination of input features into a value between 0 and 1.

2. **Decision Tree:**
   - **Type:** Supervised learning algorithm.
   - **Purpose:** Used for both classification and regression tasks.
   - **Model:** It makes decisions by recursively splitting the dataset based on the most significant attribute at each step.
   - **Algorithm:** Uses a tree-like graph of decisions to reach a conclusion about the target variable.

3. **Random Forest:**
   - **Type:** Ensemble learning algorithm.
   - **Purpose:** Used for classification and regression tasks, and particularly effective for complex problems.
   - **Model:** It consists of a collection of decision trees, where each tree "votes" on the final prediction.
   - **Algorithm:** The trees are trained on random subsets of the data and features, reducing overfitting and improving generalization.

4. **Support Vector Machine (SVM):**
   - **Type:** Supervised learning algorithm.
   - **Purpose:** Used for classification and regression tasks; particularly effective in high-dimensional spaces.
   - **Model:** It finds a hyperplane that best separates classes in feature space.
   - **Algorithm:** It aims to maximize the margin between different classes, with support vectors defining the hyperplane. SVM can also use kernel functions for nonlinear decision boundaries.

Each of these algorithms has its strengths and weaknesses, and the choice depends on the characteristics of the data and the goals of the analysis.



## HYPERPARAMETER OPTIMSATION
This is an important aspect of fine-tuning machine learning models. 

1. **Logistic Regression:**
   - **Hyperparameters:** Common hyperparameters include regularization strength (lambda or C), which controls the trade-off between fitting the training data well and preventing overfitting.

2. **Decision Tree:**
   - **Hyperparameters:** Decision Trees have hyperparameters like the maximum depth of the tree, minimum samples required to split a node, and the minimum samples required at a leaf node. Tuning these parameters can help control the tree's complexity and prevent overfitting.

3. **Random Forest:**
   - **Hyperparameters:** In addition to the hyperparameters of a single Decision Tree, Random Forests have additional parameters such as the number of trees in the forest and the number of features considered for each split. These parameters influence the ensemble's performance.

4. **Support Vector Machine (SVM):**
   - **Hyperparameters:** SVMs have hyperparameters like the choice of the kernel (linear, polynomial, radial basis function, etc.), the cost parameter (C), and in the case of kernelized SVMs, the kernel-specific parameters. These influence the decision boundary and the model's generalization.

## RESULTS

Comparing & summarising results of the models: Logistic Regression, Decision Tree, Random Forest, and SVM.

- Logistic Regression: Accuracy: 0.88
- Decision Tree: Accuracy: 0.85
- Random Forest: Accuracy: 0.90
- Support Vector Machine: 0.86 

## Summary:
- **Random Forest** achieved the highest overall accuracy (90%) and demonstrated good precision, recall, and F1-Score for both classes. It outperformed the other models across various metrics.

- **Logistic Regression** also performed well with an accuracy of 88% and balanced precision, recall, and F1-Score.

- **Decision Tree** showed slightly lower accuracy compared to Random Forest and Logistic Regression.

- **SVM** performed reasonably well but with a slightly lower accuracy compared to Random Forest and Logistic Regression.

In conclusion, the **Random Forest model** was found to be the most effective.   




