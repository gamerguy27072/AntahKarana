## **Offline Pipelines: The Engine Room**

This section details the batch-processing pipelines that I built to prepare the data, train the models, and manage the MLOps lifecycle. These pipelines are scheduled to run periodically and are entirely decoupled from the user-facing application.

### Data Ingestion and ETL

I created a robust data pipeline to automate the collection of my Notion notes and web resources. The process involves:

1. **Data Collection**: Fetching raw Notion documents via the API and converting them into a standardized Markdown format.

2. **ETL (Extract-Transform-Load)**: This pipeline crawls embedded links within the documents, computes a quality score using an LLM, and loads the cleaned data into a MongoDB document database for persistent storage.

### Feature Engineering and Fine-Tuning

I developed two key feature pipelines:

1. **RAG Feature Pipeline**: This pipeline processes my cleaned documents, chunks them, and generates embeddings. These embeddings are then loaded into a MongoDB vector index, ready for semantic search.

2. **Dataset Generation Pipeline**: To avoid costly API calls for summarization, I used distillation to create a custom, high-quality summarization dataset from my documents, which I then stored in a data registry.

### Training and Orchestration

Using the generated dataset, I fine-tuned a Llama model on a summarization task. I utilized **ZenML** to orchestrate all of these offline pipelines, ensuring a reproducible and version-controlled workflow. This allowed me to easily schedule runs, track metadata, and manage artifacts across the entire MLOps lifecycle.