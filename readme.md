# 🤖 Advanced NLP: Sentiment Benchmarking Studio
### *From Statistical Baselines to Transformer-Based Attention*

## 📝 Executive Summary
This project is a comprehensive comparative study of Sentiment Analysis techniques performed on **500,000+ Amazon Fine Food Reviews**. I transitioned from traditional machine learning to deep learning to evaluate how different architectures handle linguistic nuance, negation, and context.

## 🚀 The Three "Brains"
I implemented and benchmarked three distinct modeling approaches:

1. **The Baseline (Logistic Regression + TF-IDF):** * **Result:** 93.3% Accuracy.
   * **Takeaway:** Extremely fast and efficient but lacks understanding of word order.

2. **The Sequence Expert (LSTM - Long Short-Term Memory):** * **Result:** 94.9% Accuracy.
   * **Takeaway:** Utilizes a hidden "memory" state to understand how sentiment evolves across a sentence.

3. **The Context Powerhouse (BERT/DistilBERT):** * **Result:** State-of-the-art context window.
   * **Takeaway:** Uses **Self-Attention** to link descriptors to specific subjects, identifying complex sentiment triggers.

## 🧪 The Sarcasm Challenge: A Key Finding
A critical part of this study involved "Stress Testing" the models with sarcasm. 
* **Input:** *"If you like wasting money, this is the perfect product for you."*
* **Discovery:** Despite high accuracy on standard data, even pre-trained Transformers can be "fooled" by sarcasm without domain-specific fine-tuning. This highlights the importance of **human-in-the-loop validation** for high-stakes business decisions.

## 🛠️ Tech Stack
* **Language:** Python
* **Deep Learning:** TensorFlow (Keras), PyTorch
* **NLP Tools:** Hugging Face Transformers, NLTK, Scikit-learn
* **Infrastructure:** Trained on 500k+ samples utilizing CPU-optimized batches.

## 📈 How to Use
1. Clone the repo.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run `notebooks/sentiment_benchmarking.ipynb` to see the comparative visualizations.
