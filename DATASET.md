# 📄 Dataset Description

## Overview

This project uses two datasets to perform and evaluate Natural Language Processing tasks such as Named Entity Recognition (NER), relation extraction, and text summarization.

---

## 📊 1. Kaggle Financial News Dataset (Financial.csv)

### Description

The primary dataset used in this project is a collection of financial news articles stored in **Financial.csv**. It contains unstructured textual data from the financial domain.

### Usage

* Named Entity Recognition (NER)
* Rule-based Relation Extraction
* Input for text summarization

### Characteristics

* Domain: Financial / News
* Data Type: Unstructured text
* Content: News articles containing entities such as organizations, people, and locations

### Preprocessing

The dataset undergoes text cleaning, including:

* Removal of unwanted characters
* Normalization of whitespace
* Standardization of text

### Limitation

This dataset does not contain reference summaries, which limits its use for direct evaluation of summarization performance.

---

## 📰 2. CNN/DailyMail Dataset (Hugging Face)

### Description

The CNN/DailyMail dataset is a widely used benchmark dataset available through Hugging Face. It contains news articles paired with human-written summaries.

### Usage

* Evaluation of summarization performance
* Calculation of ROUGE scores

### Characteristics

* Domain: General news
* Data Type: Text-summary pairs
* Contains: Articles and corresponding summaries

### Advantage

Provides high-quality reference summaries, making it suitable for evaluating abstractive summarization models.

---

## 🔍 Summary

| Dataset       | Purpose                           | Type                 |
| ------------- | --------------------------------- | -------------------- |
| Financial.csv | NER + Relation Extraction + Input | Unstructured text    |
| CNN/DailyMail | Summarization Evaluation          | Text + Summary pairs |

---

## 📌 Conclusion

The combination of a domain-specific dataset (Financial.csv) and a benchmark dataset (CNN/DailyMail) ensures both practical implementation and proper evaluation of the NLP pipeline.
