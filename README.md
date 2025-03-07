# Developing a Handwritten Digits Classifier with PyTorch

## Overview

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify handwritten digits from the MNIST dataset. The model is trained, validated, and evaluated to achieve high accuracy in digit recognition.

## Dataset

- **Source**: [**MNIST Dataset**](http://yann.lecun.com/exdb/mnist/)
- **Training Set**: 50,000 images
- **Validation Set**: 10,000 images
- **Test Set**: 10,000 images
- **Preprocessing**:
  - Converted to tensors
  - Normalized to [-1, 1] for stable training

## Model Architecture

- **Conv Layer 1**: 32 filters, 3x3 kernel, ReLU, MaxPooling
- **Conv Layer 2**: 64 filters, 3x3 kernel, ReLU, MaxPooling
- **Fully Connected Layers**: 128 → 64 → 10 (output classes)
- **Activation Function**: ReLU
- **Output Layer**: Softmax (for classification)

## Training

- **Optimizer**: Adam (learning rate = 0.001)
- **Loss Function**: Cross-entropy loss
- **Epochs**: 10
- **Batch Size**: 64
- **Validation Split**: 10,000 images for tuning model performance

## Results

- **Validation Accuracy**: ~98%
- **Test Accuracy**: ~98%

## References

- [**Yann LeCun’s MNIST Benchmarks**](http://yann.lecun.com/exdb/mnist/)

## License

This project is open-source under the MIT License.
