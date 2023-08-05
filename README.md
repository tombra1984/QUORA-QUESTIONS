# mini-project-V
PROJECT DESCRIPTION

IDENTIFYING DUPLICATE QUESTIONS

Over 100 million people visit Quora every month, and it's no surprise that many people ask similar (or the same) questions. Various questions with the same intent can cause people to spend extra time searching for the best answer to their question, and results in members answering multiple versions of the same question. Quora uses random forest to identify duplicated questions to provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.

This project looks at using other classifiers to identify the duplicated questions and the performance of the classifier at performing the task.The models built will automatically identify and label questions as duplicate or not.

A variety of classifers were used ranging from logistic regression to ensemble methods. However, it was observed that the logistic regression model was the best performing classifier. Although it was a very tight contest as the XGBoost classifier also performed almost at par with the logistic regression model as seen below. 


REGRESSION MODEL CLASSIFICATION REPORT
![classification report](https://github.com/tombra1984/QUORA-QUESTIONS/assets/127909963/eaa18beb-f14d-45f9-acad-b9c61e4b6b65)





![logistic classification report](https://github.com/tombra1984/QUORA-QUESTIONS/assets/127909963/f3a4ba9e-0a50-43fd-97ae-7eb45bc75521)


In order to determine which model performed better, these factors were considered:

1. Precision: Logistic Regression model had higher precision for class 0 (0.72 vs. 0.73), indicating a better ability to correctly identify non-duplicate instances. While the XGBoost Model  had higher precision for class 1 (0.70 vs. 0.65), indicating a better ability to correctly identify duplicate instances.

2. Recall:  Logistic Regression model has higher recall for class 0 (0.88 vs. 0.83), indicating a better ability to correctly capture actual non-duplicate instances. While the XGBoost Model  has higher recall for class 1 (0.45 vs. 0.52), indicating a better ability to correctly capture actual duplicate instances.

3. F1-score:  Logistic Regression model has a higher F1-score for both class 0 (0.79 vs. 0.78) and class 1 (0.54 vs. 0.58). The F1-score balances precision and recall, and higher values indicate a better overall performance.

4. Accuracy: Both models have the same accuracy (0.71), which measures the overall correctness of the predictions across all classes.

Considering the precision, recall, and F1-score, Logistic Regression model appeared to perform slightly better than XGBoost classification model. It achieves higher scores for both classes and has a better balance between precision and recall. 


### Data

The labeled dataset can be downloaded from [here](https://drive.google.com/file/d/19iWVGLBi7edqybybam56bt2Zy7vpf1Xc/view?usp=sharing).
