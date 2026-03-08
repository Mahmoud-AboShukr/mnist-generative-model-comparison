# MNIST Generative Modeling Playground

A deep learning project that explores multiple generative approaches on the MNIST dataset, with an emphasis on reconstruction quality, latent space behavior, and sample generation. The notebook brings together **Autoencoders, Variational Autoencoders (VAE), Vector-Quantized VAE (VQ-VAE), and GAN-based models** in a single workflow for comparison and analysis.

## Project Overview

This project investigates how different generative architectures learn compact representations of handwritten digits and how those representations can be used for:

- image reconstruction
- latent space exploration
- random sample generation
- interpolation between digit representations
- model comparison across reconstruction and generation tasks

Rather than focusing on a single model, the project provides a comparative experimental pipeline showing the strengths and trade-offs of several classic deep learning approaches for generative modeling.

## Methods Included

The notebook covers the following model families:

- **Autoencoder (AE)** for compact latent representation and reconstruction
- **Variational Autoencoder (VAE)** for probabilistic latent modeling and smooth interpolation
- **Vector-Quantized VAE (VQ-VAE)** for discrete latent representations
- **DCGAN-style GAN** for image generation
- **Improved GAN variant** for more stable training and better qualitative results

## Main Components

### 1. Data preparation
- MNIST loading and preprocessing
- normalization
- dataset visualization
- class distribution inspection

### 2. Reconstruction-based models
- training and evaluation of AE / VAE-style models
- visual comparison of original vs reconstructed images
- latent interpolation between samples
- 1D latent traversals for interpretability

### 3. Discrete latent modeling
- VQ-VAE implementation and checkpoint loading
- reconstruction analysis
- visual and qualitative comparison with previous models

### 4. Adversarial generation
- GAN training pipeline on MNIST
- baseline GAN and improved GAN comparison
- stability and generation quality inspection

## Repository Structure

```text
mnist-generative-modeling-playground/
├── README.md
├── requirements.txt
├── mnist-generative-model-comparison.ipynb
└── assets/            # optional: figures or sample outputs
```

## Installation

Create a virtual environment and install the dependencies:

```bash
pip install -r requirements.txt
```

## How to Run

Open the notebook in Jupyter and execute the cells sequentially:

```bash
jupyter notebook TP.ipynb
```

or

```bash
jupyter lab TP.ipynb
```

## Outputs and Experiments

The project includes several types of outputs that are useful for analysis and presentation:

- reconstructed digit images
- generated samples
- latent interpolations
- latent traversals
- training curves
- qualitative comparisons between model families

## Repository Description

**Comparative generative modeling on MNIST using autoencoders, VAE, VQ-VAE, and GANs in PyTorch.**
