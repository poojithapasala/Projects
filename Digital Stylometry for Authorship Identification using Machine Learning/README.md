# Overview of Project:
The task is to determine if two given spans of text were written by the same author. This is a binary classification problem where the documents are labeled as 0 for "not the same author" and 1 for "same author".This project leverages BERT embeddings and TF-IDF features, combined with a linear classifier to classify authorship in text data using K-fold cross-validation.

#   Dependencies:
Install the below dependencies before executing the main code.
```markdown
pandas==1.5.3
scikit-learn==1.0.2
torch==1.12.0
transformers==4.27.0
datasets==2.11.0
nltk==3.7
numpy==1.24.2
matplotlib==3.6.3
```
# Install dependencies
```markdown
pip install -r requirements.txt
```

## Repo Contents:
- The `train.csv` and `test.csv` files are downloaded from the Kaggle competition board.
- The `requirements.txt` file includes all the dependencies necessary for the code.  
####   _scripts:_
- `Code_BERT.py`: The main script that utilizes BERT embeddings and TF-IDF features, combined with a linear classifier, to classify authorship in text data using K-fold cross-validation, providing an average F1 score and generating the final submission file.
- `Code_Logistic_reg.py`: This script which was previously used, combines TF-IDF vectorization and logistic regression with GridSearch-based hyperparameter tuning to optimize and streamline authorship prediction.
#### _images:_
- `EDA_Text_span_length.png`: The plot for text span lengths displays the distribution of text lengths in both the training and test datasets, allowing for a comparison of how the number of characters varies across the datasets.
- `EDA_Train_data_Labels.png`: The plot for train data labels visualizes the distribution of the target labels (same author vs. different author) in the training dataset, highlighting the class imbalance between the two categories.  
#### output
- `submission.csv`: Submission file for the BERT model.
- `submission_logistic_reg.csv`: The previous submission file for the logistic regression model.

## Reproducibility
- Install the dependencies by executing the `requirements.txt` file in your terminal.
- Run `Code_BERT.py` to obtain the results, including the average F1 score.

## F1 scores:
The F1 score achieved on 80% of the test data on the Kaggle leaderboard :
 -  BERT model                - 0.57510
 -  Logistic Regression model - 0.51626
