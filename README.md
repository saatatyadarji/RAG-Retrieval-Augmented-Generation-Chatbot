# RAG-Retrieval-Augmented-Generation-Chatbot
This project is an AI-powered PDF Question Answering system that allows you to upload multiple PDF files and then chat with your data by asking questions about their content — powered by Microsoft’s Phi-2 model.

🚀 Project Overview

This project helps you interact with long PDF documents through natural questions instead of manually reading everything.

It uses Natural Language Processing (NLP) and Large Language Models (LLMs) to:

Read and extract text from multiple PDFs.

Convert the text into numerical vector embeddings.

Retrieve the most relevant information using vector similarity search.

Generate clear and contextual answers using Microsoft Phi-2, a compact yet powerful open-source model.

⚙️ How the Project Works

Upload PDFs — The program extracts text from all PDFs you add.

Split Text into Chunks — Long text is divided into smaller parts for efficient retrieval.

Create Embeddings — Each text chunk is converted into a vector using the all-MiniLM-L6-v2 model.

Store in FAISS — All embeddings are saved in a FAISS vector database for quick look-ups.

Ask Questions — When you type a question:

The system finds the most relevant chunks using cosine similarity.

These chunks are passed to Phi-2 to generate an accurate and human-like answer.

🧩 Technologies & Libraries Used
🔹 Core Python Libraries

os – File handling

PyPDF2 – Extracting text from PDFs

langchain – Managing the retrieval + generation pipeline

sentence-transformers – For text embeddings (all-MiniLM-L6-v2)

faiss – For fast similarity search between text chunks

transformers – To load and use Microsoft Phi-2

huggingface_hub – For accessing models from Hugging Face

🔹 Models Used

Embedding Model: all-MiniLM-L6-v2
→ Converts text into vector representations for comparison.

Language Model: microsoft/phi-2
→ Generates coherent and context-aware answers based on retrieved information.

💡 Features

✅ Upload and process multiple PDFs
✅ Ask natural questions and get instant answers
✅ Works offline after setup
✅ Uses FAISS for efficient retrieval
✅ Modular and easy-to-understand code

❤️ Acknowledgements

Microsoft Phi-2

Sentence Transformers

LangChain

FAISS

Hugging Face Transformers
