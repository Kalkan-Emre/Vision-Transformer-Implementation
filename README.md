# Vision Transformer (ViT) Implementation

This project implements a Vision Transformer (ViT) for image classification using PyTorch. The ViT architecture adapts the transformer model, originally designed for NLP tasks, to process images by dividing them into smaller patches and treating these patches as sequential tokens.

## Key Features

### 1. Model Architecture
- **Input Patches**: Images are split into fixed-size patches and flattened.
- **Linear Embedding**: Patches are linearly embedded into higher-dimensional vectors.
- **Positional Embedding**: Positional encodings are added to retain spatial information.
- **Transformer Encoder**: Multi-head self-attention layers and feedforward networks process the embedded patches.
- **Classification Head**: A linear layer maps the output of the transformer encoder to class probabilities.

### 2. Data Handling
- **Dataset**: CIFAR-10, a 10-class image classification dataset.
- **Data Augmentation**: Normalization and image transformations are applied.
- **Data Loading**: Efficient batch processing using PyTorch DataLoader.

### 3. Training Pipeline
- **Loss Function**: CrossEntropyLoss for multi-class classification.
- **Optimizer**: Adam optimizer with adjustable learning rates.
- **Metrics**: Loss is tracked and plotted across training iterations.

### 4. Visualization
- A loss curve is plotted to monitor model performance during training.

## Highlights
- Demonstrates the use of transformers for vision tasks.
- Trains a ViT model from scratch on CIFAR-10.
- Provides a flexible framework for experimenting with ViT parameters like patch size, embedding dimension, and transformer layers.

This project showcases a hands-on implementation of Vision Transformers, bridging the gap between state-of-the-art NLP and computer vision techniques.
