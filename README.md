# Recurrent Neural Networks (RNN) for Sentiment Analysis

This repository contains a series of Jupyter notebooks demonstrating the implementation and comparison of various Recurrent Neural Network (RNN) architectures—SimpleRNN, LSTM, and GRU—for a binary sentiment classification task on the IMDb movie review dataset.

The core objective is to illustrate the foundational concepts of sequence modeling, including data preparation techniques like Integer Encoding and Word Embedding, and to compare the performance and complexity of unidirectional, bidirectional, and deep RNN structures.

The core objective is to illustrate the foundational concepts of sequence modeling, including data preparation techniques like Integer Encoding and Word Embedding, and to compare the performance and complexity of unidirectional, bidirectional, and deep RNN structures.

##  📚 Repository Structure and Contents

Notebook File:- [Integer_Encodimg_SimpleRNN.ipynb](https://github.com/AmanRajput997/RNN/blob/main/Integer_Encodimg_SimpleRNN.ipynb)

Description:- Demonstrates the initial steps of preparing text data, including tokenization, Integer Encoding, and sequence padding. It then builds and trains a basic SimpleRNN model on the encoded data.

Notebook File:- [Embedding_Encoding_SimpleRNN.ipynb](https://github.com/AmanRajput997/RNN/blob/main/Embedding_Encoding_SimpleRNN.ipynb)

Description:- Introduces the Word Embedding technique. It contrasts it with simple integer encoding by building a model with an Embedding layer followed by a SimpleRNN for the sentiment classification task.

Notebook File:- [Deep_RNNs.ipynb](https://github.com/AmanRajput997/RNN/blob/main/Deep_RNNs.ipynb)

Description:- Explores the concept of Deep RNNs by stacking multiple recurrent layers. It shows the implementation of both stacked SimpleRNN layers, stacked LSTM layers, and stacked GRU layers, highlighting the use of the return_sequences=True parameter.

Notebook File:- [Bidirectional_RNN.ipynb](https://github.com/AmanRajput997/RNN/blob/main/Bidirectional_RNN.ipynb)

Description:- Focuses on Bidirectional RNNs, which process the input sequence in both forward and backward directions to capture context from all points in the sequence. Implementations include Bidirectional wrappers around SimpleRNN, LSTM, and GRU.

Notebook File:- [RNN_Architeture_Demo.ipynb](https://github.com/AmanRajput997/RNN/blob/main/RNN_Architeture_Demo.ipynb)

Description:- A supplementary notebook that focuses on the low-level weight and parameter structure of a minimal SimpleRNN and Dense layer to reinforce understanding of RNN parameter calculation.


## ✨ Key Architectural Highlights
This project provides practical, side-by-side examples of key Recurrent Neural Network techniques:

### • Bidirectional Processing: 
Utilizing the Bidirectional layer wrapper to enhance context understanding in sequential data. The number of parameters in the recurrent layer effectively doubles when using the Bidirectional wrapper (Bidirectional(SimpleRNN(5)) has 380 params, while SimpleRNN(5) has 190 params).

### • Deep (Stacked) RNNs: 
Implementing multi-layer recurrent models (e.g., stacked LSTM/GRU) where the output of the previous layer (return_sequences=True) feeds directly into the next, allowing the model to learn more complex feature hierarchies.

### • Recurrent Cell Comparison: 
Comparing the parameter counts and structure of different recurrent cells:

### • SimpleRNN: 
The simplest form, prone to the vanishing gradient problem.

### • GRU: 
Gated Recurrent Unit, a highly effective and computationally cheaper alternative to LSTM.

### • LSTM: 
Long Short-Term Memory, the standard for capturing long-range dependencies in sequence data.
