# **Climate Finance Retrieval-Augmented Generation (RAG) System**

## **Overview**
This project implements a **Retrieval-Augmented Generation (RAG) system** for answering climate finance-related research questions. It combines **document retrieval**, **embeddings**, and a **large language model (LLM)** to generate well-informed responses.

---

## **Project Architecture**
1. **Document Processing**  
   - Documents are split into smaller **chunks**.  
   - **Sentence-transformers/all-MiniLM-L6-v2** is used to generate **embeddings**.  
   - Chunks and their embeddings are stored in a **ChromaDB** vector database.  

2. **Retrieval & Query Processing**  
   - User queries are matched with the most relevant document chunks.  
   - The relevant chunk is passed to the **Mistral-7B-Instruct-v0.3** model for response generation.  

3. **Evaluation**  
   - **ROUGE and BLEU** scores measure response quality.  
   - Evaluation criteria include **relevance, accuracy, and clarity**.  

4. **User Interface**  
   - A **Gradio** web interface allows users to submit research questions and receive responses.  

---

## **Technologies Used**
- **Python** (Main development language)  
- **Hugging Face Transformers** (Embeddings & LLM)  
- **ChromaDB** (Vector database for document retrieval)  
- **Gradio** (User-friendly interface)  
- **NLTK & ROUGE** (Text evaluation metrics)  

---


