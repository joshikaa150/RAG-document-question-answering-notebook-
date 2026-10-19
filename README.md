# 📚 RAG Document Question-Answering Assistant

<p align="center">
  <b>Ask questions about PDF documents and get context-based answers using Generative AI.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/FAISS-Vector_Search-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Ollama-Local_LLM-black?style=for-the-badge" />
</p>

## 🎯 Project Overview

The **RAG Document Question-Answering Assistant** is a Generative AI project that helps users retrieve relevant information from PDF documents and generate answers based on the retrieved content.

It combines document retrieval with a Large Language Model (LLM), helping the model answer questions using relevant document context rather than relying only on its general knowledge.

## 🚀 Features

- 📄 Load and process PDF documents.
- ✂️ Split document text into smaller chunks.
- 🧠 Generate embeddings using Hugging Face models.
- 🔎 Retrieve relevant chunks using FAISS vector search.
- 🤖 Generate answers using an Ollama language model.
- 💬 Answer user questions using retrieved document context.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| LangChain | Building the RAG pipeline |
| Hugging Face Embeddings | Converting text into numerical vectors |
| FAISS | Storing and searching vector embeddings |
| Ollama | Running the language model locally |
| Llama 3.2 | Generating answers |
| Jupyter Notebook | Development and experimentation |

## ⚙️ How It Works

1. **Document Loading:** Extract text from a PDF document.
2. **Text Chunking:** Divide the extracted text into smaller sections.
3. **Embedding Generation:** Convert text chunks into vector representations.
4. **Vector Search:** Use FAISS to find chunks relevant to the user's question.
5. **Context Retrieval:** Pass the retrieved text to the language model.
6. **Answer Generation:** Use Ollama to generate an answer based on the available context.

```text
PDF Document
     ↓
Text Extraction
     ↓
Text Chunking
     ↓
Hugging Face Embeddings
     ↓
FAISS Vector Search
     ↓
Relevant Context
     ↓
Ollama LLM
     ↓
Generated Answer
```

## 📂 Project Structure

```text
rag-document-qa-assistant/
│
├── rag_document_qa_assistant.ipynb
├── README.md
└── requirements.txt
```

## 💻 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/joshikaa150/pandas-data-analysis.git
cd pandas-data-analysis
```

### 2. Install Python dependencies

```bash
pip install -r requirements.txt
```

### 3. Install and start Ollama

Install Ollama from [ollama.com](https://ollama.com/) and download the model:

```bash
ollama pull llama3.2
```

Ensure Ollama is running before executing the notebook.

### 4. Open the notebook

```bash
jupyter notebook
```

Open `rag_document_qa_assistant.ipynb` and run the cells in order.

**Note:** Update the PDF file path to a valid local path on your computer. The original notebook's local Windows file path will not work on other machines.

## 📦 Requirements

Your `requirements.txt` should include the libraries actually imported by the notebook. Depending on the implementation, these may include:

```text
langchain
langchain-community
langchain-text-splitters
langchain-huggingface
sentence-transformers
faiss-cpu
pypdf
ollama
jupyter
```

Install any additional packages required by your notebook. Package names and versions should be verified against your working environment.

## 🎓 Learning Outcomes

- Understanding Retrieval-Augmented Generation (RAG).
- Working with PDF document processing.
- Generating text embeddings.
- Performing semantic similarity search.
- Integrating a locally hosted Large Language Model.
- Building a document-based question-answering workflow.

## 🔮 Future Improvements

- Build a user-friendly interface using Streamlit.
- Support multiple PDF documents.
- Add source citations for generated answers.
- Handle questions when the document does not contain the answer.
- Add automated evaluation tests for retrieval and answer quality.

## 👩‍💻 Author

**Joshika G.**

Computer Science Graduate | Generative AI | Machine Learning

[GitHub Profile](https://github.com/joshikaa150)

---

⭐ If you find this project useful, feel free to explore the repository and share feedback.
