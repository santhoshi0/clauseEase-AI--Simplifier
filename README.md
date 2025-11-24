ClauseEase: AI-Based Contract Language Simplifier

    "Clear Contracts. Confident Decisions."



ClauseEase is an AI-driven solution designed to bridge the gap between complex legal documents and the general public. It automates the extraction, analysis, and simplification of legal clauses into plain English, fostering transparency and enabling informed decision-making for non-lawyers, business professionals, and legal researchers.

📑 Table of Contents

    .Abstract
    .Key Features
    .System Architecture
    .AI & NLP Models
    .Tech Stack
    .Installation & Setup
    .Screenshots
    .Future Enhancements
    .Team
    .References

📝 Abstract

Legal contracts are often written in dense, specialized jargon that creates barriers for individuals without legal expertise. ClauseEase addresses this by leveraging advanced NLP (Natural Language Processing) to:

    1.Ingest documents (PDF, DOCX, TXT).
    2.Detect and classify legal clauses.
    3.Recognize specific legal terminology.
    4.Rewrite complex text into understandable plain English while preserving legal intent.

✨ Key Features

    📄 Multi-Format Ingestion: Supports uploading of PDF, DOCX, and TXT files.
    🔍 Automated Clause Detection: Identifies and categorizes specific legal clauses using BERT/T5 architectures.
    🧠 Legal Term Recognition: Flags complex legal terminology and provides definitions/context using spaCy.
    ✍️ Language Simplification: Translates intricate legal text into plain English using Transformer models.
    📊 Report Generation: Produces downloadable reports and visual analytics of the contract analysis.
    🔐 User Authentication: Secure login and data management via JWT and Firebase.
    🎛️ Admin Dashboard: A managed panel for reviewing analysis history and user activities.

🏗 System Architecture

  ClauseEase employs a multi-layered architecture:

    Frontend: HTML/CSS/JavaScript interface for user interaction.
    Backend: Flask (Python) server acting as the central hub/API.
    AI Engine: Orchestrates calls to Hugging Face Transformers and NLP libraries.
    Database: Google Firebase Cloud Firestore (NoSQL) for real-time data synchronization and storage.

🤖 AI & NLP Models

The core intelligence of ClauseEase is built upon the following specific models and libraries:
Module 	Model / Technology 	Purpose
Clause Detection 	google/flan-t5-small 	Classifies text into specific legal clause categories.
Simplification 	prajjwall/bert-mini 	Rewrites complex sentences into plain English.
Term Recognition 	en_core_web_sm (spaCy) 	Named Entity Recognition (NER) for legal terms.
🛠 Tech Stack
Backend & AI

    Language: Python
    Framework: Flask
    ML Frameworks: PyTorch, Transformers (Hugging Face), spaCy, NLTK
    Libraries: numpy, scikit-learn, fitz (PyMuPDF), python-docx, matplotlib

Frontend

    Core: HTML5, CSS3, JavaScript
    Interaction: REST API calls via Fetch

Database & Cloud

    Database: Google Firebase (Cloud Firestore)
    Auth: Json Web Token (JWT)

🚀 Installation & Setup
Prerequisites

    Python 3.10 or higher
    pip (Python Package Manager)
    A Google Firebase project with Firestore enabled.

Steps

Clone the Repository

git clone 

Create a Virtual Environment

python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

Install Dependencies

pip install -r requirements.txt

Ensure your requirements.txt includes: flask, firebase-admin, torch, transformers, nltk, spacy, pymupdf, python-docx, numpy, scikit-learn....

Download NLP Models

# Download the spaCy model
python -m spacy download en_core_web_sm

Configure Firebase

    Download your serviceAccountKey.json from Firebase Console.
    Place it in the root directory or configure the path in app.py.

Run the Application

python app.py

    Access the app at http://127.0.0.1:3000.

📸 Screenshots
1. Home Page  <img width="1919" height="1029" alt="517728424-075350ee-b798-4d7c-bfc6-216596b2a4f8" src="https://github.com/user-attachments/assets/03aca0b5-51d0-446f-ae97-2407266e9703" />
2. Analysis Results <img width="1919" height="1030" alt="517728271-3fcae6de-a1b0-47f0-b1d2-074cfe9086c1" src="https://github.com/user-attachments/assets/9c9eb604-7e40-45c2-8c54-0c2cf2e0498b" />
3. See History  <img width="1919" height="1030" alt="517728464-5e256022-f49e-4da7-983c-1fb52bd89f5f" src="https://github.com/user-attachments/assets/6e8ad648-c3d0-457d-9685-e6bd6a4250dd" />
4.Admin Dashboard  <img width="1655" height="1028" alt="517728590-a5d70914-1048-4c31-af57-06625bdd0d6d" src="https://github.com/user-attachments/assets/d1a0cffb-4500-47a7-ba47-1751402e06a4" />

🔮 Future Enhancements

    Multilingual Support: Extending models to handle non-English contracts.
    Real-time Comparison: Comparing clauses across different document versions.
    Legal Chatbot: Integration of a conversational AI assistant for specific legal queries.
    Docker Support: Full containerization for easier deployment.

Mentor: Dr. A. Kalaivani
📚 References

    Devlin, J., et al. "BERT: Pre-training of deep bidirectional transformers." (2019).
    Google AI. "Text-to-Text Transfer Transformer (T5)." (2020).
    Explosion AI. "spaCy: Industrial-strength NLP."
    Hugging Face. "Transformers Documentation."
