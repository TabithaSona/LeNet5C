# LeNet5C
**LeNet-5 Implementation from Scratch**

## Overview
This project is a from-scratch implementation of the landmark LeNet-5 convolutional neural network architecture from the paper "Gradient-Based Learning Applied to Document Recognition" by Yann LeCun et al. (1998). The entire implementation, training, and evaluation are contained within a single Google Colab notebook.

The goal was to translate the architectural description from the original paper into functional PyTorch code and validate its performance on the MNIST handwritten digit dataset.

## Architecture
- Input: 32x32 grayscale images
- C1: 6@28x28 (5x5 convolution)
- S2: 6@14x14 (2x2 average pooling)
- C3: 16@10x10 (5x5 convolution)
- S4: 16@5x5 (2x2 average pooling)
- C5: 120@1x1 (5x5 convolution)
- F6: 84 fully connected units
- Output: 10 units (RBF in paper, softmax in this implementation)

## Results
- Final Test Accuracy: 98.07%
- Error Rate: 1.93%
*This result demonstrates a successful implementation of the core LeNet-5 architecture. The variance from the paper's result provides an interesting point of analysis on historical vs. modern training techniques.*

## How to Run
1. Open the Notebook: link
2. Run the notebook

## References
LeCun, Y., Bottou, L., Bengio, Y., & Haffner, P. (1998). Gradient-based learning applied to document recognition. Proceedings of the IEEE.

## Comparison with Paper
The original paper reported:
- 0.8% error rate with distorted training data
- 0.95% error rate without distortions

Our implementation achieved: 1.93% error rate
