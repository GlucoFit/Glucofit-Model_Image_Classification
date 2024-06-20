# Food Image Classification using Transfer Learning

This repository contains a transfer learning-based image classification project for recognizing various food items from the Food-101 dataset. We employed ResNet50, DenseNet121, and EfficientNetB7 architectures, with EfficientNet showing the highest accuracy among them, achieving 80% for accuracy and val_accuracy.

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Model Architecture](#model-architecture)
4. [Training](#training)
5. [Evaluation](#evaluation)
6. [Further Work](#further-work)

---

## Introduction

This project aims to classify food items using deep learning techniques, specifically leveraging transfer learning with pre-trained models like ResNet50, DenseNet121, and EfficientNetB7. The goal is to accurately identify 60 different food categories based on images.

---

## Dataset

We used the [Food-101 dataset](https://www.kaggle.com/datasets/dansbecker/food-101), which consists of 101 food categories. 
<details>
<summary>Click to expand for the list of food categories</summary>

- apple_pie
- baby_back_ribs
- baklava
- beignets
- bibimbap
- breakfast_burrito
- caesar_salad
- cannoli
- caprese_salad
- cheesecake
- cheese_plate
- chicken_curry
- chicken_wings
- chocolate_cake
- chocolate_mousse
- churros
- club_sandwich
- creme_brulee
- cup_cakes
- donuts
- dumplings
- falafel
- filet_mignon
- fish_and_chips
- french_fries
- french_toast
- fried_calamari
- fried_rice
- frozen_yogurt
- garlic_bread
- greek_salad
- grilled_cheese_sandwich
- grilled_salmon
- gyoza
- hamburger
- hot_dog
- ice_cream
- lasagna
- macaroni_and_cheese
- macarons
- miso_soup
- nachos
- omelette
- onion_rings
- pancakes
- pizza
- prime_rib
- ramen
- red_velvet_cake
- samosa
- sashimi
- spaghetti_bolognese
- spaghetti_carbonara
- steak
- strawberry_shortcake
- sushi
- tacos
- takoyaki
- tiramisu
- waffles

</details>


The dataset provides a diverse collection of food images suitable for training deep learning models.

---

## Model Architecture

### Transfer Learning Models Used:
- **ResNet50**: Known for its deep architecture and effectiveness in image classification tasks.
- **DenseNet121**: Utilizes dense connections between layers to improve feature propagation and reuse.
- **EfficientNetB7**: A scalable and efficient model architecture that balances accuracy and computational resources.

Among these models, ResNet50 demonstrated superior performance in our experiments, achieving an accuracy of 80%.

---

## Training

### Data Preparation:
- The dataset was split into training (85%), validation (7.5%), and test (7.5%) sets.
- Images were preprocessed and augmented using `ImageDataGenerator` from TensorFlow.

### Training Procedure:
- We defined a model architecture using ResNet50 as the base feature extractor.
- The model was compiled with categorical crossentropy loss and Adam optimizer.
- Training was conducted over 20 epochs.

---

## Evaluation

### Performance Metrics:
- **Accuracy**: 80%
- **Loss**: Categorical crossentropy

The model showed robust performance in classifying food images, especially excelling in identifying certain complex dishes.

---

## Further Work

Future enhancements to this project could include:
- **Fine-tuning**: Fine-tuning the top layers of the models for better performance.
- **Deployment**: Deploying the model in a production environment, possibly as a mobile application.
- **Data Augmentation**: Exploring additional data augmentation techniques to improve model generalization.

---

This README provides an overview of our approach, results, and potential future directions for this food image classification project. For detailed implementation and code, please refer to the repository.

---
