# Medical_Chatbot_Using_RAG
## 🏥Medical Chatbot using RAG (Retrieval-Augmented Generation)

An intelligent medical-query assistant built using Retrieval-Augmented Generation (RAG).
This project enhances the accuracy and safety of AI-generated responses by grounding answers in verified medical documents supplied in the vector database.
This chatbot focusses mainly on heart diseases.

## 🚀Features
* RAG-powered medical question answering
Uses embeddings + retrieval to generate context-aware, reliable answers from your uploaded medical documents.

* OpenAI API integration
Utilizes OpenAI’s models for embeddings and LLM generation.

* Vector database support
Can be used with ChromaDB / FAISS / Pinecone (depending on your implementation).

* Streaming & follow-up conversations
Maintains chat history for multi-turn conversations.

* Clean modular architecture
Easily extendable for new data sources or new medical specialities.

## 🛠️Tech Stack
* Python 3.10+
* OpenAI API (for embeddings + LLM)
### RAG Pipeline
* Document loading → Chunking → Embeddings → Vector Store → Retrieval → LLM
* Vector DB: (Chroma)

## 🔧Installation
```
git clone https://github.com/vvarss/medical-rag-chatbot.git
cd medical-rag-chatbot
```
## 📚RAG Workflow
* Document ingestion
Loads PDFs/text → cleans → chunks.
* Embedding generation
Each chunk is encoded into vector embeddings using OpenAI.
* Vector storage
Stored in Chroma.
* Retrieval
When the user asks a question, the system finds the most relevant document chunks.
*LLM reasoning
The LLM uses the retrieved medical context + conversation history to generate a safe answer.
## 🛡️ Safety
* No diagnosis is given.
* No personalised medical instructions.
* Answers are grounded in your uploaded documents.

## 🤝Contributing
Pull requests are welcome!❤️

Feel free to open issues for feature suggestions or bug reports.
