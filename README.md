# Skin Cancer Detection - Kaggle-ISIC-Challenge
Problem Description: Develop image-based algorithms to identify histologically confirmed skin cancer cases with single-lesion crops from 3D total body photos (TBP). The image quality resembles close-up smartphone photos, which are regularly submitted for telehealth purposes. Your binary classification algorithm could be used in settings without access to specialized care and improve triage for early skin cancer detection.

## 3D TBP Images:
![isic 3d tbp images](https://github.com/user-attachments/assets/17cf3ab7-487a-448e-9c89-2b4dae679088)

## Patient lesion data:
![isic-patient data](https://github.com/user-attachments/assets/7aefcf7b-c555-4c86-b2ec-0b9505bcfc55)

Experimentation: Built hybrid architectures to combine features from 3D TBP images and patient diagnostic data (categorical and numerical variables). Experimentated with two different approaches:
Approach 1: Extracted image features using a pretrained Vision Transformer (ViT model). Then created hybrid architecture of dense neural networks - two DNNs combined together (one for image features and one for patient diagnostic features).
Approach 2: Created a bayesian convolutional network by using convolution 2d reparameterization layer from tensorflow probability for image features and another bayesian neural network for patient diagnostic data and then trained them together as a hybrid model.
