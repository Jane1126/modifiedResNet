# ECE-GY 7123 Introduction to Deep Learning Mini-Project

This is the Mini-Project for ECE-GY 7123 Introduction to Deep Learning. The goal of this mini-project is to design a modified Residual Network (ResNet) architecture with the highest test accuracy on the CIFAR-10 image classification dataset, under the constraint that your model has no more than 5 million parameters.

---

# Contributors

* **Syed Ahzam Tariq (sat10045@nyu.edu)**
* **Safdar Ahmed (sa8237@nyu.edu)**
* **Ran Xu (rx523@nyu.edu)**

---

### Abstract

In this paper, we present modified versions of the ResNet model designed to achieve high accuracy within the constraint of fewer than 5 million trainable parameters. Through extensive experimentation involving various techniques such as learning rates, efficient optimizers, epoch, and dropout strategies, we have fine-tuned these models to optimize performance. Our results are meticulously analyzed and discussed, highlighting the potential implications for applications where model size and computational resource limitations are significant.

We proposed a custom ResNet Architecture and we implemented 3 Networks ResNetSmall, ResNetMedium and ResNetLarge,

| Network      | Number of Parameters | Convolutional Channels | Optimizers                        | Training Accuracy | Testing Accuracy |
| ------------ | -------------------- | ---------------------- | --------------------------------- | ----------------- | ---------------- |
| ResNet18  | 4,815,940               | [42, 84, 168, 336]           | AdamW | 97.98%            | 93.02%           |
| ResNetLarge  | 4,903,242            | [64, 128, 256, 512]    | SGD + Momentum (Nesterov Enabled) | 98.22%            | 92.73%           |

---

### System Specification

* NYU Greene HPC Jupyter Environmrnt
* CPU: 8 Virtualized Cores of Intel Xeon-Platinum 8286
* GPU: Nvidia Tesla v100
* System Memory: 96 GB
* Python Version: 3.11
* CUDA version: v11.1.74
* Torch Version: 2.0.0

---