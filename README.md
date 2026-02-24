# AI_Research_Paper_Analysis
AI-powered research paper analysis system using Retrieval-Augmented Generation (RAG) for structured summarization and context-aware question answering.


# ScholarRAG – AI Research Paper Analysis System

ScholarRAG is an end-to-end AI-powered system that enables structured research paper analysis using Retrieval-Augmented Generation (RAG).

It allows users to upload academic papers, generate structured summaries, and ask context-aware questions grounded strictly in the paper’s content.

---

## 🚀 Key Features

- 📄 PDF Upload & Text Extraction (PyPDF2)
- 🧠 Hybrid Section Detection (Regex + LLM Refinement)
- 📚 Topic-wise Structured Summarization
- 🔎 Semantic Search using FAISS Vector Store
- 🤖 Hallucination-Controlled Question Answering
- 🌐 Interactive Web Interface (Flask + HTML/CSS)

---

## 🏗 System Architecture

PDF Upload
↓
Text Extraction
↓
Regex Section Detection
↓
LLM-based Section Refinement
↓
Section-wise Content Mapping
↓
Embedding Generation (HuggingFace)
↓
FAISS Vector Database
↓
Context-Constrained RAG QA



---

## 🧠 Technical Highlights

- Hybrid deterministic + generative parsing pipeline
- Similarity score thresholding to reduce hallucinations
- Custom prompt engineering for strict context grounding
- Lazy initialization of vector database for efficiency
- Structured summarization with layman explanation mode

---

## 🛠 Tech Stack

- Python
- Flask
- LangChain
- FAISS
- HuggingFace Embeddings
- Groq LLM
- HTML / CSS / JavaScript

---

## 📦 Installation

```bash
git clone https://github.com/your-username/ScholarRAG.git
cd ScholarRAG
python -m venv venv
pip install -r requirements.txt


## Create .env file:

GROQ_API_KEY=your_key
LLM_MODEL=your_model_name
EMBEDDING_MODEL=your_embedding_model

## Run :
python app.py
