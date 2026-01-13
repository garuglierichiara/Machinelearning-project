# Multi-label Story Tag Classification

## Project Overview
This project focuses on **Multi-label Text Classification** using the TinyStories dataset. The goal is to predict distinct story tags (such as 'Conflict', 'Foreshadowing', etc.) based on the text content.

## Methods
The project compares two distinct architectures to solving this task:
1. **Fine-tuned RoBERTa:** A transformer-based model optimized for this specific task.
2. **Custom CNN:** A Convolutional Neural Network built from scratch for text classification.
 

## Results
* **RoBERTa** was the top performer, reaching over **90% accuracy** on all categories. It did a great job spotting abstract concepts like *Conflict* and *Foreshadowing*.
* **CNN** worked well as a faster alternative. While it successfully found most tags (high recall), it struggled to be as precise as RoBERTa with subtle details.

| Tag | RoBERTa F1 | CNN F1 |
| :--- | :---: | :---: |
| **Dialogue** | 0.9396 | 0.9160 |
| **Twist** | 0.9154 | 0.8654 |
| **Conflict** | 0.5753 | 0.4271 |
| **Foreshadowing** | 0.5687 | 0.4395 |

## Languages & Libraries
The project is written in **Python** and relies on these main libraries:
* PyTorch
* Transformers (Hugging Face)
* Pandas & NumPy
* Matplotlib
* Gdown
  
## Dataset & Model Weights
Due to GitHub's file size limits, the trained model weights (`.pth`) and the specific training/test splits are hosted externally.
**[Download Models and Dataset from Google Drive](https://drive.google.com/drive/folders/10qLK2236d8LLDMgShcG9WuSTgqjoPWdr?usp=share_link)**
