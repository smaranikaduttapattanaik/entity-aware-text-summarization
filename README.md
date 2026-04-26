# 📄 Entity-Aware Text Summarization using NLP

## 📌 Overview
This project presents an NLP-based pipeline for processing unstructured news text. It combines **Named Entity Recognition (NER)**, **relation extraction**, and **abstractive summarization** to generate meaningful summaries while preserving important information.

The system is designed to ensure that key entities from the original text are retained in the generated summary.

---

## 🎯 Objectives
- Extract important entities from text using NLP
- Identify relationships between entities
- Generate concise summaries of news articles
- Evaluate summary quality using standard and custom metrics

---

## ⚙️ Features
- 🧹 Text preprocessing and cleaning
- 🧠 Named Entity Recognition using spaCy (`en_core_web_trf`)
- 🔗 Rule-based relation extraction
- ✨ Abstractive summarization using BART (`facebook/bart-large-cnn`)
- 📊 Evaluation using:
  - ROUGE Score
  - Entity Coverage (custom metric)

---

## 🗂️ Dataset
- **File:** `Financial.csv`
- Contains financial/news articles used for text mining and summarization
- Text is preprocessed before applying NLP techniques

---

## 🏗️ Project Pipeline
1. Data Loading
2. Text Cleaning & Preprocessing
3. Named Entity Recognition (NER)
4. Relation Extraction (rule-based)
5. Text Summarization (BART model)
6. Evaluation (ROUGE + Entity Coverage)

---

## 📊 Evaluation Metrics

### 🔹 ROUGE Score
Measures similarity between generated and reference summaries:
- ROUGE-1 (unigram overlap)
- ROUGE-2 (bigram overlap)
- ROUGE-L (longest common sequence)

### 🔹 Entity Coverage
Measures how many important entities from the original text are preserved in the summary.

**Formula:**coverage = (# entities in summary ∩ original entities) / total original entities

---

## 📈 Results
- Generated summaries are coherent and meaningful
- Important entities are largely retained
- ROUGE scores indicate reasonable performance

---

## ⚠️ Limitations
- Rule-based relation extraction may miss complex relationships
- No fine-tuning of the summarization model
- Limited dataset size
- Input truncation due to model constraints

---

## 🚀 Future Improvements
- Use deep learning for relation extraction
- Fine-tune BART on domain-specific datasets
- Increase dataset size
- Add advanced evaluation metrics like BERTScore

---

## 🛠️ Technologies Used
- Python
- spaCy
- Hugging Face Transformers
- rouge_score
- pandas

---

