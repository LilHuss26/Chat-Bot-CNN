# Chat-Bot-CNN

## Overview

This repository contains Python code for training a chatbot using a neural network. The chatbot is designed to interact with users, understand their queries, and provide relevant responses based on a set of defined intents.

## Liberaries

* nltk
* tensorflow
* random
* json
* pickle
* time

## Data Preparation

1. **Intents File:** A JSON file named `intents.json` is required, containing a list of intents with their corresponding patterns and responses.
2. **Training Data:** The code attempts to load pre-processed training data from a pickled file named `data.pickle`. If not found, it processes the intents data to create the necessary training features.

## Model Training

1. **Neural Network:** A sequential neural network is defined using TensorFlow, with hidden layers and a softmax output layer.
2. **Training:** The model is trained on the prepared training data, saving the trained model as `model.h5`.

## Chatbot Interaction

1. **Bag-of-Words:** The `bag_of_words` function converts user input into a numerical representation.
2. **Prediction:** The `chat` function takes user input, processes it using `bag_of_words`, and feeds it to the model for prediction.
3. **Response:** If the predicted intent probability is high enough, a random response from the corresponding intent is selected. Otherwise, a default response is provided.

## Usage

1. **Prepare Intents:** Create the `intents.json` file with your desired intents, patterns, and responses.
2. **Run the Code:** Execute the Python script.
3. **Interact with the Chatbot:** Type messages to the chatbot, and it will respond based on its training.

## Additional Notes

* Consider adding more layers, neurons, or training epochs to improve model performance.
* Experiment with different activation functions and optimizers.
* Explore techniques like regularization (e.g., dropout) to prevent overfitting.
* Consider using more advanced architectures like recurrent neural networks (RNNs) or transformers for more complex tasks.
