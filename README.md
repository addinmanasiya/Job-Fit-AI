# 📄 Resume Classifier

A machine learning web app that automatically **classifies resumes** into professional categories (like *Data Science*, *HR*, *Java Developer*, etc.) and evaluates how well a resume matches a **job description** based on **skills and specialization alignment**.

---

## 🚀 Features

- 📂 Upload a PDF resume and classify it into one of 25+ job categories using a trained neural network.
- 🎯 Match resumes with a job posting and compute a **skill similarity score**.
- ✅ See if the resume fits the selected job role based on specialization and keyword matching.
- 💡 Built using TensorFlow, TF-IDF, and Gradio for a user-friendly UI.

---

## 🧠 How It Works

1. **Text Preprocessing**: Resume text is cleaned, lowercased, and stopwords are removed.
2. **TF-IDF Vectorization**: Converts resumes into a matrix of important terms (top 5,000).
3. **Neural Network Model**: A deep learning model is trained to classify resumes based on job category.
4. **Skill Extraction**: Compares skills in the resume with those in the job description.
5. **Similarity Score**: Calculates how closely the resume matches the job posting based on shared skills.

---

## 🛠️ Tech Stack

- **Languages & Tools**: Python, Google Colab, Gradio
- **Libraries**: 
  - `TensorFlow`, `Keras` – for building and training the neural network
  - `Scikit-learn`, `TF-IDF` – for feature extraction and encoding
  - `NLTK` – for text cleaning and stopword removal
  - `PyMuPDF`, `PyPDF2` – for PDF text extraction
  - `Gradio` – for building the interactive web interface

---

## 📦 Installation

### 🔗 Option 1: Run in Google Colab

> [Click here to open in Google Colab](https://colab.research.google.com/drive/1yr3OmmWI-XpxcfLv-D0z8on9RZbt7IkJ)

No setup needed — all dependencies will be installed in the notebook.

### 💻 Option 2: Run Locally

```bash
git clone https://github.com/your-username/ResumeClassifier.git
cd ResumeClassifier

# Install dependencies
pip install PyPDF2 gradio-pdf pymupdf nltk joblib tensorflow pandas scikit-learn numpy gradio

# Run the app (if separated as a .py script)
python ResumeClassifier.py
