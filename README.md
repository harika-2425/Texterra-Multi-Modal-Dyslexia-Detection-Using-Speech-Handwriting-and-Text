# Texterra-Multi-Modal-Dyslexia-Detection-Using-Speech-Handwriting-and-Text
# Texterra: Multi-Modal Dyslexia Detection System

Texterra is a web-based, intelligent diagnostic platform designed for the early detection of dyslexia in children aged 6–12. By combining reading, dictation, and handwriting analysis into one unified interface, Texterra supports educators and parents in identifying learning difficulties through measurable, interpretable, and actionable insights.

---

## 🧠 What is Dyslexia?

Dyslexia is one of the most common and misdiagnosed learning disorders, affecting the ability to read, write, spell, and pronounce words accurately. Early intervention is critical to prevent academic delays and emotional distress. Texterra bridges the gap between early detection and practical intervention through a digital, accessible, and multi-modal platform.

---

## 🚀 Features

- 📚 **Reading Assessment**: Evaluates pronunciation accuracy using SpeechRecognition and Levenshtein distance.
- ✍️ **Dictation Module**: Tests listening and spelling accuracy using offline text-to-speech via pyttsx3.
- 📝 **Handwriting Evaluation**: Uses Google Vision API for OCR and evaluates spelling, grammar, and phonetics.
- 📊 **Report Generation**: Automatically compiles test results into downloadable PDF and CSV reports.
- 🔐 **User Management**: Assigns unique IDs to students and tests for consistent progress tracking.
- 🧮 **Machine Learning Integration**: Decision Tree Classifier predicts dyslexia probability using annotated writing data.
- 💾 **Lightweight Storage**: All data stored locally using SQLite for portability and ease of use.

---

## 🛠️ Tech Stack

- **Frontend**: Streamlit, HTML, CSS, Bootstrap  
- **Backend**: Python  
- **Libraries Used**:
  - `SpeechRecognition`
  - `pyttsx3`
  - `Levenshtein`
  - `google.cloud.vision` (OCR)
  - `sklearn` (DecisionTreeClassifier)
  - `sqlite3`
  - `reportlab` & `csv` for report generation

---

## 🧪 Project Structure

Texterra/
│
├── data/ # Datasets for reading and writing modules
├── modules/
│ ├── pronunciation.py # Pronunciation test logic
│ ├── dictation.py # Dictation test logic
│ ├── handwriting.py # OCR and evaluation logic
│ └── classifier.py # ML model training and prediction
│
├── reports/ # Generated PDF and CSV files
├── database/
│ └── texterra.sqlite # SQLite database storing test data
│
├── app.py # Main Streamlit application
├── requirements.txt # All required libraries
└── README.md # This file
