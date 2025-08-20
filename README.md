# 🧠 Antahkarana: Your Second Brain AI Assistant

Antahkarana(The Inner Instrument) is one of my dear projects that is a personal AI second brain assistant on top of your digital resources. It leverages advanced GenAI concepts, including Retrieval-Augmented Generation (RAG), fine-tuning, and LLMOps, to create a production-ready application.

## 🚀 Features

  - **Data Ingestion**: Automates the collection and processing of data from Notion and other web resources.
  - **RAG System**: Implements an advanced RAG pipeline for efficient and accurate information retrieval.
  - **LLM Fine-Tuning**: Fine-tunes an open-source LLM for specialized summarization tasks.
  - **Modular Architecture**: Built on the **Feature/Training/Inference (FTI)** architecture for scalable and maintainable MLOps.
  - **Observability**: Integrates monitoring and evaluation to track performance and prevent hallucinations.

## 📁 Project Structure

```
.
├── offline_pipelines/
│   ├── etl_pipeline/               # Data collection and preprocessing (Notion, web crawling)
│   ├── feature_pipelines/          # RAG and dataset generation
│   ├── training_pipeline/          # Fine-tuning the LLM
│   └── zenml_orchestrator/         # ZenML configurations for pipeline orchestration
│
├── online_app/
│   ├── api/                        # FastAPI/Gradio UI for the agentic inference pipeline
│   ├── llm_endpoint/               # Deployed summarization LLM
│   └── observability/              # Prompt monitoring and evaluation with Opik
│
├── docs/                           # Diagrams, project architecture, and technical explanations
├── notebooks/                      # Exploratory data analysis and PoCs
└── README.md
```

## 🛠️ Technology Stack

  - **Orchestration**: ZenML
  - **Data Stores**: MongoDB, S3
  - **Vector Search**: MongoDB Atlas Vector Search
  - **LLMs**: Llama (Fine-tuned)
  - **Deployment**: Hugging Face Dedicated Endpoints
  - **Observability**: Opik
  - **Core Libraries**: PyTorch, Hugging Face `transformers`

  ### 📄 README: `offline_pipeline/README.md`
  ### 📄 README: `online_pipeline/README.md`
