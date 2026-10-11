# Support Ticket Classification & Prioritization

## Project Overview

This project uses Machine Learning and Natural Language Processing (NLP) to classify customer support tickets into categories and assign priority levels.

The goal is to help support teams organize tickets and identify potentially urgent issues.

## Objectives

* Clean and preprocess ticket text.
* Convert text into numerical features using TF-IDF.
* Classify tickets using Machine Learning.
* Assign High, Medium, and Low priority levels.
* Evaluate the category classification model.
* Test predictions using new support tickets.

## Dataset

**Dataset:** IT Service Ticket Classification Dataset

**Source:** https://www.kaggle.com/datasets/adisongoh/it-service-ticket-classification-dataset

The dataset contains 47,837 records and two columns:

* `Document`: Support ticket text.
* `Topic_group`: Ticket category.

The original dataset does not contain priority labels.

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* TF-IDF Vectorization
* Logistic Regression
* Google Colab

## Project Workflow

1. Load and inspect the dataset.
2. Clean the ticket text.
3. Separate input text and target categories.
4. Split the data into training and testing sets.
5. Convert text into numerical features using TF-IDF.
6. Train a Logistic Regression classification model.
7. Evaluate the model using accuracy, precision, recall, F1-score, and a confusion matrix.
8. Assign ticket priorities using keyword-based rules.
9. Test the system using new ticket messages.

## Priority Assignment

The system uses predefined keyword rules to assign priorities.

* **High:** Urgent or critical issues, such as a server outage.
* **Medium:** Issues containing keywords such as error, failed, or not working.
* **Low:** Tickets that do not match the High or Medium rules.

Priority assignment is rule-based. It is not a separately trained priority prediction model.

## Model Evaluation

The category classification model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion matrix

Refer to the Jupyter Notebook for the actual evaluation results.

## Limitations

The original dataset does not contain verified priority labels. Therefore, priority assignment is based on predefined keyword rules and has not been evaluated against real priority labels.

Keyword-based rules may sometimes assign incorrect priorities. A future improvement would be to use a dataset with genuine priority labels and train a separate priority classification model.

## Conclusion

This project demonstrates Machine Learning-based support ticket classification and rule-based priority assignment. It provides a starting point for helping support teams organize tickets and identify potentially urgent requests.
