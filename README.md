# RepoGuide AI

> Your AI Copilot for to improve self-coding or understanding and navigating software repositories.

RepoGuide AI is an AI-powered software engineering assistant that helps developers by analyzing GitHub repositories and answering technical questions using Retrieval-Augmented Generation (RAG).

The goal is to make exploring complex software projects faster by providing an AI assistant that understands and is able to review and suggest on the structure, architecture, and implementation details of a codebase.

---

## 🚀 Motivation

Understanding an existing codebase is one of the biggest challenges developers face, especially when joining a new team, contributing to open-source projects, or maintaining legacy systems.

Traditional documentation is often incomplete, outdated, or spread across multiple sources. While Large Language Models can answer programming questions, they usually lack context about a specific project and cannot provide meaningful insights without understanding the underlying codebase.

Additionally, developers working on personal projects often lack a technical partner who can review their architecture decisions, suggest improvements, identify potential issues, and provide guidance throughout the development process.

RepoGuide AI addresses these challenges by indexing software repositories and allowing developers to interact with their codebase through natural language. It acts as an AI software engineering assistant that helps developers explore unfamiliar projects, understand existing implementations, review their own code, improve project structure, and receive suggestions throughout the development process.

---

## ✨ Features

### Current MVP

- [ ] Analyze GitHub repositories
- [ ] Clone and process repository files
- [ ] Generate embeddings from source code
- [ ] Store code knowledge using vector search
- [ ] Ask questions about the repository
- [ ] Generate answers based on actual project context

### Future Features

- [ ] Automatic architecture analysis
- [ ] Codebase documentation generation
- [ ] Dependency analysis
- [ ] Code quality recommendations
- [ ] Security vulnerability detection
- [ ] Test coverage suggestions
- [ ] Architecture diagrams generation
- [ ] Pull Request reviews
- [ ] Multi-agent software engineering workflows

---

## 🏗️ Architecture Overview

RepoGuide AI follows a Retrieval-Augmented Generation (RAG) architecture.

~~~
                  User
                   |
                   v
              Web Interface
                   |
                   v
              Backend API
                   |
        +----------+----------+
        |                     |
        v                     v
 Repository Processor     AI Assistant
        |                     |
        v                     v
 Code Chunking          Context Retrieval
        |                     |
        v                     v
 Embeddings --------> Vector Database
                              |
                              v
                         LLM Response
~~~

---

## 🛠️ Tech Stack

### Frontend

- Next.js
- React
- TypeScript
- Tailwind CSS
- shadcn/ui

### Backend

- Python
- FastAPI
- SQLAlchemy

### Database

- PostgreSQL
- pgvector

### AI / Machine Learning

- LangChain
- LangGraph
- Gemini API
- Embeddings models

### Infrastructure

- Docker
- Docker Compose
- GitHub Actions

---

## 📂 Project Structure

~~~
repoguide-ai/

├── frontend/          # Web application
├── backend/           # API and AI services
├── docs/              # Project documentation
├── docker/            # Docker configurations
├── .github/           # GitHub workflows
├── docker-compose.yml
└── README.md
~~~

---

## 🧠 How It Works

At a high level, RepoGuide AI follows these steps:

1. User provides a GitHub repository URL.
2. The system clones and analyzes the repository.
3. Source code is divided into meaningful chunks.
4. Text embeddings are generated from the code.
5. Embeddings are stored in a vector database.
6. User questions are converted into semantic searches.
7. Relevant code context is retrieved.
8. The AI generates an answer based on the retrieved information.

---

## 📌 Example Use Cases

### Understanding a new project

> "Explain the authentication flow in this application."

### Exploring architecture

> "How are API requests handled?"

### Finding technical debt

> "Which parts of this codebase could be improved?"

### Learning a framework

> "Explain how state management is implemented."

---

## 🗺️ Roadmap

### Phase 1 — Repository Analysis

- [ ] Project setup
- [ ] GitHub repository ingestion
- [ ] Source code processing
- [ ] Basic repository indexing

### Phase 2 — AI Assistant

- [ ] RAG pipeline implementation
- [ ] Vector database integration
- [ ] Conversational interface

### Phase 3 — Developer Intelligence

- [ ] Architecture analysis
- [ ] Code recommendations
- [ ] Documentation generation

### Phase 4 — Advanced AI Agents

- [ ] Tool calling
- [ ] Repository exploration agents
- [ ] Automated refactoring suggestions
- [ ] Development workflow integration

---

## 🎯 Project Goals

This project aims to explore and implement modern AI engineering concepts, including:

- Retrieval-Augmented Generation (RAG)
- Vector databases
- Embeddings
- AI agents
- Large Language Model applications
- Full-stack AI product development

---

## 👨‍💻 Author

Lucas Silva Teixeira

Software Engineering Student | Full Stack Developer

LinkedIn: https://www.linkedin.com/in/lucasteixeiraa

---

## 📄 License

This project is licensed under the MIT License.
