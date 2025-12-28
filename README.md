---
title: DocPilotAI – RAG-Based PDF Chatbot
emoji: 📘
colorFrom: indigo
colorTo: blue
sdk: gradio
sdk_version: 6.2.0
app_file: app.py
pinned: false
---

# 📘 DocPilotAI – RAG-Based PDF Chatbot

**DocPilotAI** is a web-based **Retrieval-Augmented Generation (RAG)** chatbot designed to help users interact with academic PDF documents more effectively. Instead of manually searching through lengthy files, users can upload multiple PDFs and ask questions to receive **accurate, context-aware answers** strictly grounded in the document content.

The chatbot focuses on **clear understanding**, providing **example-based explanations** for theoretical and computer science concepts. When the document content is programming-related, DocPilotAI generates **code-based explanations** aligned with the source material. Users can also **download generated answers as a PDF**, making it suitable for academic study and documentation.

---

## 🏛 Architecture Overview

- **Frontend**: Gradio Blocks UI (`app.py`)  
- **Document Processing**:
  - PDF text extraction using PyPDF2  
  - Text chunking for efficient retrieval  
- **Retrieval Layer**:
  - Keyword-based relevance matching  
  - Top relevant chunks selected per query  
- **Generation Layer**:
  - Groq LLM API (Llama 3)  
  - Document context injected into prompts  
- **Export**:
  - AI-generated answers downloadable as PDF  

This architecture ensures responses remain **document-grounded**, modular, and easy to extend.

---

## 🌟 Key Features

- Upload and query multiple PDF documents  
- Retrieval-Augmented Generation (RAG) pipeline  
- Context-aware answers strictly based on document content  
- Example-driven explanations for concepts  
- Code-based explanations for programming topics  
- Download AI-generated answers as a PDF  
- Clean, student-friendly Gradio interface  

---

## 🛠 Tech Stack

- **Python**
- **Gradio**
- **Groq API (Llama 3)**
- **PyPDF2**
- **FPDF**
- **Hugging Face Spaces**

---

## 🎓 Academic Context

This project was developed as part of a semester coursework with the objective of building an **intelligent document-based question answering system** using Retrieval-Augmented Generation and modern large language models.

A complete demo video demonstrating the functionality of DocPilotAI is included with the project submission.

---

## ⚠️ Notes

- DocPilotAI answers questions **only from the uploaded PDF content**  
- External knowledge is not used to avoid hallucinations  
- API keys are managed securely using Hugging Face Secrets  

---

🙏 **Special Thanks To:**  
👨‍🏫 **Dr. Muhammad Nadeem Majeed (PMP®)** – Instructor  
🎓 **Hussain Raza** – Teaching Assistant  
🎓 **Amos Shehzad** – Teaching Assistant  

---

## 📌 Author

**Annas Sharif**  
Developed as part of an academic lab project using Python, Gradio, and Groq API.
