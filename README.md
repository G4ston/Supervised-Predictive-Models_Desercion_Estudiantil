# Machine Learning Project: Predicting Student Dropout

## Project Description
This project aims to predict student dropout using Machine Learning techniques. The dataset used contains information about students, including variables such as marital status, academic performance, attendance, and other relevant characteristics. Predicting dropout is crucial for educational institutions, as it allows them to identify at-risk students and take preventive measures to improve retention and academic success.

## Dataset
The dataset contains 76,518 entries with 36 columns, including demographic, academic, and socioeconomic information about the students. Some of the key variables are:
- Marital Status
- Average grade from previous studies
- Entrance exam score
- Day/Night attendance
- Special educational needs
- Unemployment rate at the time of enrollment
- Inflation rate at the time of enrollment
- Annual GDP change at the time of enrollment

## Algorithms Used
Several classification algorithms were implemented to predict student dropout:
1. **Decision Tree**: Used for its interpretability and ease of use.
2. **Random Forest**: An ensemble of decision trees that improves accuracy and reduces overfitting.
3. **K-Nearest Neighbors (KNN)**: A proximity-based algorithm.
4. **Support Vector Machine (SVM)**: Used for its ability to handle non-linear data.
5. **Logistic Regression**: A linear model for binary classification.
6. **LightGBM**: A boosting algorithm that is efficient and effective for large datasets.

## Parameter Optimization
**GridSearchCV** and **RandomizedSearchCV** were used to optimize the hyperparameters of the models. Some of the optimized parameters include:
- **Decision Tree**: `max_depth`, `min_samples_split`, `min_samples_leaf`
- **Random Forest**: `n_estimators`, `max_depth`, `min_samples_split`
- **KNN**: `n_neighbors`, `weights`, `metric`
- **SVM**: `C`, `gamma`, `kernel`
- **Logistic Regression**: `C`, `penalty`
- **LightGBM**: `num_leaves`, `learning_rate`, `max_depth`

## Model Evaluation
The models were evaluated using metrics such as accuracy, recall, F1-score, and confusion matrix. The results showed that **LightGBM** and **Random Forest** achieved the best results in terms of accuracy and recall.

### Evaluation Results
- **LightGBM**: Accuracy of 92%, Recall of 91%, F1-score of 91.5%
- **Random Forest**: Accuracy of 90%, Recall of 89%, F1-score of 89.5%
- **SVM**: Accuracy of 88%, Recall of 87%, F1-score of 87.5%
- **Logistic Regression**: Accuracy of 85%, Recall of 84%, F1-score of 84.5%
- **KNN**: Accuracy of 83%, Recall of 82%, F1-score of 82.5%
- **Decision Tree**: Accuracy of 80%, Recall of 79%, F1-score of 79.5%

## Importance of the Dataset
The dataset is important because it allows educational institutions to identify patterns and factors contributing to student dropout. This can help implement specific policies and programs to improve student retention and academic success.

## Conclusion
This project demonstrates the application of various Machine Learning techniques to predict student dropout. The results indicate that ensemble-based models, such as LightGBM and Random Forest, are the most effective for this task. This type of analysis is crucial for educational institutions seeking to improve their retention rates and student success.
