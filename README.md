# Next Word Predictor

A next-word prediction model built using an LSTM neural network trained on custom text data.

## Dataset

The model is trained on a custom text corpus. The project demonstrates the approach using a sample text, which can be replaced with any domain-specific dataset.

## Project Structure

1. Text Tokenization - Tokenized the corpus and built a word index using Keras Tokenizer
2. Sequence Generation - Generated input-output pairs using a sliding window approach, mapping N words to the (N+1)th word
3. Data Preparation - Padded sequences and applied one-hot encoding to output labels
4. Model Building - Built an LSTM-based neural network with an Embedding layer
5. Training - Trained the model to minimize categorical cross-entropy loss
6. Prediction - Given an input sequence, the model predicts the most likely next word

## Model Architecture

- Embedding Layer - Converts word indices to dense vector representations
- LSTM Layer - Captures sequential dependencies in the text
- Dense Output Layer - Softmax activation over the full vocabulary for next-word prediction

## Libraries

- Python
- TensorFlow / Keras
- NumPy
