# 🎓 College Information Chatbot using RAG Architecture

> An end-to-end Retrieval-Augmented Generation (RAG) based AI chatbot developed as a Final Year B.Tech Project. The system provides intelligent, context-aware responses to college-related queries by combining semantic search, vector databases, and Large Language Models.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue.svg">
  <img src="https://img.shields.io/badge/LangChain-RAG-green.svg">
  <img src="https://img.shields.io/badge/LLM-GROQ-orange.svg">
  <img src="https://img.shields.io/badge/VectorDB-ChromaDB-purple.svg">
  <img src="https://img.shields.io/badge/UI-Streamlit-red.svg">
  <img src="https://img.shields.io/badge/Status-Completed-success.svg">
</p>

---

# 📌 Project Overview

The **College Information Chatbot** is an AI-powered assistant built using the **Retrieval-Augmented Generation (RAG)** framework. It enables users to ask natural language questions related to college information and receive accurate, context-aware responses in real time.

Unlike traditional chatbots that rely solely on pre-trained knowledge, this chatbot first retrieves the most relevant information from a custom knowledge base and then generates responses using a Large Language Model (LLM). This significantly improves response accuracy while reducing hallucinations.

The project was developed as a **Final Year B.Tech Project**, following an industry-inspired modular architecture for scalability, maintainability, and future enhancements.

---

# 🚀 Key Features

- End-to-End RAG Pipeline
- Intelligent College Information Assistant
- Context-Aware Question Answering
- Modular Project Architecture
- Semantic Search using Vector Embeddings
- Fast Document Retrieval with ChromaDB
- GROQ LLM API Integration
- Interactive Streamlit + CSS User Interface
- Scalable and Beginner-Friendly Implementation
- Easy Knowledge Base Updates

---

# 🏗 Project Architecture

```
                    User Query
                         │
                         ▼
                Streamlit Interface
                         │
                         ▼
                  RAG Generation Pipeline
                         │
     ┌───────────────────┴───────────────────┐
     │                                       │
Retrieval Pipeline                     Generation Pipeline
     │                                       │
Embedding Model                     GROQ LLM API
     │                                       │
Vector Database (ChromaDB)                  │
     │                                       │
Relevant Context Retrieval                   │
     └───────────────────┬───────────────────┘
                         ▼
               Context + Prompt Construction
                         ▼
                 Intelligent AI Response
```

---

# ⚙️ Technologies Used

## Programming Language

- Python

## Frameworks

- LangChain
- Streamlit

## Embedding Model

- all-MiniLM-L6-v2

## Vector Database

- ChromaDB

## Large Language Model

- GROQ API

## Frontend

- Streamlit
- Custom CSS

## Other Libraries

- Sentence Transformers
- Transformers
- PyTorch

---

# 🧠 Working Methodology

The chatbot follows a complete Retrieval-Augmented Generation workflow.

## Step 1 — Data Collection

- Collected college-related information.
- Stored knowledge in structured text files.

---

## Step 2 — Document Processing

- Loaded documents.
- Performed preprocessing.
- Removed unnecessary formatting.

---

## Step 3 — Text Chunking

Large documents were divided into smaller overlapping chunks using LangChain's CharacterTextSplitter.

Benefits:

- Better retrieval
- Better context preservation
- Improved embedding quality

---

## Step 4 — Embedding Generation

Each chunk was converted into semantic vectors using

```
all-MiniLM-L6-v2
```

These embeddings capture the semantic meaning instead of exact keywords.

---

## Step 5 — Vector Database Creation

Generated embeddings were stored inside

```
ChromaDB
```

This enables fast similarity search over thousands of document chunks.

---

## Step 6 — Retriever Pipeline

When a user asks a question,

the retriever

- converts the query into embeddings
- searches the vector database
- retrieves the most relevant chunks

---

## Step 7 — Prompt Engineering

Retrieved context is combined with the user query using a custom prompt template.

Example:

```
Context:
...

Question:
...

Answer:
```

This minimizes hallucination and ensures grounded responses.

---

## Step 8 — Generation Pipeline

The constructed prompt is sent to the

```
GROQ LLM API
```

which generates an accurate, human-like response.

---

## Step 9 — Streamlit Interface

The chatbot is deployed using

- Streamlit
- Custom CSS

Features include

- Interactive Chat Interface
- Clean Dark Theme
- Chat History
- Responsive Layout
- Sidebar Navigation
- Smooth User Experience

---

# 📂 Project Structure

```
College-Information-Chatbot/
│
├── backend/
│   ├── ingestion.py
│   ├── retrieval.py
│   ├── rag_pipeline.py
│   ├── embedding.py
│   └── vectorstore.py
│
├── data/
│   └── college_information.txt
│
├── app.py
├── requirements.txt
├── README.md
└── assets/
```

---

# 🎯 Applications

This chatbot can be used for

- College Information System
- Student Assistance
- Faculty Information
- Admission Guidance
- Campus Navigation
- Department Details
- Placement Information
- Personalized Knowledge Assistants
- Enterprise Knowledge Management

---

# 💡 Why RAG?

Traditional LLMs rely only on pre-trained knowledge, which can lead to hallucinations and outdated information.

Retrieval-Augmented Generation improves reliability by retrieving relevant context before generating a response.

Benefits include

- Higher Accuracy
- Reduced Hallucination
- Domain-Specific Knowledge
- Real-Time Knowledge Updates
- Better User Trust

---

# 🌟 Highlights

✔ End-to-End RAG Architecture

✔ Complete Retrieval Pipeline

✔ Complete Ingestion Pipeline

✔ Generation Pipeline using GROQ LLM

✔ Modular Project Structure

✔ Semantic Search

✔ Vector Database Integration

✔ Streamlit User Interface

✔ Industry-Oriented Workflow

✔ Final Year B.Tech Project

---

# 🔮 Future Enhancements

- PDF Support
- Multiple Document Formats
- Conversation Memory
- Voice Assistant
- Image-based Query Support
- Multi-language Support
- User Authentication
- Cloud Deployment
- Admin Dashboard
- Analytics Dashboard

---

# 📚 Learning Outcomes

During this project, I gained hands-on experience with

- Retrieval-Augmented Generation (RAG)
- LangChain Framework
- Prompt Engineering
- Embedding Models
- Vector Databases
- Semantic Search
- Large Language Models
- Streamlit Development
- Modular Python Architecture
- AI Application Development

---

# 👨‍💻 Contributors

- Suryavhi Das (Group Leader)
- Aiswarya Paul (Group Co-Lead)
- Suja Uddin Mollah
- Anand Kumar Jha
- Manprit Acharya

---

# 🎓 Academic Information

**Project Title**

College Information Chatbot using RAG Architecture

**Institution**

Techno Engineering College Banipur

**Degree**

Bachelor of Technology (B.Tech)

---

# ⭐ Support

If you found this project interesting,

⭐ Star this repository

🍴 Fork it

💬 Share your feedback

---

# 📬 Connect With Me

**Suryavhi Das**

Aspiring AI Engineer | Data Analyst | Machine Learning Enthusiast | Generative AI Developer

Let's connect and collaborate on AI, Data Science, and Open Source projects.

---

> "Retrieval makes AI knowledgeable. Generation makes AI conversational. RAG combines the best of both worlds."
