# 🧠 Image Captioning Project (CNN + LSTM & CNN + Transformer)

## 📌 Project Description

This project focuses on **Image Captioning using Deep Learning**, where the goal is to automatically generate meaningful textual descriptions for images.

We implemented and compared two main architectures:
- **CNN + LSTM model**
- **CNN + Transformer model**

The CNN is used for extracting visual features from images, while the sequence models (LSTM and Transformer) are used to generate natural language captions based on those features.

Our experiments were conducted on the **Flickr8k dataset**, where each image is associated with multiple human-written captions.

The objective is to analyze which architecture produces more accurate, fluent, and context-aware captions.

---

## ⚠️ Notebook Display Notice

Some notebooks in this repository contain large outputs (images, predictions, and evaluation results).  

Due to GitHub rendering limitations, notebooks may not display correctly or fully on the website.

### ✅ Solutions:
- Download the notebooks and open them locally using Jupyter Notebook or JupyterLab.
- Or view them using Nbviewer: https://nbviewer.org/

Simply paste the GitHub notebook link into Nbviewer to see full results with outputs.

---

## 📊 Key Idea

- CNN → Extract image features  
- LSTM / Transformer → Generate captions  
- Comparison of both architectures to evaluate performance  

---

## 📂 Dataset

- Flickr8k Dataset (each image has 5 captions)

---

## 📊 Results

| Model            | BLEU-4 Score |Clider     Rougl
|-------------------|-------------|---------|-------------|
| CNN + LSTM        | 0.29        |0.31     |0.29
| CNN + Transformer | 0.29      |0.38       |0.41
## 🚀 Future Work

- Train on larger dataset (Flickr30k or MSCOCO)
- Improve Transformer architecture
- Add attention visualization
- Deploy model as a web app

  ## ⚖️ Comparison

- LSTM is sequential and slower
- Transformer uses attention and performs better on long context
- Transformer produces more accurate and fluent captions

To enhance the understanding of images, we designed a **fusion strategy** that combines the output of the image captioning model with the emotion recognition model.

---

### 🧠 Idea

Instead of treating caption generation and emotion detection separately, we merge both outputs to produce a **context-aware description of the image**.

## 🔗 Caption–Emotion Fusion Example

To clearly show the benefit of the fusion module, we compare the caption output **with and without emotion integration**.

---

### ❌ Without Emotion (Basic Captioning Output)

- Caption: *"A child playing in a park"*

👉 This output only describes the scene without any emotional context.

---

### 😊 With Emotion (Fusion Output)

- Caption: *"A child playing in a park"*
- Emotion: 😊 Happy

👉 Final Fusion Result:
> "A happy child playing in a park"

---

### 🎯 Key Difference

- Without emotion → only **visual description**
- With emotion → **description + emotional context**

This makes the generated sentence more natural, expressive, and closer to human perception.
## 🎯 Goal
To study and compare the performance of **RNN-based (LSTM)** vs **Attention-based (Transformer)** models in image caption generation.
