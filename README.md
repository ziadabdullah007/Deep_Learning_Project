# 🍽️ Multi-Model Food Image Captioning & Recommendation System

An advanced Deep Learning project that generates AI-powered food descriptions and recommends visually similar dishes using multiple CNN + RNN architectures.

This project compares different Computer Vision and NLP pipelines for food understanding and caption generation.

---

# 🚀 Project Overview

This system allows users to:

- Upload a food image
- Generate an automatic food description
- Recommend visually similar dishes
- Compare multiple Deep Learning models side-by-side

The project combines:

- Computer Vision (CNN)
- Natural Language Generation (RNN)
- Attention Mechanisms
- Recommendation Systems
- Multi-Model Comparison GUI

---

# 🧠 Models Used

## 🔹 Model 1 — EfficientNetB0 + BiLSTM

- CNN Backbone: EfficientNetB0
- Sequence Model: Bidirectional LSTM
- Lightweight baseline model

---

## 🔹 Model 2 — ResNet50 + Attention BiLSTM

- CNN Backbone: ResNet50
- Stacked Bidirectional LSTM
- Attention Mechanism
- Better contextual caption generation

---

## 🔹 Model 3 — EfficientNetB3 + BiGRU + MultiHeadAttention

- CNN Backbone: EfficientNetB3
- Stacked Bidirectional GRU
- MultiHead Attention
- Best overall architecture

---

# 📌 Features

✅ Food Image Caption Generation  
✅ AI Menu Description Generation  
✅ Similar Dish Recommendation  
✅ Multi-Model Comparison  
✅ Attention Mechanisms  
✅ MultiHeadAttention  
✅ Mixed Precision Training  
✅ Data Generator Pipeline  
✅ Gradio GUI  
✅ GPU Optimized Training  

---

# 🖼️ Example

## Input Food Image

<p align="center">
  <img src="examples/food_example.jpg" width="400">
</p>

---

## 🧠 Generated Captions

### 🔹 EfficientNetB0 + BiLSTM

```text
Fresh vegetable salad with creamy garlic dressing.
```

---

### 🔹 ResNet50 + Attention BiLSTM

```text
Roasted eggplant served with fresh vegetables and herbs.
```

---

### 🔹 EfficientNetB3 + BiGRU + MultiHeadAttention

```text
Mediterranean roasted vegetables topped with creamy garlic sauce and fresh herbs.
```

---

# 🍽️ Recommended Dishes

```text
1. Mediterranean Eggplant Salad
2. Roasted Garlic Vegetable Bowl
3. Greek Style Garden Salad
4. Fresh Herb Veggie Plate
5. Grilled Vegetable Medley
```

---

# 🏗️ Project Architecture

## CNN Feature Extraction

Food images are processed using pretrained CNN models:

- EfficientNetB0
- ResNet50
- EfficientNetB3

Extracted visual embeddings are used for:
- Caption Generation
- Recommendation System

---

## NLP Caption Generation

The extracted image features are passed into:

- BiLSTM
- Attention BiLSTM
- BiGRU + MultiHeadAttention

to generate natural language descriptions.

---

## Recommendation System

The system uses:

- Cosine Similarity
- Visual Embeddings

to recommend visually similar dishes.

---

# 📂 Project Structure

```bash
project/

│
├── models/
│   ├── efficientnet_b0/
│   ├── resnet50/
│   └── efficientnet_b3/
│
├── notebooks/
│   ├── feature_extraction.ipynb
│   ├── training.ipynb
│   └── inference.ipynb
│
├── gui/
│   └── gradio_app.py
│
├── examples/
│   └── food_example.jpg
│
├── outputs/
│
└── README.md
```

---

# 📊 Technologies Used

## Deep Learning
- TensorFlow
- Keras

## Computer Vision
- EfficientNet
- ResNet50

## NLP
- BiLSTM
- BiGRU
- Attention
- MultiHeadAttention

## Recommendation
- Cosine Similarity

## GUI
- Gradio

## Data Processing
- NumPy
- Pandas
- Scikit-learn

---

# ⚡ Training Optimizations

The project includes several optimizations:

- Mixed Precision Training
- Data Generators
- GPU Optimization
- Batch Streaming
- Early Stopping
- Model Checkpoints

---

# 📈 Challenges Solved

## Memory Optimization

Large sequence datasets caused RAM crashes.

### ✅ Solution
- DataGenerator Pipeline
- Mixed Precision Training

---

## Caption Repetition

Generated captions sometimes repeated words excessively.

### ✅ Solution
- Top-K Sampling
- Temperature Sampling
- Caption Cleaning Pipeline

---

## Weak Natural Language Descriptions

Ingredient-based captions were too raw.

### ✅ Solution
- Attention Mechanisms
- MultiHeadAttention
- Improved Caption Cleaning

---

# 💻 GUI Demo

The project includes a professional Gradio interface for:

- Uploading food images
- Comparing all models
- Viewing captions
- Viewing recommendations
- Comparing inference speed

---

# 📦 Installation

```bash
pip install tensorflow
pip install gradio
pip install pandas
pip install numpy
pip install scikit-learn
pip install pillow
```

---

# ▶️ Run The GUI

```bash
python gradio_app.py
```

---

# 📚 Dataset

The dataset contains:

- Food images
- Titles
- Ingredients
- Recipes / Descriptions

Used for:
- Caption Generation
- Recommendation System Training

---

# 🎯 Future Improvements

- Transformer Decoder
- Vision Transformers (ViT)
- Beam Search Decoding
- BLEU / ROUGE Evaluation
- Attention Visualization
- Full Recipe Generation

---

# 👨‍💻 Author

## Ziad Abdullah

Computer Science Student  
Junior Data Scientist & Deep Learning Enthusiast

---

# ⭐ GitHub

If you like this project, consider giving it a star ⭐
