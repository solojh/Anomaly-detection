# X-ray Baggage Anomaly Detection

## Overview

This project implements an AI-based anomaly detection system for X-ray baggage images using the Reverse Distillation model from Anomalib.

The system is designed for security screening applications such as:

- Airport baggage inspection
- Security checkpoint monitoring
- Contraband detection

The model is trained to learn normal X-ray baggage patterns and detect anomalous or concealed objects.

---

# Features

- Reverse Distillation anomaly detection model
- X-ray baggage image dataset training
- Data preprocessing and augmentation
- Model evaluation and testing
- PyTorch model export
- OpenCLIP feature extraction support
- GPU acceleration using CUDA

---

# Model Configuration

The project uses:

- Model: ReverseDistillation
- Backbone: wide_resnet50_2
- Framework: Anomalib
- Device: CUDA / CPU

```python
model = ReverseDistillation(
    backbone="wide_resnet50_2",
    layers=["layer1", "layer2", "layer3"]
)

