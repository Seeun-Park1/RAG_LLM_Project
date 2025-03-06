# 🔍 RAG-Based Chatbot with Upstage LLM  

## 📌 Project Overview  
This project is a **Retrieval-Augmented Generation (RAG)** chatbot built using **Streamlit**, **Upstage LLM**, and **ChromaDB**.  
It enables users to upload PDF documents and ask questions based on their content.  
The chatbot retrieves relevant document sections and generates **accurate, context-aware responses**.  

The goal of this project is to improve **document-based Q&A systems**, making it easier to extract key information from uploaded files while maintaining conversational memory.  

---

## 🚀 Key Features  
- **📄 PDF Upload & Preview**: Users can upload and view PDFs within the app.  
- **🧠 Context-Aware Responses**: Uses previous conversations to maintain continuity.  
- **📚 RAG-based Retrieval**: Extracts relevant document sections for accurate answers.  
- **🌐 Streamlit Web Interface**: Simple, interactive, and user-friendly UI.  

---

## 🔧 Steps Involved  

### 1️⃣ **Document Upload & Processing**  
- Users can upload PDF files via the **Streamlit sidebar**.  
- The app reads and processes the PDF using **PyPDFLoader**.  

### 2️⃣ **Vector Embedding & Retrieval**  
- **ChromaDB** is used to store document embeddings.  
- **UpstageEmbeddings** converts text into vector representations for efficient retrieval.  

### 3️⃣ **Chatbot Interaction**  
- The chatbot **contextualizes** user questions by referring to conversation history.  
- Relevant **document snippets** are retrieved and passed to **Upstage LLM** for generating responses.  

### 4️⃣ **Response Generation & Display**  
- Answers are presented in **a chat-style interface**.  
- Users can view **supporting document context** through an expandable section.  



```
python -m venv venv
source venv/bin/activate
pip install --upgrade --quiet  langchain langchain-community python-dotenv langchain-core langchain-upstage
python chatbot.py
```
