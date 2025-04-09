# ⚡ RAG Chatbot with Groq, LangChain & Streamlit

A lightning-fast AI chatbot powered by **Groq's LPU** and **LangChain RAG**, delivering real-time answers from web documents. Built with Python and Streamlit.



## 🌟 Features

- **Blazing-fast responses** using Groq's Mistral-Saba-24b (or Llama 3)
- **Retrieval-Augmented Generation (RAG)** with LangChain
- **FAISS vector store** for efficient similarity search
- **Ollama embeddings** for local text processing
- **Streamlit UI** for easy interaction

## 🛠️ Tech Stack

| Component       | Technology |
|----------------|------------|
| LLM            | Groq API (Mistral-Saba-24b/Llama 3) |
| Framework      | LangChain |
| Vector Store   | FAISS |
| Embeddings     | OllamaEmbeddings |
| UI             | Streamlit |

## 🚀 Quick Start

### Prerequisites
- Python 3.10+
- [Groq API Key](https://console.groq.com/)
- Ollama (for local embeddings) [Install Guide](https://ollama.ai/)

### Installation
```bash
git clone https://github.com/yourusername/rag-groq-chatbot.git
cd rag-groq-chatbot
pip install -r requirements.txt



Configuration
1. Add your Groq API key to .env:

    GROQ_API_KEY=your_api_key_here

2. (Optional) Change the default URL in app.py to your target website.

Run the App

    streamlit run app.py

📂 Project Structure

    .
    ├── app.py                # Streamlit application
    ├── requirements.txt      # Python dependencies
    ├── .env.example          # Environment template
    └── README.md

🤖 How It Works
Loads documents from a URL using WebBaseLoader

Splits text into chunks with RecursiveCharacterTextSplitter

Generates embeddings via OllamaEmbeddings

Stores vectors in FAISS for semantic search

Answers queries using Groq's LLM with relevant context
