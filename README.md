# AI-Powered Resume to Job Matching using NLP

## 📌 Overview
This project is an **NLP-based AI tool** that matches candidate resumes to job descriptions based on skill and experience similarity.  
It uses **TF-IDF vectorization** and **cosine similarity** to rank resumes from a given dataset according to how closely they match a job posting.

Dataset Source: [Kaggle – Resume Dataset](https://www.kaggle.com/datasets/snehaanbhawal/resume-dataset)

---

## 🚀 Features
- Cleans and preprocesses raw resume text using **spaCy** (lemmatization, stopword removal, tokenization).
- Converts text into numerical features using **TF-IDF**.
- Ranks resumes by similarity to a given job description using **cosine similarity**.
- Outputs the top matching candidates with match scores.
- Easily extendable to **semantic search** with BERT or Sentence Transformers.

---

## 🛠️ Tech Stack
- **Python**
- **pandas** – Data handling
- **spaCy** – NLP preprocessing
- **scikit-learn** – TF-IDF & cosine similarity
- **KaggleHub** – Dataset download

---
## 📊 Example Output
Top Matching Candidates:
Category Match_Score
2293 ARTS 0.124965
926 AGRICULTURE 0.100726
267 INFORMATION-TECHNOLOGY 0.085227

## 📜 How to Run
1. Open in **Google Colab** or local Python environment.
2. Install dependencies:
   ```bash
   pip install pandas scikit-learn spacy kagglehub
   python -m spacy download en_core_web_sm
3.Download dataset
import kagglehub
path = kagglehub.dataset_download("snehaanbhawal/resume-dataset")

4.Run the notebook and provide your job description.

##💡 Future Improvements
-Use BERT/Sentence Transformers for semantic similarity.

-Build a Flask API for real-time resume-job matching.

-Integrate with ATS systems for HR automation.

