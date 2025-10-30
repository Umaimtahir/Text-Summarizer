# 🎯 BERT-Based Sentiment Classification with Gradio Interface

This project implements a **BERT-powered Sentiment Analysis System** that classifies text statements into *Positive*, *Negative*, or *Neutral* sentiments.  
It combines the power of **Transformer-based NLP** with an elegant **Gradio Web UI**, allowing users to interactively test statements and visualize predictions side by side.

---

## 🚀 Features

✅ Fine-tuned **BERT model** (`bert-base-uncased`) for sentiment classification  
✅ Fully implemented **training, validation, and testing pipeline** using PyTorch  
✅ Smart **DataLoader with stratified splits** for balanced training  
✅ **Performance metrics**: accuracy, precision, recall, F1-score  
✅ Clean and minimal **Gradio Interface** for real-time predictions  
✅ Optional **debug mode** for quick inspection of model confidence  

---

## 🧠 Tech Stack

| Component | Technology |
|------------|-------------|
| Language | Python 3.12 |
| Model | BERT (Hugging Face Transformers) |
| Framework | PyTorch |
| Tokenizer | AutoTokenizer (bert-base-uncased) |
| UI | Gradio |
| Data Handling | Pandas, scikit-learn |
| Metrics | sklearn.metrics |

---

## 📁 Project Structure

📦 sentiment-analysis-bert
├── 📄 Text Summarizer.ipynb # Training and validation logic
├── 📄 requirements.txt # Required dependencies
├── 📄 README.md # Project documentation
└── 📂 checkpoints/ # Saved model weights and tokenizer


---

## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/bert-sentiment-analysis.git
   cd bert-sentiment-analysis

2.Install dependencies

pip install -r requirements.txt


3.Train or load model

python Text Summarizer.ipynb

(Or use your pre-trained checkpoint in /checkpoints)

Open the web interface

The Gradio UI will open automatically in your browser.

Type a sentence and see the real-time predicted sentiment.

🧩 Example Predictions

| Statement                            | Predicted Sentiment |
| ------------------------------------ | ------------------- |
| “I love this product!”               | 😊 Positive         |
| “This is the worst experience ever.” | 😡 Negative         |
| “It’s okay, not too bad.”            | 😐 Neutral          |

🧪 Sample Test Cases

| Input Sentence                        | Expected Output |
| ------------------------------------- | --------------- |
| “The movie was absolutely wonderful!” | Positive        |
| “I hate waiting in long lines.”       | Negative        |
| “It was an average experience.”       | Neutral         |
| “I’m impressed with the quality!”     | Positive        |
| “Not what I expected at all.”         | Negative        |

🖥️ Gradio Interface (Dark UI)

.✨ Clean dark theme
.🧩 Side-by-side layout for input/output
.⚙️ Custom slider with range 10–100 for confidence threshold
.🐞 “Debug” toggle to display raw model scores

📊 Model Performance (Example)
| Metric    | Score |
| --------- | ----- |
| Accuracy  | 92.4% |
| Precision | 91.8% |
| Recall    | 93.2% |
| F1-score  | 92.5% |
