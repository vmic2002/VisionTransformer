# VisionTransformer
This repository contains an implementation of a Vision Transformer (ViT) model for image classification tasks. It was developed as part of the "CSC_52002_EP - Computer Vision: from Fundamentals to Applications" class at École Polytechnique.

![Screenshot 2025-01-17 at 9 11 18 PM](https://github.com/user-attachments/assets/ea093b62-789c-4631-9e6d-d25abe9d2ed3)

## Overview
### Model: The Vision Transformer architecture is implemented from scratch, including:
  - Patch Embedding: Converts image patches into vectors using a 2D convolution.
  - Transformer Encoder: Utilizes self-attention mechanisms across image patches.
  - Positional Encoding: Supports both sinusoidal and learned positional encodings.
  - Classification Layer: A simple MLP head for final classification based on the class token.

### Components:
  - `TransformerEncoderBlock`: A single encoder block with multi-head self-attention and feed-forward network.
  - `SinusoidalPositionalEncoding` and `LearnedPositionalEncoding`: For adding positional information.
  - `MultiHeadAttention` and its derivatives for handling attention mechanisms.
  - `FFN` (Feed-Forward Network): Implements the position-wise feed-forward layers.

### Training Loop:
- Includes training and validation phases with metrics like loss and accuracy reported per epoch.

## Usage
To use this model:
1. Ensure you have PyTorch installed.
2. Adjust hyperparameters in the training script.
3. Provide your dataset through a DataLoader (not included in this repo).
4. Run the training script to train the model on your dataset.

## Acknowledgements
This project was developed for educational purposes in the Computer Vision course, providing a practical example of applying transformers to vision tasks. While this implementation is not optimized for production use, it serves as a learning tool and a portfolio piece demonstrating competency in deep learning and computer vision.
