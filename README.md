# Generative Deep Learning Projects

A collection of practical deep learning projects focused on generative modeling and sequence generation using TensorFlow and Keras.

## Projects

### 1. Character-Level Text Generation Using LSTM

A character-level language model trained on *Alice's Adventures in Wonderland* to learn character sequences and generate new text.

**Key concepts:**

- Character-level text preprocessing
- Sequence creation
- Embeddings
- LSTM networks
- Next-character prediction
- Autoregressive text generation
- Temperature-based sampling
- Model evaluation

[View LSTM Text Generation Project](lstm-text-generation/)

---

### 2. Handwritten Digit Generation Using DCGAN

A Deep Convolutional Generative Adversarial Network trained on the MNIST dataset to generate synthetic handwritten digit images.

**Key concepts:**

- Generative Adversarial Networks
- Generator and Discriminator
- Convolutional neural networks
- Transposed convolution
- Adversarial training
- Custom TensorFlow training loops
- Latent-space sampling
- Image generation
- Training progression

[View DCGAN Project](dcgan-mnist/)

---

## Technologies

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Jupyter Notebook

## Repository Structure

```text
generative-deep-learning-projects/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── lstm-text-generation/
│   ├── lstm_text_generation.ipynb
│   ├── README.md
│   ├── data/
│   ├── models/
│   └── outputs/
│
└── dcgan-mnist/
    ├── dcgan_mnist.ipynb
    ├── README.md
    ├── models/
    └── outputs/