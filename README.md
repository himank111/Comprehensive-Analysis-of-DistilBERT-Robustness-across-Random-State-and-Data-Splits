# 💬 BERT-vs-DistilBERT-Sentiment-Analysis  

## 📌 Overview  
This project compares **BERT** and **DistilBERT** on a **product reviews dataset** for **sentiment analysis**.  
It demonstrates that **DistilBERT performs nearly identically to BERT** on small datasets while being **faster and more efficient**, followed by a **robustness analysis** across multiple data splits and random states.  

---

## 🧠 Objective  
To evaluate how **model size** impacts performance in sentiment classification and determine whether **lighter models like DistilBERT** can match **BERT’s accuracy** on limited data.  

---

## 📊 Dataset  
- **Type** → Product reviews dataset  
- **Task** → Sentiment classification (Positive / Neutral / Negative)  
- **Size** → Small-scale dataset for lightweight testing  
- **Preprocessing** → Text cleaning, tokenization using Hugging Face Transformers  

---

## ⚙️ Approach  
- **Models Used** →  
  - `bert-base-uncased`  
  - `distilbert-base-uncased`  
- **Frameworks** → PyTorch, Hugging Face Transformers  
- **Training Details** →  
  - Tokenization with padding/truncation  
  - 80/20, 70/30, and 60/40 train-test splits  
  - Evaluation metrics: Accuracy, F1-Score  
- **Robustness Check** → Performance consistency across different random states and splits  

---

## 🏆 Results  

| Model         | Accuracy | F1 Score | Notes                      |
|----------------|-----------|-----------|-----------------------------|
| **BERT**       | ~98.5%    | ~98.5%    | Baseline model              |
| **DistilBERT** | ~98.4%    | ~98.4%    | Similar performance, faster |

➡️ **DistilBERT achieved the same performance as BERT on small datasets while being faster and lighter.**  

---

## 📈 Observations  
- Minimal performance gap between BERT and DistilBERT  
- DistilBERT shows **robust performance** across different data splits  
- Ideal choice for **resource-constrained** environments  

---

## 👨‍💻 Contributors  
- [**Himank Xavier Soren**](https://github.com/himank111)  
