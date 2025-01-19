# PDF Document Q&A System with Gemini Pro


## 🚀 Overview
An AI-powered document question-answering system that leverages Google's Gemini Pro model and Cohere embeddings. Upload PDF documents and get instant, accurate answers to your questions about the content.

[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.24.0-FF4B4B.svg)](https://streamlit.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## ✨ Features
- 📄 PDF document upload and processing
- 🔍 Advanced text chunking and embedding generation
- 🔎 Semantic search using FAISS
- 💻 Interactive web interface using Streamlit
- 🤖 Real-time answer generation using Gemini Pro
- 📊 Context visualization for transparency

## 🛠️ Prerequisites
- Python 3.8 or higher
- Virtual environment (pip/conda)
- Cohere API key
- Google API key

## ⚡️ Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/VivekRajpoot01/gemini-rag.git
cd gemini-rag
```

### 2. Set Up Virtual Environment
#### Using venv
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

#### Using conda
```bash
conda create -n pdf-qa-env python=3.8
conda activate pdf-qa-env
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure API Keys
Create a `.env` file:
```env
COHERE_API_KEY=your_cohere_api_key
GOOGLE_API_KEY=your_google_api_key
```

### 5. Run the Application
```bash
streamlit run app.py
```

## 📁 Project Structure
```
gemini-rag/
│
├── app.py                 # Main application file
├── requirements.txt       # Project dependencies
├── .env                  # Environment variables
└── README.md             # Project documentation
```

## 🔧 How It Works

### Document Processing Pipeline
1. **PDF Upload**: System accepts PDF documents through web interface
2. **Text Extraction**: Uses PyPDFLoader for content extraction
3. **Chunking**: Implements RecursiveCharacterTextSplitter for text segmentation
4. **Embedding Generation**: Utilizes Cohere's embedding model
5. **Index Creation**: Builds FAISS index for similarity search

### Question Answering Flow
1. **Question Input**: User submits question
2. **Embedding Processing**: Converts question to embedding format
3. **Similarity Search**: Uses FAISS to find relevant chunks
4. **Context Assembly**: Combines relevant information
5. **Answer Generation**: Leverages Gemini Pro for response generation

## 📦 Dependencies
- `streamlit==1.24.0`
- `langchain==0.0.200`
- `langchain-community==0.0.10`
- `pypdf==3.15.0`
- `langchain-text-splitters==0.0.1`
- `langchain-cohere==0.0.3`
- `faiss-cpu==1.7.4`
- `google-generativeai==0.2.0`
- `langchain-google-genai==0.0.3`

## 🔑 Environment Variables

Required API keys:
- `COHERE_API_KEY`: For embeddings generation
- `GOOGLE_API_KEY`: For Gemini Pro model access

## 💻 Development Setup

### Setting up Development Environment
```bash
# Clone repository
git clone https://github.com/VivekRajpoot01/gemini-rag.git
cd gemini-rag

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Linux/macOS
# or
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt
```

### Development Tools
```bash
pip install black flake8 pytest
```

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License
Distributed under the MIT License. See `LICENSE` for more information.

## 🙏 Acknowledgments
- Streamlit - Web interface
- LangChain - Document processing
- Google Gemini Pro - Language model
- Cohere - Embeddings
- FAISS - Similarity search

## 📫 Contact
Vivek Rajpoot - [GitHub](https://github.com/VivekRajpoot01)

Project Link: [https://github.com/VivekRajpoot01/gemini-rag](https://github.com/VivekRajpoot01/gemini-rag)
