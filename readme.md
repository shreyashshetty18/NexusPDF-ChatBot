# 🧠 NexusPDF Chatbot

**MultiPDF Chatbot** is an AI-powered assistant that allows users to query and extract information from multiple PDF documents using natural language. It leverages semantic search and large language models (LLMs) to provide accurate, context-aware answers from document content—making it ideal for research, business, legal, and technical applications.

## 🔗 Live Link -> https://nexuspdf-chatbot-multipdf.streamlit.app/
---

## 🚀 Features

* 📄 Upload and query multiple PDF documents
* 🔍 Semantic search using vector embeddings
* ⚡ Fast and relevant responses via LLMs
* 🖥️ User-friendly web interface with Streamlit

---

## 🛠️ Tech Stack

| Category           | Tools / Libraries                                             |
| ------------------ | ------------------------------------------------------------- |
| Language           | Python 3.8+                                                   |
| Frontend           | Streamlit                                                     |
| PDF Processing     | PyPDF2                                                        |
| Embedding Models   | Sentence Transformers (e.g., Sentence-BERT from Hugging Face) |
| Vector Database    | FAISS (Facebook AI Similarity Search)                         |
| LLM Integration    | LangChain, ChatGroq (LLaMA-3.3-70B)                           |
| Environment Config | python-dotenv for secure API key management                   |

---

## 🧱 System Architecture

1. **PDF Upload** – Users upload one or more PDF documents.
2. **Text Extraction** – Raw text is extracted from each file.
3. **Chunking & Preprocessing** – Extracted text is cleaned and split into smaller segments.
4. **Embedding Generation** – Chunks are embedded into vector representations using transformer models.
5. **Storage** – Embeddings are stored in a FAISS vector index for efficient retrieval.
6. **Query Handling** – User queries are transformed into embeddings.
7. **Semantic Retrieval** – Similar chunks are retrieved based on vector similarity.
8. **Answer Generation** – An LLM generates answers using retrieved chunks as context.
9. **Chat Interface** – Users interact through a Streamlit-based conversational UI.

---

## 💻 Installation & Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/multipdf-chatbot.git
cd multipdf-chatbot

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Set environment variables
cp .env.example .env
# Add your API keys to .env

# Run the application
streamlit run app.py
```

---

## 🧰 Dependencies

* `streamlit`
* `pypdf2`
* `sentence-transformers`
* `faiss-cpu`
* `langchain`
* `chatgroq`
* `python-dotenv`

---

## 📎 Use Cases

* Academic research
* Legal document analysis
* Business report querying
* Multi-document knowledge extraction
* Internal enterprise documentation search

