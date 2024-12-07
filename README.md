# End-to-End Retrieval-Augmented Generation (RAG) Project

This repository demonstrates an end-to-end **Retrieval-Augmented Generation (RAG)** system using open-source **LLM models** and the **Groq inferencing engine**. The project integrates LangChain, FAISS, and Streamlit to create a robust document retrieval and query-answering application.

---

## 🌟 Features

- **Open-Source LLM Models**: Implements models such as **LLaMA** and **Mistral** for embeddings and retrieval, ensuring flexibility and cost-effectiveness.
- **Groq Inferencing Engine**: Utilizes Groq's **Language Processing Unit (LPU)** for faster and efficient model inferencing.
- **Streamlit UI**: Provides an interactive web application to query the system and view results.
- **Document Processing**: Efficiently reads and processes web documents, splitting them into manageable chunks.
- **Custom Chat Prompts**: Contextual responses generated using tailored prompt templates.
- **Vector Store**: Embeddings are stored in **FAISS** for fast similarity search and retrieval.

---

## 🚀 Quick Start

### 1. Clone the Repository

```
git clone https://github.com/your-username/rag-project.git
cd rag-project
```
2. Install Dependencies
```
pip install -r requirements.txt
```
4. Set Up Environment Variables

Create a .env file in the root directory and add your Groq API key:
```
GROQ_API_KEY=your-api-key
```
4. Run the Application
```
streamlit run app.py
```

📄 How It Works
Document Loading:

Loads content from a given web source using WebBaseLoader.
Embedding:

Processes documents into embeddings using AMAEmbedding, an open-source method.
Vector Store:

Embeddings are stored in FAISS, enabling fast similarity-based retrieval.
Query and Retrieval:

Queries are matched with documents, and the system generates responses based on the retrieved context.
Streamlit Interface:

A user-friendly web interface for interaction and visualization.


📦 Project Structure

```
rag-project/
│
├── app.py                # Main Streamlit application
├── document_loader.py    # Document loading and preprocessing
├── retrieval_system.py   # Vector store and retrieval logic
├── .env                  # Environment variables (not included in the repo)
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation

```
🛠️ Key Libraries
LangChain: For document loading, processing, and embedding.
FAISS: For vector similarity search.
Streamlit: For building the interactive web app.
Groq: High-speed inferencing engine.


📊 Example Queries
"How to set up an environment for LangChain?"
"Steps to create an API key in Groq?"
"What are the benefits of using Groq's LPU?"



🚀 Future Enhancements
Integrate larger context length models for better retrieval accuracy.
Optimize indexing for larger datasets with incremental loading.
Add a more detailed query analysis and advanced visualization features.


🤝 Contributing
Contributions are welcome! Please fork the repository, submit issues, or create pull requests to enhance the project.

📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

🙌 Acknowledgments
Special thanks to the open-source contributors of LangChain, FAISS, and Streamlit
