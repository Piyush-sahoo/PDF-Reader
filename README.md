# PDF Assistant

A Python-based interactive CLI assistant that can read, understand, and answer questions about PDF documents using LLM (Language Learning Model) capabilities through the Groq API.

## Short Description
PDF Assistant is a CLI tool powered by Groq API that enables interactive conversations with PDF documents. It uses vector database storage for efficient document retrieval and maintains conversation history for contextual responses.

## Features
- PDF document loading and processing
- Vector database storage using PostgreSQL
- Conversation history tracking
- Interactive CLI interface
- Knowledge base searching capabilities
- Tool call visibility in responses

## Prerequisites
- Python 3.8+
- PostgreSQL database
- Groq API key

## Installation
1. Clone the repository
2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
Create a `.env` file with:
```
GROQ_API_KEY=your_api_key_here
```

4. Set up PostgreSQL database with the following configuration:
```
Host: localhost
Port: 5532
Database: ai
User: ai
Password: ai
```

## Usage
Run the assistant:
```bash
python pdf_assistant.py
```

Options:
- `--new`: Start a new conversation session
- `--user`: Specify user ID (default: "user")

Example:
```bash
python pdf_assistant.py --new --user john
```

## Configuration
The assistant is configured to use:
- PDFUrlKnowledgeBase for document processing
- PgVector2 for vector storage
- PgAssistantStorage for conversation storage

## Dependencies
- phidata
- python-dotenv
- groq
- sqlalchemy
- pgvector
- psycopg[binary]
- pypdf
- (other dependencies in requirements.txt)



## GitHub Description
A CLI-based PDF assistant powered by Groq API that enables interactive conversations with PDF documents. Features include vector database storage, conversation history tracking, and knowledge base searching. Built with Python, PostgreSQL, and phidata framework.
