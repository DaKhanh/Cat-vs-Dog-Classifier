# Cat and Dog Classification Project

This project focuses on image classification, initially distinguishing between cats and dogs, and later extended to classify all 10 classes from the CIFAR-10 dataset. It demonstrates the use of both a custom CNN model and a pretrained EfficientNetB0 model for classification tasks.


## Project Overview

The project originally aimed to classify images into two categories: cats and dogs. Two different approaches were implemented:

1. **Custom CNN model** – Designed from scratch for binary classification.  
2. **Pretrained EfficientNetB0** – Fine-tuned for improved accuracy using transfer learning.  

The project was later extended to handle **10-class classification** using the CIFAR-10 dataset.


## Dataset

- **Cat vs Dog dataset** – Images of cats and dogs.  
- **CIFAR-10 dataset** – 60,000 32x32 color images in 10 classes, with 6,000 images per class. Classes include:  
  `airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck`.


## Models

### 1. Custom CNN Model
- Designed from scratch for binary classification.  
- Achieved **88.2% validation accuracy** on Cat vs Dog dataset.  

### 2. Pretrained EfficientNetB0
- Fine-tuned on the Cat vs Dog dataset using transfer learning.  
- Achieved **99.1% validation accuracy** on Cat vs Dog dataset.  

### 3. CIFAR-10 Extension
- Models were modified to output 10 classes.  
- Custom CNN and EfficientNetB0 architectures were adapted to handle 10-class classification.


## Training

- Used **Tensorflow** framework.  
- Binary cross-entropy loss for Cat vs Dog classification.  
- Cross-entropy loss for CIFAR-10 10-class classification.  
- Optimizers: Adam with learning rate scheduling.  
- Data augmentation: random flips, rotations, and normalization applied during training.  


## Results

| Model                   | Cat vs Dog Accuracy | CIFAR-10 Accuracy |
|-------------------------|------------------|----------------|
| Custom CNN              | 88.2%            |  66.5          |
| Fine-tuned EfficientNetB0 | 99%              | 91.3             |

> Note: CIFAR-10 accuracies depend on training runs and hyperparameters.


## Extending to CIFAR-10

1. Updated model output layer to 10 neurons for 10 classes.  
2. Adjusted loss function from binary to multi-class cross-entropy.  
3. Adapted data loaders for CIFAR-10 dataset.  

# Cat-vs-Dog-Classifier
