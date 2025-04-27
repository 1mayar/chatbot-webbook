# 🛒 E-commerce Chatbot with RAG (Retrieval-Augmented Generation)

This project builds a smart chatbot that can answer questions about products from an e-commerce website.  
It uses web scraping, semantic search (FAISS), and a lightweight language model (FLAN-T5) to create a Retrieval-Augmented Generation (RAG) pipeline.

---

## 📚 Project Overview

- **Scrape**: Extract product information (names, prices, categories) from an online store.
- **Preprocess**: Clean and split the data into semantic chunks.
- **Embed**: Create semantic embeddings using `sentence-transformers` (all-MiniLM-L6-v2).
- **Store**: Save embeddings in a FAISS vector database for fast similarity search.
- **Retrieve + Generate**: When the user asks a question, retrieve relevant chunks and generate an intelligent answer using a HuggingFace LLM (Flan-T5-small).
- **Chatbot**: A simple interactive chatbot that communicates with the user via text.

---

## 🛠️ Tech Stack

- Python
- BeautifulSoup (Web Scraping)
- Sentence-Transformers (Embeddings)
- FAISS (Vector Database)
- HuggingFace Transformers (LLM + Pipeline)
- LangChain (RAG Pipeline)
- NLTK (Text Splitting)

---

## 🚀 How it Works

1. **Scrape Website Content**  
2. **Clean and Chunk Text**  
3. **Generate Vector Embeddings**  
4. **Store Vectors in FAISS**  
5. **Ask Questions via Chatbot**  
6. **Retrieve Relevant Chunks + Generate Final Answer**

---

## 🧠 Example Questions

You can ask the chatbot:

- "What is the price of the Signature Cheesecake?"
- "Show me the featured products."
- "Where is the store located?"
- "What is the best dessert available?"
- "Do you have any offers?"
- "What products are available in the chocolate category?"
- "Is there a delivery option?"

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/ecommerce-rag-chatbot.git
cd ecommerce-rag-chatbot
pip install -r requirements.txt
python chatbot.py
