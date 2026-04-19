
# GenAiProject

Practicing GenAI and LangChain with a simple notebook-based workflow for talking to an LLM and experimenting with retrieval-augmented generation (RAG) on PDF content.

## Overview

This project is a hands-on GenAI learning repo built around LangChain. It includes:

- a notebook for chatting with a large language model
- a PDF document used as a knowledge source for RAG experiments
- the basic package requirements needed to run the project

The current notebook demonstrates:
- loading environment variables from a `.env` file
- connecting to Groq through `ChatGroq`
- using the `llama3-70b-8192` model
- loading and splitting a PDF with `PyPDFLoader`

## Features

- LLM chat demo with LangChain
- Environment variable support with `python-dotenv`
- PDF loading for document-based Q&A
- RAG experimentation with LangChain components
- Easy setup for further GenAI practice

## Tech Stack

- Python
- Jupyter Notebook
- LangChain
- LangChain Groq
- LangChain OpenAI
- LangChain Community
- Chroma
- PyPDF
- Unstructured
- BeautifulSoup
- python-dotenv

## Project Files

- `01_talk_to_llm.ipynb` — main notebook
- `Bus PDF.pdf` — source document for RAG
- `requirements.txt` — required Python packages
- `.gitignore` — ignored files and folders

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/AsifIqbal011/GenAiProject.git
cd GenAiProject
````

### 2. Create a virtual environment

Using Conda:

```bash
conda create -n llmapp python=3.11 -y
conda activate llmapp
```

Or using `venv`:

```bash
python -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

## Environment Setup

Create a `.env` file in the project root and add your API key:

```env
GROQ_API_KEY=your_groq_api_key_here
```

If you extend the project with OpenAI-based components, also add:

```env
OPENAI_API_KEY=your_openai_api_key_here
```

## Usage

1. Open `01_talk_to_llm.ipynb` in Jupyter Notebook or VS Code.
2. Run the cells step by step.
3. Update the notebook prompt or PDF source as needed.
4. Experiment with:

   * different system prompts
   * different LLM models
   * custom PDF documents
   * vector stores and retrieval settings

## RAG Workflow

The notebook shows the start of a RAG pipeline:

1. Load the PDF document
2. Split the document into chunks
3. Use LangChain tools to connect retrieval with generation
4. Ask questions based on the loaded content

## Example Use Case

This repository can be used to build a chatbot that answers questions from a custom PDF, such as:

* class notes
* project reports
* company documents
* research papers

## Requirements

Main packages used in this project:

* `langchain`
* `langchain-openai`
* `langchain-groq`
* `langchain-community`
* `python-dotenv`
* `bs4`
* `unstructured`
* `pypdf`
* `langchain-chroma`

## Future Improvements

* Add a full RAG pipeline with embeddings and vector search
* Build a chat UI with Streamlit or Flask
* Add source citations in answers
* Support multiple documents
* Add prompt templates and memory support

## Author

Asif Iqbal
