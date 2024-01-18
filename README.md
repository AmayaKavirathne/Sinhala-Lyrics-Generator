# Sinhala-Song-Lyrics-Generator

This repository contains code for generating new Sinhala song lyrics using a Long Short-Term Memory (LSTM) neural network. The model is trained on a dataset of Sinhala song lyrics obtained from KAggle dataset 'Genius Song Lyrics'.

# Prerequisites
Make sure you have the following libraries installed:

- pandas
- numpy
- seaborn
- matplotlib
- wordcloud
- string
- os
- tensorflow
- keras

# Usage
## Clone the repository:

git clone https://github.com/your-username/sinhala-lyrics-generator.git
cd sinhala-lyrics-generator

## Run the provided Python script:

python sinhala_lyrics_generator.py

This script includes the following sections:

 ### Data Loading and Preprocessing: 
 Reads the dataset from 'output.csv', removes unnecessary columns, and filters the dataset for Sinhala songs.

### Data Visualization: 
Analyzes the word count distribution of the Sinhala songs and removes records with more than 600 words.

### Tokenization: 
Tokenizes the lyrics and prepares input sequences for the LSTM model.

### LSTM Model Development: 
Builds a Bidirectional LSTM model for training on the Sinhala song lyrics. The model is trained for 10 epochs.

### Accuracy Plotting: 
Plots the training accuracy over epochs.

### Lyrics Generation:
Defines a function to generate new Sinhala song lyrics based on a seed text.

# Results
The LSTM model is trained on the provided dataset, and you can use the complete_this_song function to generate new Sinhala song lyrics by providing a seed text and the desired number of words.


complete_this_song("අහස නිල් පාටයි", 40)

Output: 'අහස නිල් පාටයි ඉන්න තනලා තනලා ඉරේ නිව නිව දමා අරන් අරන් සිහිල් සිහිල් සිහිල්...'


