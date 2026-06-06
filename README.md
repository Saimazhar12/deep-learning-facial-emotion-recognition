# 😊 Facial Emotion Recognition using Hybrid CNN-GCN

This project presents a Facial Emotion Recognition system that combines a pretrained ResNet50 CNN with a Graph Convolutional Network (GCN) built on facial landmarks extracted using MediaPipe. The model classifies facial expressions into seven emotions with high accuracy.

## 📌 Project Overview

The system uses both facial appearance features and landmark-based geometric relationships to improve emotion recognition performance.

## 🎭 Emotion Classes

- Angry
- Disgust
- Fear
- Happy
- Neutral
- Sad
- Surprise

## 📂 Dataset

**Dataset:** RAF-DB (Real-world Affective Faces Database)

Dataset Link:
https://www.kaggle.com/datasets/dollyprajapati182/balanced-raf-db-dataset-7575-grayscale

### After Cleaning & Balancing

| Split | Images |
|--------|--------:|
| Training | 27,916 |
| Validation | 6,347 |
| Testing | 3,773 |

The dataset was processed using:

- Duplicate image removal
- Perceptual hashing (pHash)
- Data augmentation
- Class balancing

## ⚙️ Features

- Hybrid ResNet50 + GCN architecture
- MediaPipe facial landmark extraction
- Dataset cleaning and duplicate removal
- Data augmentation and class balancing
- Early stopping and model checkpointing
- Confusion matrix and classification report

## 🏋️ Model Training

- Architecture: Hybrid ResNet50 + GCN
- Optimizer: Adam
- Batch Size: 32
- Epochs: 10
- Early Stopping & Checkpoint
- Best Validation Accuracy: 95.81%
- Best Validation F1-Score: 96.04%

## 🧠 Technologies Used

- Python
- PyTorch
- Torch Geometric
- ResNet50
- MediaPipe
- OpenCV
- Scikit-learn
- Matplotlib

## 📊 Results

- Test Accuracy: **94.51%**
- Macro F1-Score: **94.72%**

## 🚀 How to Run

1. Clone the repository
2. Install dependencies
3. Prepare the RAF-DB dataset
4. Run the training notebook
5. Evaluate the model

## 📌 Conclusion

This project demonstrates how combining CNN-based image features with GCN-based facial landmark features can achieve highly accurate facial emotion recognition.
