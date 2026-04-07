# AI Ethics RAG Chatbot 🤖

## 📌 Project Overview
This project is an AI-powered **Retrieval-Augmented Generation (RAG)** chatbot built using **Flowise**. It is designed to answer questions based on documents related to **Artificial Intelligence Ethics**, specifically focusing on the research paper by Ştefan Trăuşan-Matu.

The chatbot retrieves relevant information from the provided document and generates accurate, context-based responses using the Mistral LLM.

---

## 🎯 Objective
- To apply AI in real-world problem solving.
- To improve document-based question answering using RAG.
- To ensure ethical and responsible AI responses based on source material.

---

## ⚙️ Tech Stack
- **Framework:** Flowise AI
- **LLM:** Mistral AI (`ChatMistralAI`)
- **Embeddings:** Google Gemini / HuggingFace Inference
- **Vector Store:** In-Memory Vector Store
- **Chain:** Conversational Retrieval QA Chain

---

## 🔄 Workflow Explanation

1. **File Loader**
   - Loads the "Ethics in Artificial Intelligence" PDF.
2. **Text Splitter**
   - Splits the document into smaller chunks for efficient processing.
3. **Embeddings**
   - Converts text chunks into vector format using Google Gemini.
4. **Vector Store**
   - Stores these embeddings temporarily for similarity searching.
5. **Retriever**
   - Fetches the most relevant snippets from the document based on the user's question.
6. **Chat Model (Mistral)**
   - Processes the retrieved context to generate a natural language response.
7. **Conversational Chain**
   - Uses **Buffer Memory** to maintain chat history for multi-turn conversations.

---

---

## 📸 Screenshots

### 🔹 Flowise Workflow
![Workflow Configuration](flowise.png)

### 🔹 Chatbot Interaction & Results
![Chat Output 1](output1.png)
![Chat Output 2](output2.png)
![Chat Output 3](output3.png)

---

---

## 📂 Project Files
- `RAG Chatbot Chatflow.json`: The Flowise export file.
- `Ethics in Artificial Intelligence.pdf`: The source knowledge base.
- `/screenshots`: Visual guides of the setup and output.

---

## 🚀 How to Run

1. **Open Flowise:** Ensure your Flowise instance is running.
2. **Import Chatflow:** - Click **Add New** > **Load Chatflow**.
   - Select the `.json` file from this repository.
3. **Add API Keys:**
   - Input your **Mistral API Key**.
   - Input your **Google Gemini API Key**.
4. **Run:** Save the flow and start chatting!

---

## 📈 Future Improvements
- **Persistent Database:** Move from In-Memory to **Pinecone** or **FAISS**.
- **Web Deployment:** Integrate into a React or HTML website.
- **Multi-Doc Support:** Allow the chatbot to query multiple ethics papers.

---

## 👩‍💻 Author
**Simarjeet Kaur**

---

## 📜 License
This project is for educational purposes.
