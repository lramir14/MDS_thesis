# 📢 Presidential Echoes: A Systemic Analysis of López Obrador’s Conferences and News Coverage

> A master's thesis on the intersection of political communication and natural language processing in Mexico (2018–2024).

---

## 🎓 Thesis Metadata

- **Author:** Luis Fernando Ramírez Ruiz  
- **Program:** Master of Data Science for Public Policy – Hertie School  
- **Thesis Supervisor:** Prof. Dr. Arianna Ornaghi  
- **Thesis Date:** May 2025  
- **Repository URL:** [github.com/lramir14/MDS_thesis](https://github.com/lramir14/MDS_thesis)  
- **Contact:** lfrr93@gmail.com  

---

## 🧭 Introduction

Welcome to the repository for my master's thesis in data science.  
Feel free to explore the Jupyter notebooks and code included in this project.

**📩 Access to Data**  
The datasets are not publicly included in the repository. If you're interested in accessing them:

- Contact me via email: `lfrr93@gmail.com`
- Alternatively, I can invite you as a guest to my private Kaggle datasets because they are set as "private" datasets. 

---

## 📝 Project Overview

This project investigates how Mexico’s daily presidential press conferences (2018–2024) influenced national media coverage.

Using advanced NLP methods — including **topic modeling**, **sentence embeddings**, and **cosine similarity** — the analysis explores how closely media outlets followed or deviated from the presidential narrative.

**Corpus Summary:**

- 🗣 **2,300+** Press conferences  
- 📰 **36,000+** News articles  

---

## 📌 Research Questions

- How are Mexican media outlets covering daily presidential press conferences?
- Can we quantify the semantic similarity between what the president says and what media outlets report?
- Which outlets reproduce the presidential narrative, and which deviate?

---

## 🔍 Methodology

### 📚 Data Collection

- **Speeches:** Scraped from [AMLO's official website](https://amlo.presidente.gob.mx/secciones/version-estenografica/)
- **News Articles:** Scraped from Google News (2018–2024) using a Selenium-based scraper with VPN access

### 🧹 Preprocessing

- Language: Spanish (`spacy` – `es_core_news_md`)
- Tokenization, stopword removal, custom filters
- Paragraph-level chunking (4 sentences per chunk)

### 🧠 NLP Techniques

- **Topic Modeling:** LDA via `scikit-learn`
- **Embeddings:** [`hiiamsid/sentence_similarity_spanish_es`](https://huggingface.co/hiiamsid/sentence_similarity_spanish_es) (BERT-based)
- **Similarity Metric:** Cosine similarity between embedded chunks

### 📈 Statistical Modeling

- **Model 1:** Fixed Effects OLS (media outlet, month/year dummies)
- **Model 2:** Time-Series Regression with lagged similarity variables
- **Additional:** Rolling average trends, residual diagnostics, clustering

---

## 📊 Key Findings

- Media outlets on average followed the **presidential narrative**, with a similarity score of ~**0.30**
- **Infobae** and **Proceso** consistently **diverged**, suggesting more critical editorial stances
- **Similarity increased over time**, especially in 2023–2024, indicating growing narrative alignment
- Results suggest that the **impact of press conferences is measurable and non-trivial**, but not uniformly strong

---

## 📁 Repository Structure

