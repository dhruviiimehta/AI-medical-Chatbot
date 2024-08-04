# AI-medical-Chatbot
Overview
Zana's current chatbot is designed to answer general questions, onboard customers, drive engagement, and provide support. However, it has several limitations such as basic interaction capabilities, lack of multilingual support, and absence of advanced AI functionalities. The Prosperia AI Chatbot aims to overcome these limitations by leveraging the LLaMA2 model and Langchain integration to provide a more engaging and personalized user experience.

Key Features
Multilingual Support: Supports multiple languages to cater to a diverse user base.
Advanced AI Capabilities: Utilizes LLaMA2 for natural language understanding and generation.
Personalized Interactions: Provides responses tailored to the user's health conditions and medical history.
Real-Time Medical Assistance: Connects users with healthcare professionals for urgent consultations.
Timely Notifications: Sends reminders for medication and scheduled appointments.
Scalable and Efficient: Capable of handling a large volume of queries with low latency.
System Architecture
Data Ingestion and Preprocessing

PDF File Medical Books: Uses medical textbooks in PDF format.
Extract Data: Text extraction using Python libraries like PyMuPDF, PyPDF2, or pdfminer.six.
Text Chunks: Segmentation of extracted text into manageable chunks.
Embedding Generation

Embeddings: Conversion of text chunks into high-dimensional vectors using Sentence Transformers.
Indexing and Storage

Building Semantic Index: Compilation of embeddings into a structured index.
Knowledge Base: Storage of the semantic index and embeddings.
Vector Database

Pinecone Vector DB: Storage and real-time similarity search of embeddings.
Query Processing and RAG

User Query: Conversion of user queries into embeddings.
Document Retrieval: Similarity search in Pinecone Vector DB.
Combining Retrieval and Generation: Integration with Langchain to combine retrieved text chunks with user queries.
LLaMA2: Generation of coherent and contextually appropriate responses.
