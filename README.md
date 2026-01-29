## 📌 Project Overview

- Word-level **LSTM language model**
- Trained on ~6,400 dialogue lines
- Generates next-word predictions
- Uses **temperature-based sampling** for controlled randomness
- Designed to run on **CPU**

---

## 🧠 Model Architecture

- **Embedding Layer** – converts words into dense vector representations  
- **LSTM Layer** – learns sequence and context information  
- **Dense + Softmax Layer** – predicts probability distribution over vocabulary  

This is a classic neural language modeling approach suitable for learning dialogue structure.

---

## ✨ Features

- Character-style dialogue generation  
- Temperature control for creativity vs stability  
- Short, sitcom-like sentence generation  
- Lightweight and CPU-friendly  
- Clean and reproducible training pipeline  

---

## ⚙️ Requirements

- Python 3.8+
- TensorFlow
- NumPy
- Pandas

Install dependencies using:
```bash
pip install -r requirements.txt
🚀 How to Run
1. Train the model
python train.py
2. Generate text
generate_text("jake peralta", 14, temperature=0.85)
generate_text("captain holt", 10, temperature=0.5)
Temperature guide:

0.5 – 0.6 → controlled, formal (Captain Holt)

0.8 – 0.9 → creative, chaotic (Jake Peralta)

📊 Training Details
Dataset size: ~6,461 dialogue lines

Epochs: 25

Batch size: 64

Final loss: ~2.7

Final accuracy: ~43%

These results align with the practical performance limits of word-level LSTM models.

⚠️ Limitations
Grammar is not always perfect

Long-range coherence degrades after ~15–20 words

Punchlines are inconsistent

These limitations are inherent to word-level LSTM architectures and are discussed in the project design.

📁 Dataset Notice
The dataset is not included due to copyright restrictions

This project is intended strictly for educational purposes

👤 Author

Himanshu Thakkar

Jash Vakharia
