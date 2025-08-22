# Face Recognition using Siamese Network

## Overview
This project implements a **Face Verification and Recognition System** using a **Siamese Neural Network** with TensorFlow and OpenCV.  
The system is capable of learning **similarity between face pairs** and can verify whether two given face images belong to the same person.  

## Approach
- **Dataset Preparation**  
  - Used the **LFW (Labeled Faces in the Wild)** dataset.  
  - Created three sets of images: **Anchor**, **Positive**, and **Negative**.  
  - Performed preprocessing (grayscale conversion, resizing, normalization).  

- **Model Architecture**  
  - Built a **Siamese Network** using Keras with convolutional layers, max pooling, and dense layers.  
  - Designed a **contrastive loss function** to measure similarity between embeddings.  
  - Used triplet-style training with Anchor, Positive, and Negative samples.  

- **Training Strategy**  
  - Generated positive and negative pairs dynamically.  
  - Optimized with **Adam optimizer** and early stopping to avoid overfitting.  
  - Achieved good generalization on unseen test data.  

- **Real-Time Testing**  
  - Integrated with **OpenCV** to capture images from a webcam.  
  - System verifies if a captured face matches the registered person.  

## Key Features
- Uses a **Siamese Network** for robust face verification.  
- Handles variations in lighting and background using preprocessing.  
- Works in **real-time** with webcam input.  

## Results
- Successfully distinguishes between matched and unmatched face pairs.  
- Achieved reliable accuracy in both training and real-time testing.  
- Demonstrated potential for applications in **biometric authentication**.  

## Future Scope
- Extend to larger datasets for more robustness.  
- Optimize for **deployment on edge devices** (Raspberry Pi, mobile).  
- Add support for **multi-face recognition** and **user database management**.  

---
