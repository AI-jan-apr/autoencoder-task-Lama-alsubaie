# Autoencoder with MNIST Dataset

## Project Overview
This project demonstrates how to build and train an autoencoder using the MNIST handwritten digit dataset.  
The model learns to compress images into a latent representation and reconstruct them.  
The encoded features are also used for visualization and image retrieval.

## Dataset
- Dataset: MNIST (mnist_784)
- Total images: 70,000
- Image size: 28 × 28 pixels
- Each image is flattened into 784 features.

## Model Architecture
The autoencoder consists of two parts:

**Encoder**
- Input: 784 features
- Dense layers compress the image into a smaller latent representation.

**Decoder**
- Reconstructs the original image from the latent space.

## Training
- Loss Function: Mean Squared Error (MSE)
- Optimizer: Adam
- The model is trained to reconstruct the input images.

## Visualization
The encoded features are reduced to 2 dimensions using PCA for visualization of the latent space.

## Image Retrieval
A query image is encoded using the encoder.  
Cosine similarity is then used to find the most similar images from the training set.

## Results
- Training and validation loss decrease steadily.
- The model successfully reconstructs digit images.
- Image retrieval returns visually similar digits.

## Conclusion
The autoencoder effectively learns compressed representations of handwritten digits.  
These representations can be used for reconstruction, visualization, and similarity-based image retrieval.