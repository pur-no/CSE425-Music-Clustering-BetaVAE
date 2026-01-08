# Unsupervised Learning Project: VAE for Hybrid Language Music Clustering

## 📌 Project Overview
**Course:** CSE425: Neural Networks  
**Goal:** Implement a Variational Autoencoder (VAE) to cluster music tracks based on a hybrid of Audio features (Spectrograms) and Lyrical meaning (DistilBERT embeddings).

Compare three architectures:
1. **Baseline:** PCA + K-Means (Linear)
2. **Basic VAE:** CNN Encoder (Audio Only)
3. **Multi-Modal Beta-VAE:** Disentangled Audio+Text Representation

## 📂 Repository Structure
- `data/`: Contains the dataset metadata (`lyrics_dataset.csv`). *Note: Audio files are excluded due to size constraints. Audio Files are in the drive folder*
- `notebooks/`: Contains the complete source code `CSE425_Neural_Networks_Project.ipynb`.
- results and report are in the drive folder

## 📊 Key Results
Our proposed **Beta-VAE (beta=4)** significantly outperformed both the linear baseline and the standard VAE.

| Model | Modality | Silhouette Score |
|-------|----------|------------------|
| PCA Baseline | Audio | 0.4018 |
| Basic VAE | Audio | 0.3172 |
| **Beta-VAE** | **Audio + Lyrics** | **0.5321** |

## 🚀 How to Run
1. **Install Dependencies:**
   ```bash

   pip install -r requirements.txt
