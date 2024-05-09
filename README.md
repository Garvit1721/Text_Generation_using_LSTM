# Text_Generation_using_LSTM

###This repository contains code for generating text using LSTM (Long Short-Term Memory) neural networks trained on a book from Project Gutenberg.

#Description
This script utilizes TensorFlow and Keras to train an LSTM model for text generation. Here's a brief overview of the process:

The text file is downloaded and read. It is then converted to lowercase and split into sentences.
Tokenization is performed using Keras Tokenizer, and sequences of tokens are generated.
Padding is applied to sequences to make them uniform in length.
The model architecture is defined using Keras Sequential API. It consists of an Embedding layer, a Bidirectional LSTM layer, and a Dense output layer.
The model is compiled with the Adam optimizer and trained on the input sequences and labels.
After training, text generation is performed using a seed text. The model predicts the next word in the sequence, and the process is repeated to generate a specified number of words.
