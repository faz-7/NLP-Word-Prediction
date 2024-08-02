# Word Prediction and POS

## Overview
This repository contains the implementation of a Natural Language Processing (NLP) project focused on text processing, n-gram modeling, and part-of-speech tagging using the Hazm library for Persian text.

## Table of Contents
- [Installation](#installation)
- [Libraries Used](#libraries-used)
- [Data Preprocessing](#data-preprocessing)
- [N-gram Language Model](#n-gram-language-model)
- [Perplexity Calculation](#perplexity-calculation)
- [Word Prediction](#word-prediction)
- [POS Tagging](#pos-tagging)
- [Usage](#usage)
- [Conclusion](#conclusion)

## Installation
To run the code, ensure you have the following libraries installed:

```bash
pip install pandas hazm nltk
```

## Libraries Used
- **pandas**: For data manipulation and analysis.
- **hazm**: A Python library for processing Persian text.
- **nltk**: The Natural Language Toolkit for various NLP tasks.

## Data Preprocessing
The data is read from a CSV file containing comments. The preprocessing steps include:
- Tokenizing comments into sentences.
- Removing punctuation and extra spaces.
- Adding start and end tokens for n-gram modeling.
- Replacing singleton words with `<UNK>`.

## N-gram Language Model
The project implements n-gram models (unigrams, bigrams, trigrams) to predict the next word in a sequence based on the context provided by previous words.

## Perplexity Calculation
Perplexity is calculated for given sentences to evaluate the model's performance.

## Word Prediction
The model suggests the next words based on the trained n-gram probabilities. It also handles out-of-vocabulary words.

## POS Tagging
Part-of-speech tagging is performed on the tokenized sentences using a pre-trained POS tagger.

## Usage
1. Place your `digikala_comment.csv` file in the appropriate directory.
2. Run the script to preprocess the data, train the n-gram models, and perform predictions and tagging.
3. Check the output for suggested words and their perplexities.

## Conclusion
This project demonstrates fundamental NLP techniques applied to Persian text, including data preprocessing, language modeling, word prediction, and POS tagging. The methods can be further extended for more complex NLP tasks.
