
# Eng-Hin_translator

This project implements a Neural Machine Translation (NMT) model for translating English sentences to Hindi using an Encoder-Decoder architecture with Long Short-Term Memory (LSTM) units.

# Overview
The code provided in this repository trains a sequence-to-sequence model using Keras with TensorFlow backend. The dataset used for training is a truncated version of the Hindi-English parallel corpus, focusing on TED talks as the data source.


## Requirements

- Python 3.12
Jupyter Notebook (for running the provided code)
Libraries: 
    NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, Keras

## Data Preprocessing
Loading and cleaning the dataset.
Filtering data from TED talks as the source.
Handling missing values and duplicates.
Text preprocessing steps:
Converting to lowercase.
Removing quotes, special characters, and digits.
Handling Hindi characters.
Adding start and end tokens.

## Model Architecture
The NMT model consists of an Encoder and a Decoder. Key components include:

Embedding layers for input and target sequences.
LSTM layers for both Encoder and Decoder.
Dense layer for final output.
Categorical crossentropy used as the loss function.
RMSprop optimizer.

## Training
The model is trained with the provided training data for a specified number of epochs. The training process involves generating batches of data using a custom data generator.

## Evaluation
The model's performance can be evaluated on a test set. The code includes examples of making predictions on new English sentences and obtaining corresponding Hindi translations.

# Usage
Install the required dependencies.
Run the Jupyter Notebook containing the code.
Results
The model's performance and training/validation loss graphs can be observed through the printed logs and visualizations generated during training

## Saved Model
The trained model is saved as 'nmt_weights.h5'. To load the model, use the provided code.

## Inference
The code includes functions for pre-processing input sequences and generating predictions for new sentences.
  


## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/language-translation.git
   cd language-translation

-- pip install -r requirements.txt

