# 💊 Medicine Recommendation System using Machine Learning

A Content-Based Medicine Recommendation System that recommends similar medicines based on their descriptions and medical uses. The project applies Natural Language Processing (NLP) techniques to extract textual features and uses Cosine Similarity to find medicines with similar characteristics.

---

## 📌 Project Overview

Choosing an alternative medicine with similar composition or usage can be challenging. This project builds a recommendation engine that analyzes medicine descriptions and reasons (medical indications) to recommend medicines with similar properties.

The recommendation model is built using Natural Language Processing (NLP) and Machine Learning techniques.

---

## 🚀 Features

- Medicine recommendation based on similarity
- Text preprocessing using NLP
- Stemming using Porter Stemmer
- Feature extraction using CountVectorizer
- Cosine Similarity-based recommendation
- Simple and lightweight implementation
- Easily extendable to a web application

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- NLTK
- CountVectorizer
- Cosine Similarity
- Jupyter Notebook

---

## 📂 Dataset

The dataset contains information such as:

- Medicine Name
- Description
- Medical Reason / Indication

Example:

| Drug Name | Description | Reason |
|------------|-------------|--------|
| Medicine A | Antibiotic used for bacterial infection | Fever, Infection |

---

## ⚙️ Workflow

1. Load the dataset
2. Handle missing values
3. Remove duplicate records
4. Tokenize Description and Reason
5. Merge text features into a single Tags column
6. Convert text into lowercase
7. Apply stemming using Porter Stemmer
8. Convert text into numerical vectors using CountVectorizer
9. Compute Cosine Similarity
10. Recommend Top-5 similar medicines

---

## 🧠 Machine Learning Approach

This project uses a **Content-Based Filtering** recommendation system.

### NLP Pipeline

- Text Cleaning
- Tokenization
- Lowercase Conversion
- Stopword Removal (via CountVectorizer)
- Porter Stemming
- Bag of Words

### Vectorization

CountVectorizer

```python
CountVectorizer(
    stop_words="english",
    max_features=5000
)
```

### Similarity Metric

Cosine Similarity

```python
cosine_similarity(vectors)
```

---

## 📊 Recommendation Function

Input:

```
Medicine Name
```

Output:

```
Top 5 Similar Medicines
```

Example:

```
Input:
ACGEL CL NANO Gel 15gm

Output:
ACGEL NANO Gel 15gm
Acnehit Gel 15gm
Acnelak Soap 75gm
Acnetor AD 1% Ointment 15gm
Acnetor AD Cream 15Acnetor AD Gel 15gm
```

---

## 📁 Project Structure

```
Medicine-Recommendation-System/
│
├── Medicine Recommendation System.ipynb
├── medicine.csv
├── README.md
├── requirements.txt
└── LICENSE
```

---

## 📦 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Medicine-Recommendation-System.git
```

Move into the project

```bash
cd Medicine-Recommendation-System
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the notebook

```bash
jupyter notebook
```

---

## 📈 Future Improvements

- Streamlit Web Application
- Flask API
- Medicine Image Support
- Symptom-Based Recommendation
- Deep Learning Embeddings
- BERT Sentence Embeddings
- Drug Interaction Prediction
- Disease Prediction Integration

---

## 📚 Libraries Used

- pandas
- numpy
- nltk
- scikit-learn

---

## 👨‍💻 Author

Hari Narayana Rao Chepuri

If you found this project useful, don't forget to ⭐ the repository.
