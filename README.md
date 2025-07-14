# RAG-Summarization-Engine-Using-LangChain

A Retrieval-Augmented Generation (RAG) application for intelligent task summarization using LangChain and Streamlit.

## 🚀 Features

- **RAG-powered Summarization**: Combines document retrieval with generative AI for context-aware task summaries
- **Web Interface**: User-friendly Streamlit interface for easy interaction
- **Document Processing**: Supports various document formats and web scraping
- **Real-time Processing**: Interactive chat interface for dynamic task summarization
- **Customizable Models**: Support for different LLMs including Groq

## 📋 Prerequisites

- Python 3.8 or higher
- pip package manager
- Git

## 🛠️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/HassamUmar/RAG-TaskSummarizer.git
cd RAG-TaskSummarizer
```

### 2. Create Virtual Environment

#### On macOS/Linux:
```bash
python3 -m venv .venv
source .venv/bin/activate
```

#### On Windows:
```bash
python -m venv .venv
.venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

If `requirements.txt` is not available, install the core dependencies:

```bash
pip install streamlit langchain langchain-community beautifulsoup4 requests lxml python-dotenv groq
```

### 4. Set Up Environment Variables (Implement yourself)

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key_here
OPENAI_API_KEY=your_openai_api_key_here
HUGGINGFACE_API_KEY=your_huggingface_api_key_here
```

#### Getting API Keys:

- **Groq**: Visit [Groq Console](https://console.groq.com/) and create an API key
- **OpenAI**: Get your key from [OpenAI Platform](https://platform.openai.com/api-keys)
- **Hugging Face**: Create a token at [Hugging Face Tokens](https://huggingface.co/settings/tokens)

### 5. Export Environment Variables

```bash
export GROQ_API_KEY="your_groq_api_key_here"
export OPENAI_API_KEY="your_openai_api_key_here"
```

## 🚀 Usage

### 1. Activate Virtual Environment

```bash
source .venv/bin/activate  # On macOS/Linux
# or
.venv\Scripts\activate     # On Windows
```

### 2. Run the Application

```bash
streamlit run app.py
```

### 3. Access the Interface

Open your browser and navigate to:
```
http://localhost:8501
```

## 📁 Project Structure

```
RAG-TaskSummarizer/
├── app.py                 # Main Streamlit application
├── .env                   # Environment variables (create this)
├── .venv/                 # Virtual environment (auto-generated)
├── requirements.txt       # Python dependencies
├── README.md             # This file
└── groq/                 # Groq-specific implementations
    └── app.py
```

## 🔧 Configuration

### Model Configuration

The application supports multiple LLM providers:

- **Groq**: Fast inference with Llama models
- **OpenAI**: GPT-3.5/GPT-4 models
- **Hugging Face**: Open-source models

### Document Sources

Supported document sources:
- Web URLs
- PDF files
- Text files
- CSV files
- Word documents

## 📝 Features Overview

### 1. Document Loading
- Upload documents or provide URLs
- Automatic content extraction and preprocessing
- Support for multiple file formats

### 2. RAG Pipeline
- Document chunking and embedding
- Vector store creation for efficient retrieval
- Context-aware response generation

### 3. Task Summarization
- Intelligent task extraction from documents
- Contextual summarization
- Action item identification

## 🐛 Troubleshooting

### Common Issues

1. **BeautifulSoup Import Error**:
   ```bash
   pip install beautifulsoup4 lxml html5lib
   ```

2. **API Key Issues**:
   - Ensure API keys are "exported" before use

3. **Virtual Environment Issues**:
   ```bash
   deactivate
   rm -rf .venv
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```

4. **Streamlit Port Issues**:
   ```bash
   streamlit run app.py --server.port 8502
   ```

## 🧪 Testing

Run the application in development mode:

```bash
streamlit run app.py --server.runOnSave true
```

## 📦 Dependencies

Core dependencies:
- `streamlit`: Web interface framework
- `langchain`: LLM application framework
- `langchain-community`: Community extensions
- `beautifulsoup4`: HTML parsing
- `requests`: HTTP requests
- `python-dotenv`: Environment variable management
- `groq`: Groq API client

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit changes: `git commit -m 'Add feature'`
4. Push to branch: `git push origin feature-name`
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

**Shaista Khan**
- GitHub: [@shaistakhan28](https://github.com/shaistakhan28)

## 🙏 Acknowledgments

- LangChain for the RAG framework
- Streamlit for the web interface
- Groq for fast LLM inference
- OpenAI for GPT models

## 📞 Support

If you encounter any issues:
1. Check the troubleshooting section
2. Review the GitHub issues
3. Create a new issue with detailed error information

---

**Happy Summarizing! 🎉**
