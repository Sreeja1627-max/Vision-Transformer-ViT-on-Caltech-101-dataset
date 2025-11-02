# Vision Transformer (ViT) on Caltech-101  
**Author:** Sreeja Roychoudhury  
**Roll No:** 22052067  
**Institution:** KIIT Deemed To Be University  
**Course:** Deep Learning / Advanced Neural Networks  

---

##  Objective
This project implements a **Vision Transformer (ViT)** from scratch using **PyTorch**, trained on a **Caltech-101 subset** to explore attention-based image classification.  
It evaluates the performance of ViT with roll-number-based hyperparameters to understand how transformer architectures can be adapted for computer vision tasks.

---

##  Dataset
The model is trained and evaluated on a **15-class subset of Caltech-101** containing categories such as:  
`airplanes`, `butterfly`, `chair`, `dolphin`, `elephant`,  
`flamingo`, `kangaroo`, `laptop`, `watch`, `cellphone`,  
`pizza`, `sunflower`, `tick`, `wheelchair`, and `anchor`.

**Preprocessing:**
- All images resized to 224×224 pixels  
- Normalized using ImageNet statistics  
- Divided into non-overlapping 14×14 patches  
- 80/20 train-validation split  

**Dataset Source:** 
 *Google Drive link is provided in* `dataset_link.txt`.

---

##  Model Configuration
**Framework:** PyTorch  
**Architecture:** Vision Transformer (ViT) implemented manually

**Roll-Number-Based Parameters (Seed = 67):**
- Hidden Dimension = 192  
- Attention Heads = 5  
- Patch Size = 14  
- Epochs = 12  

**Model Components:**
- Patch Embedding  
- Multi-Head Self-Attention  
- Transformer Encoder Blocks  
- MLP Head for Classification  
- **Total Parameters:** ~2.8 Million  

Training used **CrossEntropyLoss**, **AdamW optimizer**, and **OneCycleLR scheduler** for stable convergence.

---

##  Setup & Installation

### Requirements
Can install all dependencies using the `requirements.txt` file:
```bash
pip install -r requirements.txt
