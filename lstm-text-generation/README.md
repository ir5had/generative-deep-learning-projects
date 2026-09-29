# Character-Level Text Generation Using LSTM

A small character-level language model built with TensorFlow and Keras that learns character patterns from *Alice's Adventures in Wonderland* and generates text autoregressively.

## Project Overview

This project demonstrates a complete character-level language modeling workflow:

- Text preprocessing
- Character-level encoding
- Sequence creation
- LSTM-based next-character prediction
- Autoregressive generation
- Temperature sampling
- Perplexity-based evaluation
- Controlled model improvement
- Failure analysis

The project intentionally uses a small dataset and compact model so that the complete workflow remains understandable and fast to train.

## Dataset

The project uses the public-domain text of *Alice's Adventures in Wonderland* by Lewis Carroll from Project Gutenberg.

Source:

https://www.gutenberg.org/ebooks/11

Approximately 80,000 characters from the beginning of the story are used as the training corpus.

## Architecture

```text
Character IDs
      ↓
Embedding(64)
      ↓
LSTM(128)
      ↓
Dense(72, Softmax)