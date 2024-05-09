# Text_Generation_using_LSTM

## This repository contains code for generating text using LSTM (Long Short-Term Memory) neural networks trained on a book from Project Gutenberg.

# Description
 This script utilizes TensorFlow and Keras to train an LSTM model for text generation. Here's a brief overview of the process:

### Data Preprocessing: 
 The code starts by downloading a text file from Project Gutenberg and preprocessing it. This involves converting the text to lowercase and splitting it into sentences.
### Tokenization:
  It utilizes the Tokenizer class from Keras to tokenize the sentences into sequences of integers. These sequences represent the words in the text.
 ### Padding:
  The sequences are padded to make them uniform in length. This is necessary for feeding the data into the neural network.
 ### Model Architecture:
  The LSTM model architecture is defined using the Sequential API from Keras. It consists of an Embedding layer, a Bidirectional LSTM layer, and a Dense     output layer.
 ### Model Training: 
  The model is compiled with the Adam optimizer and trained on the input sequences and labels. It is trained for a specified number of epochs.
 ### Text Generation: 
  After training, the model is used to generate text. It takes a seed text as input and predicts the next word in the sequence. This process is repeated to generate a specified number of words.
 ### Results:
  The generated text demonstrates the model's ability to produce coherent sequences of words based on the input seed text.
