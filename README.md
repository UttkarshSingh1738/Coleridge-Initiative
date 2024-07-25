# Coleridge Initiative
https://www.kaggle.com/c/coleridgeinitiative-show-us-the-data
Can natural language processing find the hidden-in-plain-sight data citations? Can machine learning find the link between the words used in research articles and the data referenced in the article?

Natural Language Processing (NLP) to automate the discovery of how scientific data are referenced in publications.

This repository contains various scripts for analyzing and classifying scientific data citations in publications using Natural Language Processing (NLP) and machine learning. The goal is to explore how NLP can uncover hidden data citations in research articles and assess the relationships between textual data and referenced data.

## Project Structure

### Folders

- **train/**  
  Contains sample training data for the models. The full dataset can be downloaded from [Kaggle](https://www.kaggle.com/c/coleridgeinitiative-show-us-the-data).

- **test/**  
  Contains sample test data for the models. For the complete dataset, refer to [Kaggle](https://www.kaggle.com/c/coleridgeinitiative-show-us-the-data).

- **nlp_model/**  
  Generated by `bert_named_entity_recognition.ipynb`. This folder includes files and outputs from the BERT-based Named Entity Recognition model.

### Notebooks

- **bert_named_entity_recognition.ipynb**  
  Utilizes the BERT-base-multilingual language model for Named Entity Recognition (NER). This script processes text data to identify and categorize named entities.

- **multi_model_eval.ipynb**  
  Performs a multi-modal evaluation using various models. It includes vectorization using Doc2Vec and BERT-base-uncased, followed by classification using logistic regression, random forest, naive bayes, and SVM.

- **tf-idf_random_forest_classification.ipynb**  
  Implements TF-IDF vectorization to transform publication texts into feature vectors, which are then classified using a Random Forest classifier.

- **word2vec_data_analysis.ipynb**  
  Applies Word2Vec for exploratory data analysis. It finds similar words, common terms, and performs other analyses to gain insights into the text data.
