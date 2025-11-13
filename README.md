# 💬 Tweet Sentiment Analysis App  
A full-stack sentiment analysis application built with **Streamlit** (frontend) and **Flask** (API).  
The system allows users to explore a large tweet dataset, perform text analysis, and classify sentiment interactively.

---

## 🧭 Overview

This project combines **data exploration**, **text preprocessing**, and a **real-time polarity classifier**.

### 🧱 System Architecture

```
Streamlit UI  <───>  Flask API (/predict)
     │                    │
     │                    └── TextBlob polarity model
     │
     ├── Data Exploration (Users / Timelines / Counts)
     ├── Sentiment Distribution
     ├── Text Preprocessing & Word Frequency
     └── Tweet Sentiment Classifier (API call)
```

---

## ✨ Features

### 1️⃣ **Data Exploration**
- Browse tweet samples  
- Filter by user  
- Daily tweet volume timeline  
- Explore positive vs negative distribution  

### 2️⃣ **Text Processing**
- Emoji normalization  
- URL & username cleaning  
- Stop-word removal  
- Lemmatization  
- Word frequency analysis  
- Side-by-side visualization of negative vs positive terms  

### 3️⃣ **Sentiment Classifier**
- Type any text → gets sent to Flask API  
- Returns a **polarity score** (−1 ~ 1)  
- Uses **TextBlob** under the hood  

---

## 🛠️ Tech Stack

### Frontend
- **Streamlit**
- **Matplotlib + Seaborn**
- **NLTK** (tokenization, stopwords)

### Backend API
- **Flask**
- **TextBlob**

### Storage
- SQLite database containing tweet dataset

---

## 📷 Screenshot

<img width="827" height="409" alt="sentiment_ui" src="https://github.com/user-attachments/assets/ac558ba8-dba7-4c98-b3bf-b68a3e0eba97" />

---

## 🚀 How to Run the Project

### 1. Start the Flask API
```bash
python api.py
```

### 2. Start the Streamlit App
```bash
streamlit run app.py
```

### 3. Test sentiment in the UI
Input e.g.:
```
I really love this course!
```

---

## 📌 Project Goals
- Demonstrate a clean full-stack ML pipeline  
- Provide hands-on experience with NLP preprocessing  
- Build an interactive visual analytics tool  
- Showcase API + frontend integration for ML apps  

---

## 🧑‍💻 Author
Weilun LIN
