# 🧠 Antahkarana: Your Second Brain AI Assistant

![Antahkarana Flow Diagram](docs/Antahkarana_flow_diagram.png)

Antahkarana(The Inner Instrument) is one of my dear projects that is a personal AI second brain assistant on top of your digital resources. It leverages advanced GenAI concepts, including Retrieval-Augmented Generation (RAG), fine-tuning, and LLMOps, to create a production-ready application.

## 🚀 Features

  - **Data Ingestion**: Automates the collection and processing of data from Notion and other web resources.
  - **RAG System**: Implements an advanced RAG pipeline for efficient and accurate information retrieval.
  - **LLM Fine-Tuning**: Fine-tunes an open-source LLM for specialized summarization tasks.
  - **Modular Architecture**: Built on the **Feature/Training/Inference (FTI)** architecture for scalable and maintainable MLOps.
  - **Observability**: Integrates monitoring and evaluation to track performance and prevent hallucinations.

## 📁 Project Structure

```bash
.
├── apps / 
|   ├── infrastructure/           # Docker infrastructure for the applications
|   ├── second-brain-offline/     # Offline ML pipelines
|   └── second-brain-online/      # Online inference pipeline = our AI assistant
└── docs/                         # Documentation and diagrams
```

## 🛠️ Technology Stack

  - **Orchestration**: ZenML
  - **Data Stores**: MongoDB, S3
  - **Vector Search**: MongoDB Atlas Vector Search
  - **LLMs**: Llama (Fine-tuned)
  - **Deployment**: Hugging Face Dedicated Endpoints
  - **Observability**: Opik
  - **Core Libraries**: PyTorch, Hugging Face `transformers`

## 🖥️ Demo Video
<video src="https://github.com/user-attachments/assets/bfea8e24-6d52-4a33-8857-5d05154ab69e"></video>

