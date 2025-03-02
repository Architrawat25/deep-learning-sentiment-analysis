# Deep Learning-based Sentiment Analysis 
## Fine-tuning roBERTa on amazon beauty product reviews

## Overview

This project explores sentiment analysis of Amazon beauty product reviews by fine-tuning the RoBERTa model. As a baseline comparison, a rule-based approach was applied to understand the difference in performance between traditional sentiment analysis methods and deep learning models. 

## Objective

- Classify product reviews into **Positive**, **Negative**, or **Neutral** sentiments.
- Use rule-based technique (VADER) as a baseline to understand the performance gap between rule-based and deep learning approaches.
- Compare how well RoBERTa's sentiment predictions align with the product ratings associated with the reviews.
- Visualise the correlation between predictions and product ratings.

## Dataset

The dataset is sourced from [Amazon Reviews 2023](https://amazon-reviews-2023.github.io/). It contains customer reviews and their corresponding product ratings (0-5) for beauty products.

## Approach

1. **Preprocessing**: Basic text cleaning like lowercasing, removing special characters, and tokenization to prepare the text data.
2. **Rule-Based Approach (VADER)**: VADER (**Valence Aware Dictionary and sEntiment Reasoner**) is a simple but effective sentiment analysis tool that uses pre-defined word lists with sentiment scores. It’s fast but often struggles with context and sarcasm.
3. **Deep Learning Approach (RoBERTa)**: I fine-tuned the **RoBERTa** transformer model on the dataset to classify the sentiments more accurately.
4. **Comparison**: The sentiment classifications from both methods were compared with the product ratings to understand which method better reflects customer satisfaction.
5. **Visualisation**: Plots were generated to visualise how well each model’s predictions aligned with the numerical ratings.

## Why This Project?

I wanted to see how much of an improvement deep learning models like RoBERTa offer over traditional methods like VADER — especially when applied to product reviews, where sentiment isn't always straightforward.

## Dependencies

- Python
- Transformers
- Scikit-learn
- Matplotlib, Seaborn
- Pandas
- NLTK (for VADER)

## Results

- The **RoBERTa** model consistently provided more accurate sentiment classifications compared to VADER.
- Visualisations showed that **RoBERTa's** predictions aligned more closely with user ratings, especially in distinguishing neutral and mixed reviews.


## Author

Archit Rawat

## License

This project is licensed under the MIT License.

