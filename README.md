# Fake News Detection README

## Introduction
This repository contains code for detecting fake news using machine learning models, specifically Multinomial Naive Bayes (MNB) and Gaussian Naive Bayes (GNB). The models are trained on a dataset consisting of news articles labeled as either fake or real.

## Dataset
The dataset used for training and evaluation is split into three parts: training, validation, and test sets. It includes features such as the text of the news articles and labels indicating whether each article is fake or real.

### File Structure
- `train.csv`: Training dataset containing labeled news articles.
- `val.csv`: Validation dataset for evaluating model performance during training.
- `test.csv`: Test dataset for final evaluation of model performance.

## Code Structure
The code is organized into several sections:

### Data Preprocessing
- **Data Cleaning**: The text data is preprocessed to remove noise and irrelevant information, including expanding contractions, removing URLs, tokenizing, lowercasing, removing punctuation, lemmatization, and stemming.
- **Feature Engineering**: Text data is transformed into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency) and Count Vectorization.

### Model Training
- **Multinomial Naive Bayes (MNB)**: Implementation of the MNB model using the `MultinomialNB` class from the `sklearn` package. Hyperparameter tuning is performed to optimize model performance.
- **Gaussian Naive Bayes (GNB)**: Implementation of the GNB model using the `GaussianNB` class from the `sklearn` package. Hyperparameter tuning is performed to optimize model performance.

### Evaluation
- Model performance is evaluated on the validation and test sets using accuracy as the evaluation metric. Both MNB and GNB models are evaluated using TF-IDF and Count Vectorization representations of the text data.

## Instructions for Use
1. **Dataset Preparation**: Ensure that the `train.csv`, `val.csv`, and `test.csv` files are available in the repository.
2. **Environment Setup**: Set up the Python environment with necessary dependencies. This can be achieved using a virtual environment or by installing dependencies directly.
3. **Data Preprocessing**: Run the data preprocessing script to clean and transform the text data into numerical features.
4. **Model Training**: Train the MNB and GNB models using the preprocessed data. Hyperparameter tuning can be performed to optimize model performance.
5. **Evaluation**: Evaluate the trained models on the validation and test sets to assess their performance using accuracy as the evaluation metric.

## Dependencies
- pandas
- scikit-learn
- matplotlib
- seaborn
- numpy

## Contributors
- [Your Name]

## License
This project is licensed under the [MIT License](LICENSE).
