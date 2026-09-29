# Handwritten Digit Generation Using DCGAN

This project implements a Deep Convolutional Generative Adversarial Network (DCGAN) using TensorFlow and Keras to generate handwritten digit images similar to the MNIST dataset.

The project demonstrates the complete GAN workflow, including image preprocessing, Generator and Discriminator design, adversarial training, latent-space sampling, training progression, and final image generation.

## Project Objective

Build and train a DCGAN capable of learning the visual distribution of handwritten digits and generating new synthetic digit images from random latent vectors.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Jupyter Notebook

## Model Architecture

### Generator

The Generator maps a 100-dimensional random latent vector to a `28 × 28 × 1` grayscale image.

```text
100-dimensional latent vector
            ↓
        Dense Layer
            ↓
        7 × 7 × 256
            ↓
    Conv2DTranspose
            ↓
       14 × 14 × 128
            ↓
    Conv2DTranspose
            ↓
        28 × 28 × 64
            ↓
        Conv2D + tanh
            ↓
        28 × 28 × 1