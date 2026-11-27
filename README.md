# DOMCHAT 🤖
### Domain Conversational Hub for Analytical Tasks

**AI-Powered Domain Analysis, Document Intelligence & Conversational Reporting**

DOMCHAT is an intelligent AI-powered web application designed to simplify domain analysis, document understanding, and information retrieval through conversational interactions. Built using Python and Flask, it combines domain intelligence, document processing, Retrieval-Augmented Generation (RAG), and Large Language Models (LLMs) to deliver contextual insights and analytical responses through an interactive web interface.

The application supports multiple analysis sessions and provides flexibility through cloud-based and locally hosted language models.

## 🚀 Key Features

- **AI-Powered Domain Analysis:** Analyze domain-related information and generate contextual insights.
- **URL Analysis:** Process and analyze information obtained from web URLs.
- **Document Intelligence:** Upload and process documents for conversational analysis.
- **Conversational AI:** Interact with the system using natural language queries.
- **Retrieval-Augmented Generation (RAG):** Retrieve relevant information from stored knowledge to improve response relevance.
- **Vector Database Integration:** Use ChromaDB for storing and retrieving document embeddings.
- **Multiple LLM Providers:** Support for Groq API and locally hosted language models.
- **Session Management:** Create and manage multiple independent analysis sessions.
- **Interactive Web Interface:** User-friendly interface for domain and document interactions.
- **RESTful API:** Structured backend endpoints for application functionality.
- **Logging and Diagnostics:** Application logging and system status monitoring.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Backend | Python |
| Frontend | HTML, CSS, JavaScript |
| Framework | Flask |
| Vector Database | ChromaDB |
| Embeddings | Sentence Transformers |
| AI Integration | Groq API, Local LLM |
| RAG Framework | Retrieval-Augmented Generation |
| Document Processing | PDF, DOCX and HTML processing |
| Web Automation | Playwright (where configured) |
| Environment Management | Python Virtual Environment |

## 🏗️ System Architecture

DOMCHAT follows a modular architecture that integrates domain analysis, document processing, vector retrieval, and language model inference.

### Core Components

**1. Domain Analysis Engine**

Processes domain-related information and generates meaningful insights using the application's analysis components.

**2. Document Processing Engine**

Extracts and processes content from supported documents, preparing information for semantic retrieval and conversational interactions.

**3. Embedding Generation**

Uses Sentence Transformers to convert textual information into numerical vector representations.

**4. Vector Storage and Retrieval**

Uses ChromaDB to store document embeddings and retrieve relevant information based on semantic similarity.

**5. Language Model Integration**

Uses Groq API or a locally configured language model to generate contextual responses based on retrieved information.

**6. Flask Backend**

Handles API requests, session management, document uploads, analysis operations, and communication between frontend and backend components.

## 🔄 RAG Workflow

DOMCHAT uses a Retrieval-Augmented Generation workflow to provide context-aware responses.

1. **Document Ingestion:** Users upload documents or provide information for analysis.
2. **Text Extraction:** The application extracts textual content from supported sources.
3. **Text Processing:** Extracted content is prepared for semantic processing.
4. **Embedding Generation:** Sentence Transformers generate vector embeddings.
5. **Vector Storage:** ChromaDB stores embeddings along with their associated metadata.
6. **Semantic Retrieval:** User queries are converted into embeddings, and relevant information is retrieved.
7. **Response Generation:** Retrieved context is supplied to the configured language model to generate relevant responses.

## 📋 Prerequisites

- Python 3.10 or later (compatible with your installed dependencies).
- Git.
- pip package manager.
- Internet connection for installing dependencies and using cloud-based services.
- Groq API key when using the Groq provider.
- Sufficient system resources for locally hosted language models.

## 🔧 Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/DOMCHAT.git
cd DOMCHAT
```

### 2. Create a Virtual Environment

**Windows:**

```powershell
python -m venv dcenv
```

Activate it:

```powershell
.\dcenv\Scripts\Activate.ps1
```

**Linux:**

```bash
python3 -m venv dcenv
source dcenv/bin/activate
```

### 3. Install Dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Install Playwright Browsers

If Playwright is required by your configured application:

```bash
playwright install
```

## 🔑 Environment Configuration

Create a `.env` file in the project root directory.

Add the required configuration:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Configure additional settings according to the options available in `config.py`.

**Important:** Never upload your actual API keys or sensitive credentials to GitHub.

## 🚀 Running the Application

### 1. Activate the Virtual Environment

**Windows:**

```powershell
.\dcenv\Scripts\Activate.ps1
```

**Linux:**

```bash
source dcenv/bin/activate
```

### 2. Start the Application

```bash
python api.py
```

### 3. Access the Application

Open your browser and navigate to:

```text
http://localhost:5000
```

You can now interact with the DOMCHAT application through its web interface.

## 📁 Project Structure

```text
DOMCHAT/
│
├── api.py                  # Main Flask application and REST API
├── config.py               # Application configuration
├── requirements.txt        # Python dependencies
├── .env                    # Environment variables (not committed)
├── .gitignore              # Git ignored files
│
├── core/
│   ├── analyzer.py         # Domain analysis logic
│   ├── llm_singleton.py    # Language model management
│   └── ...                 # Other core modules
│
├── static/                 # CSS, JavaScript and frontend assets
│
├── templates/              # HTML templates
│
└── README.md               # Project documentation
```

*Note: The structure above highlights the main components. Refer to the repository for the complete directory structure.*

## 🔌 API Integration

DOMCHAT uses REST API endpoints to connect its frontend with backend functionality.

The backend supports operations such as:

- Application initialization.
- Analysis session creation and management.
- Domain analysis.
- Document uploading and processing.
- Conversational document queries.
- Document session status monitoring.
- Document management.
- Language model configuration and status.

## 🔮 Future Enhancements

- Advanced domain intelligence and threat analysis.
- Improved document retrieval and ranking mechanisms.
- Multilingual conversational support.
- Enhanced response accuracy and hallucination reduction.
- Advanced analytical dashboards and reporting.
- Improved scalability and performance optimization.

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push your branch.
5. Submit a Pull Request.

## 👨‍💻 Author

**Mohamed Ibrahim Badhusha M K**

GitHub: [MohamedIbrahimBadhushaMK](https://github.com/MohamedIbrahimBadhushaMK)

## 🙏 Acknowledgments

- Flask for backend application development.
- ChromaDB for vector database functionality.
- Sentence Transformers for semantic embeddings.
- Groq for cloud-based LLM inference.
- Open-source contributors and developers.

---

⭐ If you find this project interesting, consider giving it a star!
