# Job Recommendation System (PySpark + NLP + LSH)

A scalable Job Recommendation System built using **PySpark**, **TF-IDF**, **NLP techniques**, and **Locality Sensitive Hashing (LSH)** to process and recommend relevant job roles from a dataset of 22K+ Naukri.com job postings.

This project demonstrates distributed data processing, efficient feature engineering, and fast approximate nearest-neighbor search for large-scale recommendation systems.

---

## 🚀 Features

- Distributed NLP preprocessing using **PySpark**  
- TF-IDF vectorization on >20,000-dimensional sparse vectors  
- **LSH-based similarity search** for fast recommendations (<1 sec)
- Skill-based filtering and similarity scoring  
- Rule-based title normalization for clean output  
- Scalable pipeline that handles 20K–40K+ job records efficiently  

---

## 🧱 Tech Stack

- **PySpark**
- **Python**
- **NLP (Tokenizer, StopWordsRemover)**
- **TF-IDF (HashingTF + IDF)**
- **Locality Sensitive Hashing (LSH)**
- **Google Colab** (runtime)

---

## 📌 Project Workflow

1. Load and clean job description + skills text  
2. Apply tokenization and stopword removal  
3. Generate TF-IDF feature vectors using HashingTF (20k features)  
4. Cache transformed data for performance  
5. Train Bucketed Random Projection LSH model  
6. Convert user skills to TF-IDF vector  
7. Retrieve nearest job postings using ANN search  
8. Convert distances to similarity scores (0–1 scale)  
9. Rank top recommendations and normalize job titles  



*(Optional — add your screenshot here after adding sample_output.png)*

