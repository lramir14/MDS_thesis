# This is the repository for my master's thesis on Data Science. 

Feel Free to explore the notebooks. 

For information about the datasets please contact me at: lfrr93@gmail.com  So I can send them to you. Otherwise they are also available on Kaggle but are set as private so I am able to invite you as a guest. 


📢 Presidential Echoes: A Systemic Analysis of López Obrador’s Conferences and News Coverage
Author: Luis Fernando Ramírez Ruiz
Program: Master of Data Science for Public Policy – Hertie School
Thesis Supervisor: Prof. Dr. Arianna Ornaghi
Thesis Date: May 2025
Repository URL: github.com/lramir14/MDS_thesis


📝 Overview
This repository contains all data processing scripts, models, and analysis pipelines used in the master's thesis "Presidential Echoes: A Systemic Analysis of López Obrador’s Conferences and News Coverage." The project investigates how Mexico’s presidential daily press conferences (2018–2024) influenced national media coverage.

Using advanced NLP techniques such as topic modeling, sentence embeddings, and cosine similarity, this work builds a framework to analyze over 2,300 presidential speeches and 36,000 news articles.

📌 Research Questions
How are Mexican media outlets covering daily presidential press conferences?

Can we quantify the semantic similarity between what the president says and what media report?

Which outlets reproduce the presidential narrative, and which deviate?

🔍 Methodology
📚 Data Collection
Presidential Speeches: Scraped from AMLO's official archive

Media Articles: Scraped from Google News using a headless Selenium-based bot with VPN support

🧹 Preprocessing
Language: Spanish (Spacy's es_core_news_md)

Custom stopword lists

Paragraph-level text chunking

🧠 NLP Techniques
Topic Modeling: LDA (Latent Dirichlet Allocation)

Embeddings: hiiamsid/sentence_similarity_spanish_es (BERT-based)

Similarity: Cosine similarity between embedded paragraphs

📈 Statistical Modeling
Fixed Effects OLS to estimate similarity across outlets

Time-Series Regression with lagged similarity

Rolling averages for temporal trend analysis
