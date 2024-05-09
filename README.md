# Text_Generation_using_LSTM
Text Generation using LSTM
This repository contains code for generating text using LSTM (Long Short-Term Memory) neural networks trained on a book from Project Gutenberg.

Setup
To run the code, follow these steps:

Clone the repository:
bash
Copy code
git clone https://github.com/your_username/your_repository.git
cd your_repository
Install the required dependencies:
bash
Copy code
pip install tensorflow keras numpy
Usage
Download the text file from Project Gutenberg:
bash
Copy code
wget https://www.gutenberg.org/files/1661/1661-0.txt -O book.txt
Run the Python script:
bash
Copy code
python text_generation.py
Description
This script utilizes TensorFlow and Keras to train an LSTM model for text generation. Here's a brief overview of the process:

The text file is downloaded and read. It is then converted to lowercase and split into sentences.
Tokenization is performed using Keras Tokenizer, and sequences of tokens are generated.
Padding is applied to sequences to make them uniform in length.
The model architecture is defined using Keras Sequential API. It consists of an Embedding layer, a Bidirectional LSTM layer, and a Dense output layer.
The model is compiled with the Adam optimizer and trained on the input sequences and labels.
After training, text generation is performed using a seed text. The model predicts the next word in the sequence, and the process is repeated to generate a specified number of words.
Results
The trained model demonstrates the ability to generate coherent text based on the input seed. Example output:

css
Copy code
I could not help laughing at the ease with which he explained his process of deduction the manager locked the door and ordered the chicken to be sliced and served in a piquant sauce of madeira and vinegar the sergeant lapped it up the man at the table pointed and whispered something to himself
Feel free to experiment with different seed texts and generate longer sequences by adjusting the next_words parameter in the script.

Acknowledgments
Project Gutenberg for providing public domain texts.
TensorFlow and Keras teams for their contributions to deep learning frameworks.
