# 🖼️ Image Captioning with ResNet50 + LSTM (Flickr8k)

This project implements an image captioning model using an **Encoder-Decoder architecture**, where a **pretrained ResNet-50** CNN is used to extract image features and a **stacked LSTM** network generates textual descriptions. The model is trained and evaluated on the **Flickr8k dataset**, achieving a **BLEU-1 score of 62%** and **BLEU-2 score of 41%**, surpassing the original benchmark.

## 📌 Features

- 🧠 Encoder-Decoder architecture using ResNet-50 + LSTM
- 📊 BLEU score evaluation
- 🔤 Tokenization and padding of captions
- 📁 Data pipeline with preprocessing and feature extraction
- 🧪 Training visualization and performance tracking

---

## 📁 Dataset

- **Flickr8k Dataset**  
  - 8,000 images
  - 5 human-annotated captions per image  
  - Download link: [Flickr8k Dataset](https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_Dataset.zip)  
  - Captions: [Flickr8k Text](https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_text.zip)

---

## 🛠️ Technologies Used

- Python
- TensorFlow & Keras
- ResNet-50 (pretrained on ImageNet)
- LSTM for sequence generation
- Numpy, Matplotlib, Pickle, tqdm

---

## 🧮 Model Architecture

### Encoder:
- Pretrained **ResNet-50** with final classification layer removed
- Extracted 2048-dimension feature vectors

### Decoder:
- **Embedding layer** for word vectors
- **Stacked LSTM layers**
- **Dense layers** to predict the next word in sequence

---

## 📊 Results

| Metric   | Score |
|----------|-------|
| BLEU-1   | 62%   |
| BLEU-2   | 41%   |
| BLEU-3   | 27%   |
| BLEU-4   | 18%   |

> ✨ Scores surpass the original paper which achieved BLEU-1 of 61% and BLEU-2 of 41%.

---

