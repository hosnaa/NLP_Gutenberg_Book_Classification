# NLP_Gutenberg_Book_Classification

## Problem Overview
In this task, we are using semantically-close books from the Gutenberg project and we aim to classify text segments to its corresponding book name.
## Libraries and Dependencies
*The versions are the defaults set by colaB*
- Python
- NLTK
- SKlearn
- Eli5
- Lime
- Matplotlib
- Jupyter/spider/colaB 
## Output Example:
An example for the output of eli5 for the top 10 words of 5 books:
![image](https://user-images.githubusercontent.com/36189572/149307432-481069e1-2c85-481e-bce4-8dc01b52d5a6.png)
## Steps:
1. We start by 5 books that are semantically close to each other. 
2. Extract 200 samples from each book, each sample comprises 100 words. 
3. Data preprocessing is performed on these segments: 
- Tokenization
- Punctuation and stop words Removal
- Lowercasing
- Lemmatization
4. Feature Engineering on the clean data from (3):
- Bag of Words
- TF-IDF
5. Splitting the data into train/test splits (80/20) and 10 fold cross validation.
6. Modelling for TF-IDF features:
- Decision Tree
- KNN
- SVM
- Logistic Regression
7. Evaluation: Accuracy, Bias-Variance tradeoff
8. Error Analysis for Misclassified segments: 
- eli5
- Lime
9. Insights, Analysis then modify some hyperparameters *(e.g. number of words per segment)* and retrain.

