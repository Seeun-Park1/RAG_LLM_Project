🔍 RAG-Based Chatbot with Upstage LLM
📌 Project Overview
This project is a Retrieval-Augmented Generation (RAG) chatbot built using Streamlit, Upstage LLM, and ChromaDB. It enables users to upload PDF documents and ask questions based on their content. The chatbot retrieves relevant document sections and generates accurate, context-aware responses.

The goal of this project is to improve document-based Q&A systems, making it easier to extract key information from uploaded files while maintaining conversational memory.

🚀 Key Features
📄 PDF Upload & Preview: Users can upload and view PDFs within the app.
🧠 Context-Aware Responses: Uses previous conversations to maintain continuity.
📚 RAG-based Retrieval: Extracts relevant document sections for accurate answers.
🌐 Streamlit Web Interface: Simple, interactive, and user-friendly UI.
🔧 Steps Involved
1️⃣ Document Upload & Processing
Users can upload PDF files via the Streamlit sidebar.
The app reads and processes the PDF using PyPDFLoader.
2️⃣ Vector Embedding & Retrieval
ChromaDB is used to store document embeddings.
UpstageEmbeddings converts text into vector representations for efficient retrieval.
3️⃣ Chatbot Interaction
The chatbot contextualizes user questions by referring to conversation history.
Relevant document snippets are retrieved and passed to Upstage LLM for generating responses.
4️⃣ Response Generation & Display
Answers are presented in a chat-style interface.
Users can view supporting document context through an expandable section.
⚙️ Setup Instructions
1️⃣ Clone the Repository
bash
Copy
Edit
git clone https://github.com/Seeun-Park1/RAG_LLM_Project.git
cd RAG_LLM_Project
2️⃣ Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
3️⃣ Set Up API Key
Create a .env file and add your Upstage API Key:

plaintext
Copy
Edit
UPSTAGE_API_KEY=your_api_key_here
4️⃣ Run the Streamlit App
bash
Copy
Edit
streamlit run chatbot.py
🛠 Technologies Used
📚 Libraries: Streamlit, LangChain, ChromaDB, PyPDFLoader
🤖 LLM Model: Upstage LLM for generating responses
📂 Vector Storage: ChromaDB for storing document embeddings
📌 Future Improvements
Enhance multi-document support for broader context awareness.
Improve retrieval accuracy using better embedding models.
Add user authentication for personalized document history.



```
python -m venv venv
source venv/bin/activate
pip install --upgrade --quiet  langchain langchain-community python-dotenv langchain-core langchain-upstage
python chatbot.py
```
