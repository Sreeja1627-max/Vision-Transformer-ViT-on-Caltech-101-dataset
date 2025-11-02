# Vision Transformer (ViT) on Caltech-101  
**Author:** Sreeja Roychoudhury | **Roll No.:** 22052067  

---

##  Objective
This project implements a Vision Transformer (ViT) from scratch using **PyTorch**, trained on a **Caltech-101 subset** to analyze attention-based image classification as part of a deep learning assignment.
---

##  Dataset
The model is trained and evaluated on a subset of the Caltech-101 dataset containing multiple object classes such as *sunflower*, *airplane*, *butterfly*, *chair*, and others.  
All images are resized to 224×224 and divided into training and validation sets.  
The dataset link is provided in **`dataset_link.txt`**.

---

##  Model Configuration
- Framework: PyTorch  
- Hidden Dimension: 192  
- Attention Heads: 5  
- Patch Size: 14  
- Epochs: 12  
- Seed: 67  

The Vision Transformer architecture includes patch embedding, multi-head self-attention, feed-forward MLP layers, and a classification head.

---

## Setup
1. Clone the repository:  
   ```bash
   git clone https://github.com/Sreeja1627-max/Vision-Transformer-ViT-on-Caltech-101-dataset.git
   cd Vision-Transformer-ViT-on-Caltech-101-dataset
