AI Document Assistant using RAG
📌 Overview

This project implements a Retrieval-Augmented Generation (RAG) based conversational chatbot that enables users to interact with documents in a natural, question-answering format.

The system processes documents, converts them into embeddings, stores them in a vector database, and retrieves relevant context to generate accurate and context-aware responses.

🚀 Features
📄 Document-based Question Answering
🔍 Semantic Search using Embeddings
🧠 Context-Aware Conversations with Memory
⚡ Real-time Response Generation
🔗 End-to-End RAG Pipeline
🏗️ Architecture

The chatbot follows a modular RAG pipeline:

Document Loading
Loads input documents (PDF/Text)
Text Splitting
Splits content into manageable chunks
Uses recursive character splitting for better context retention

Embedding Generation
Converts text into vector embeddings using Google Gemini

Vector Storage
Stores embeddings in an in-memory vector database
Enables similarity-based retrieval

Conversational Retrieval
Retrieves relevant chunks based on user query
Uses chat model (Mistral AI) to generate responses
Memory Integration
Maintains chat history for contextual conversations

Tech Stack
LLM: Mistral AI
Embeddings: Google Gemini Embeddings
Vector Store: In-Memory Vector Store
Framework: Flowise / LangChain-based pipeline
Architecture Type: Retrieval-Augmented Generation (RAG)

 Project Workflow
User Query
   ↓
Retriever (Vector Store)
   ↓
Relevant Document Chunks
   ↓
LLM (Mistral AI)
   ↓
Final Response
Use Case
<img width="1830" height="898" alt="Screenshot 2026-04-07 121804(1)" src="https://github.com/user-attachments/assets/61911b40-53ed-4656-aa4c-7533a3fd954b" />


This chatbot is designed to work on AI Ethics documents, enabling:

Understanding complex research papers
Answering conceptual questions
Extracting insights on:
Transparency
Fairness
Privacy

The system helps bridge the gap between technical AI research and user-friendly interaction.

⚙️ Setup Instructions
1. Clone the Repository
git clone https://github.com/your-username/ai-document-assistant-rag.git
cd ai-document-assistant-rag

3. Install Dependencies
npm install

5. Add API Keys

Create a .env file and add:

MISTRAL_API_KEY=your_key_here
GOOGLE_API_KEY=your_key_here

4. Run the Project
npm run start
🧠 How It Works
Documents are split into chunks
Each chunk is converted into embeddings
When a user asks a question:
The system retrieves the most relevant chunks
Passes them to the LLM
Generates an accurate response based on context

📈 Future Improvements
Persistent vector database (Pinecone / FAISS)
Multi-document support
UI integration (Streamlit / React)
Advanced prompt engineering for better accuracy
Ethical bias detection integration

🎯 Key Learnings
Practical implementation of RAG architecture
Working with LLMs + embeddings + vector search
Understanding AI ethics integration in AI systems
Building context-aware conversational systems

👩‍💻 Author

Jashan
