# 🩺 Physician Notetaker – Medical NLP Pipeline

An AI-powered **medical transcription and analysis system** that extracts structured clinical information, performs patient **sentiment & intent analysis**, and generates **SOAP notes** from physician–patient conversations using NLP and Transformer models.

---

## 📌 Project Overview

This project demonstrates how Natural Language Processing (NLP) can be applied to healthcare conversations to assist clinicians with documentation and patient understanding.

The system processes raw physician–patient dialogue and produces:
- Structured medical summaries
- Patient sentiment and intent classification
- Automated SOAP notes

---

## 🧠 Key Features

### 1️⃣ Medical NLP Summarization
- Extracts **Symptoms, Diagnosis, Treatment, Prognosis**
- Uses **spaCy** for Named Entity Recognition (NER)
- Outputs structured **JSON medical reports**

### 2️⃣ Sentiment & Intent Analysis
- Transformer-based **zero-shot classification**
- Classifies patient:
  - **Sentiment:** Anxious, Neutral, Reassured
  - **Intent:** Reporting symptoms, Seeking reassurance, Expressing concern, Providing information

### 3️⃣ SOAP Note Generation (Bonus)
- Automatically converts conversation text into:
  - Subjective
  - Objective
  - Assessment
  - Plan
- Ensures clinically readable structured output


---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Dev-debasish-09/Emitrr_Project.git
cd Emitrr_Project
```
NLP Pipeline Workflow

Text Cleaning
Removes markdown symbols and noise
Normalizes conversation text
Medical Entity Extraction
Identifies symptoms, treatments, diagnoses
Sentiment & Intent Classification
Uses Transformer zero-shot learning
SOAP Note Mapping
Classifies each sentence into SOAP categories
Aggregates into structured clinical notes


🧾 Medical Summary (JSON)
```{
  "Patient_Name": "Janet Jones",
  "Symptoms": ["Neck pain", "Back pain", "Head impact"],
  "Diagnosis": "Whiplash injury",
  "Treatment": ["10 physiotherapy sessions", "Painkillers"],
  "Current_Status": "Occasional backache",
  "Prognosis": "Full recovery expected within six months"
}```
