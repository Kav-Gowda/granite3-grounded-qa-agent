# granite3-grounded-qa-agent

A **Grounded Question-Answering (Q/A) Agent** built with **IBM Granite 3**, **LangChain**, and **Retrieval-Augmented Generation (RAG)**.  
This project demonstrates how to design a retrieval-based pipeline where the model’s responses are **grounded in actual data**, ensuring factual accuracy and transparency in generated answers.

---

## 🚀 Project Overview
This project showcases a **Granite 3–powered Grounded Q/A Agent** that retrieves relevant context from private documents before generating an answer.  
By combining **LangChain’s retrieval tools** with **IBM watsonx.ai’s Granite 3 LLM**, the system minimizes hallucinations and ensures that every response is supported by retrieved evidence.

**Key Idea:**  
The agent doesn’t “guess” - it *retrieves, reasons, and responds* based on verifiable information.

---

## 🧩 Tech Stack
- **LLM Platform:** IBM watsonx.ai  
- **Model:** Granite 3 (8B Instruct)  
- **Framework:** LangChain  
- **Embeddings:** Watsonx Embeddings (SLATE model)  
- **Vector Store:** ChromaDB  
- **Language:** Python  
- **Environment:** Google Colab  

---

## 📂 Project Structure
granite3-grounded-qa-agent/
├── .gitignore
├── LICENSE
├── README.md
└── src/
└── granite3_langchain_rag_agent.py


---

## ⚙️ How It Works
1. Load private documents locally (kept secure).  
2. Split documents into manageable chunks using `CharacterTextSplitter`.  
3. Create embeddings with **Watsonx Embeddings (SLATE)**.  
4. Store and retrieve data through **ChromaDB**.  
5. Query the **Granite 3 LLM** with retrieved context to generate grounded answers.  
6. Output accurate, reference-supported responses.  

---

## 🧠 Key Features
- **Fact-grounded responses:** Every answer is derived from retrieved content.  
- **Customizable document source:** Easily replace or expand with your own files.  
- **Granite 3 integration:** Leverages IBM’s latest LLMs via watsonx.ai.  
- **LangChain orchestration:** Clean modular design with retriever and chain components.  

---

## 🔒 Data Privacy
This project is built for **secure local document processing**.  
No confidential data or credentials are included in this repository. Replace placeholders in the code with your own credentials if running locally.

---

## 🪪 License
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 👩‍💻 Author
**Kavitha Lingarajegowda**  
AI Product Management enthusiast focused on building reliable, grounded AI systems that transform information into insight.
