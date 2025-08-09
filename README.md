# 🗳️ Political Sentiment & Emotion Analysis – Nepal

## Overview
The **Political Sentiment & Emotion Analysis** project is an NLP system that detects and classifies **sentiments** and **emotions** in political discourse. It processes text from **social media**, **news articles**, and **public forums** to evaluate **changes in public perception** toward major political figures **before and after elections** in Nepal.

Built with **BERT** and **RoBERTa**, the system supports **multilingual input** (Devanagari, Romanized Nepali, English) and can handle **large-scale datasets** to provide near real-time insights. This makes it valuable for tracking political trends, analyzing reactions to policies, and forecasting electoral outcomes.

---

## Features
- 🗣️ **Multi-class sentiment classification** — Positive, Negative, Neutral  
- ❤️ **Emotion detection** (anger, joy, sadness, etc.)  
- 🌐 **Multilingual support** — Devanagari, Romanized Nepali, English  
- 📊 **Pre vs Post election comparison** for public perception analysis  
- ⚡ **Real-time monitoring** for streaming data sources  
- 📈 **Visualizations** of sentiment and emotion distributions (time-series, pie charts)  
- 🗄️ **Scalable processing** for large datasets with batch & streaming modes

---

## 🛠️ Technologies Used
- **Programming Language:** Python  
- **NLP & Models:** Hugging Face Transformers — BERT, RoBERTa  
- **Frameworks:** PyTorch / Transformers
- **Data & Utils:** Pandas, NumPy, scikit-learn  
- **Visualization:** Matplotlib, Seaborn, Plotly 

---

## 🚀 Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/political-sentiment-analysis.git
    cd political-sentiment-analysis
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

---

## ▶️ Usage

- Run the analysis script:
    ```bash
    python analyze.py --input data/comments.csv --output results/
    ```

- Run the dashboard (if included):
    ```bash
    streamlit run app.py
    # or
    python run_dashboard.py
    ```

- Example arguments (replace with your file paths):
    ```bash
    python analyze.py --model roberta-base --labels mapping.json --time-split pre_post
    ```

Results and visualizations will be saved to the `results/` folder.

---

## 📚 Dataset
- Comments directed at major political figures in Nepal  
- Collected from social media platforms, news article comments, and public forums  
- Labeled with `time-period` (pre-election, post-election) for comparative study  
- Multilingual: Devanagari (Nepali script), Romanized Nepali, and English

---

## 🧠 Model Details
- **Models:** BERT and RoBERTa fine-tuned for:
  - Sentiment classification (LABEL_0 = Negative, LABEL_1 = Positive, LABEL_2 = Neutral)  
  - Emotion classification (multi-label / multi-class depending on dataset)
- **Training:** Transfer learning with class-balancing, LR scheduling, and early stopping  
- **Evaluation:** Accuracy, F1-score, Precision, Recall; confusion matrices for class insights  
- **Deployment:** Batch processing and optional streaming pipeline for real-time inference

---

## 📈 Results & Applications
- Track public opinion shifts across time and events  
- Assist policymakers and campaign teams in understanding public sentiment  
- Monitor public reaction to policy changes or announcements  
- Feed into forecasting models for election outcome analysis

---

## 🔑 Keywords
Sentiment Analysis, Emotion Detection, NLP, Text Classification, Political Monitoring, BERT, RoBERTa, Nepal

---

