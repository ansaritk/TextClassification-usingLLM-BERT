# IMDB Text Classification Program
This project is a machine learning solution built to classify IMDB movie reviews by sentiment, categorizing reviews as positive or negative. Using the Hugging Face transformers library and pre-trained NLP models, this program demonstrates how to perform binary text classification through transfer learning.

## Key Features
* Sentiment Analysis: Classifies movie reviews as positive or negative based on their text content.
* Fine-Tuned Transformer Models: Leverages pre-trained transformer model - BERT, from the Hugging Face transformers library for improved accuracy.
* Efficient Data Handling: Uses the Hugging Face datasets library to efficiently load, shuffle, and split the IMDB dataset for training and evaluation.
* Metrics Tracking: Computes accuracy to evaluate model performance, with options for custom metric integration.

## How It Works
1) Data Encoding: IMDB reviews are tokenized and encoded to be compatible with transformer models.
2) Model Training: Using Trainer with a specified compute_metrics function, the model trains on the IMDB dataset's labeled reviews.
3) Evaluation: After training, the model evaluates itself on a separate validation set, outputting accuracy.

## Prerequisites
Python 3.x
Hugging Face transformers library
Datasets (IMDB) compatible with Hugging Face datasets
PyTorch or TensorFlow backend (depending on the model used)

## How to use
1) Clone the repository:
git clone https://github.com/ansaritk/TextClassificationUsingLLM-BERT.git
2) Install dependencies:
pip install -r requirements.txt
3) Run the training script to fine-tune the transformer model:
python imdb_text_classification.py

## Applications
* Customer Sentiment Analysis: Can be adapted to analyze customer reviews and feedback in various industries.
* Market Research: Helps understand consumer sentiments in media, e-commerce, and beyond.
* Content Moderation: Assists in filtering content based on positive or negative sentiment.
## Future Enhancements
* Fine-tuning for Multiclass Classification: Extending to categorize more nuanced sentiments beyond binary classification.
* Support for Real-time Sentiment Prediction: Integrate with web applications for real-time analysis.
