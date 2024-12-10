
# Next Word Predictor using LSTM

This project demonstrates a text-generation model using a Long Short-Term Memory (LSTM) neural network. The model is trained on a given corpus and generates new text based on learned patterns, providing a foundation for applications like predictive text and creative writing tools.


## Features

Generates text based on a given seed phrase.

Uses an LSTM-based architecture for sequential data processing.

Handles custom datasets with tokenization and padding.

Supports adjustable vocabulary size, embedding dimensions, and model depth.
## Technologies Used

Programming Language: Python
Deep Learning Framework: TensorFlow/Keras

Libraries:

    numpy
    time 
    keras.preprocessing
## How it Works

1. Preprocessing:

The input text is tokenized into sequences of integers using the Tokenizer from Keras.
Sequences are padded to ensure consistent input length.

2. Model Architecture:

An Embedding layer converts integer sequences to dense vector representations.
An LSTM layer learns sequential dependencies in the text.
A Dense layer with a softmax activation predicts the next word.

3. Training:

The model is trained using the categorical cross-entropy loss and the Adam optimizer.
It predicts the next word in a sequence, iteratively building complete sentences.

4. Text Generation:

Given a seed phrase, the model predicts the next word and appends it to the input.
This process continues iteratively, creating a sequence of words
## Installation and Setup

Prerequisites

Ensure you have the following installed:

    Python 3.7+
    TensorFlow 2.0+
    NumPy

Steps

1. Clone the repository:

    git clone https://github.com/your-username/text-generation-lstm.git
    cd text-generation-lstm

2. Install required packages:

    pip install -r requirements.txt

3. Add your training data in the script or load it from a file.

4. Run the script to train the model:

    python train_text_generator.py
    
5. Generate text using:

    python generate_text.py
## Sample Output

Given the seed text "Aditya", the model generates:

    Aditya was a young software developer working at a modest IT firm in Pune...

## Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request.
## License

This project is licensed under the MIT License. See the LICENSE file for more details.