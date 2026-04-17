# 🎬 Multimodal IMDB Genre Classification (Keras)

This project explores multimodal deep learning for film genre classification using the IMDB dataset. Two separate models are implemented and evaluated:

- 🖼️ **CNN** for classifying movie posters (image data)
- 📝 **LSTM** for classifying movie overviews (text data)

The task is **multi-label classification** across 25 genres.

---

## 📊 Project Overview

The goal is to compare how effectively visual and textual information can be used to predict film genres. The project includes:

- Data preprocessing pipelines using `tf.data`
- Custom CNN with **Residual Blocks**
- LSTM model with **TextVectorization + Embedding**
- Model training with checkpoints
- Evaluation using:
  - Training curves
  - Confusion matrices
  - Example predictions

---

## 🧠 Models

### 🔹 CNN (Poster Classification)
- Input: 64×64 RGB images
- Residual architecture
- Global Average Pooling
- Output: 25 genre probabilities (sigmoid)

### 🔹 LSTM (Overview Classification)
- TextVectorization (vocab size = 10,000)
- Embedding layer
- Bidirectional LSTM layers
- Output: 25 genre probabilities (sigmoid)

---

## 📈 Key Findings

- CNN shows **better generalisation** but struggles with recall
- LSTM captures **semantic meaning** but suffers from overfitting
- Visual and textual modalities provide **complementary information**

---

## 📁 Repository Structure
