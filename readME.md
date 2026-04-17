# Image Recognition Model Comparison

## Overview
This project focuses on building and evaluating multiple deep learning models for image recognition. The objective was to compare different neural network architectures, preprocessing techniques, and training strategies to identify the best-performing configuration for image classification.

Several experiments were conducted using variations in:

- Data preprocessing
- Convolutional layers
- Dense layers
- Pooling strategies
- Batch normalization
- Dropout
- Optimizers
- Batch sizes
- Early stopping

---

## Project Goals

- Build and compare multiple image classification models
- Improve performance through experimentation
- Reduce overfitting
- Learn deep learning workflows
- Evaluate models using structured metrics

---

## Features

- 13 trained model versions
- Structured experiment comparison
- Accuracy / loss evaluation
- Reproducible training pipeline
- Performance benchmarking

---

## Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook / Google Colab

---

## Final Results (Top Models)

| Rank | Model | Test Accuracy | Validation Accuracy | Time |
|------|------|--------------|--------------------|------|
| 🥇 | Model 13 - Together | **90.38%** | **90.98%** | 4m |
| 🥈 | Model 12 - Together | **86.76%** | 86.76% | 5m |
| 🥉 | Model 11 - Sara | **83.98%** | 84.20% | 9m |
| 4 | Model 10 - Philippe | **81.55%** | 81.93% | 6m |

---

## Top Performing Models

### 🥇 Model 13 - Together (90.38%)

**Key Changes**
- Final MobileNetV2 Model
- Gradio Deployment Ready
- 128 Neurons
- Batch Normalization
- Dropout
- Global Average Pooling
- Padding
- Learning Rate: 0.00001
- Adam Optimizer
- Batch Size: 16

**Metrics**
- Training Accuracy: 88.48%
- Validation Accuracy: 90.98%
- Test Accuracy: **90.38%**

---

### 🥈 Model 12 - Together (86.76%)

**Key Changes**
- MobileNetV2 Base Model
- 128 Neurons
- Batch Normalization
- Dropout
- Learning Rate: 0.0005
- Adam Optimizer
- Batch Size: 64

**Metrics**
- Training Accuracy: 86.63%
- Validation Accuracy: 86.76%
- Test Accuracy: **86.76%**

---

### 🥉 Model 11 - Sara (83.98%)

**Key Changes**
- 128 Neurons
- 6 Convolution Layers
- 2 MaxPooling Layers
- Batch Normalization
- Data Augmentation
- Padding
- Batch Size: 64

**Metrics**
- Training Accuracy: 91.65%
- Validation Accuracy: 84.20%
- Test Accuracy: **83.98%**

---

### 4. Model 10 - Philippe (81.55%)

**Key Changes**
- 128 Neurons
- 6 Convolution Layers
- 2 MaxPooling Layers
- Batch Normalization
- Global Average Pooling
- Data Augmentation

**Metrics**
- Training Accuracy: 89.68%
- Validation Accuracy: 81.93%
- Test Accuracy: **81.55%**

---

## Best Result

The strongest configuration was **Model 13 - Together**, achieving:

- **90.38% Test Accuracy**
- **90.98% Validation Accuracy**
- Fast runtime (4 minutes)
- Strong generalization performance

---

## What We Learned

- Simpler architectures can outperform deeper CNNs
- Batch Normalization improves training stability
- Dropout reduces overfitting
- Learning rate tuning is critical
- Batch size influences convergence
- Structured experimentation improves results faster

---

## Future Improvements

- Advanced Transfer Learning (ResNet, EfficientNet, DenseNet)
- Automated Hyperparameter Optimization
- Training on Larger and More Diverse Datasets
- Real-time Camera Prediction System
- Ensemble Model Architectures
- Explainable AI and Model Interpretability

---

## Authors
Sara Ahmadi,  
Dimitrios Gretsistas,  
Philippe Rallier du Baty

## Run Project

```bash
pip install -r requirements.txt
python train.py
```

