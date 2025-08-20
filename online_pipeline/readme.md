## **Online Pipeline(App): The User-Facing AI Assistant**

This part of the project is the live, production-ready application that serves real-time user requests. It's built to be highly available and responsive.


### Core Services

I designed and implemented the core inference services that power the AI assistant:

1. **Summarization Endpoint**: I deployed the fine-tuned Llama model as a real-time inference endpoint on **Hugging Face Dedicated Endpoints**. This service is consumed by my main agentic pipeline for efficient summarization.

2. **Agentic Pipeline**: This is the brain of the assistant. It is a an agent that uses two primary tools: a **retriever tool** that queries the pre-populated vector database for relevant information and a **summarization tool** that uses my custom fine-tuned LLM.

### Observability and Monitoring

A crucial part of this project was implementing observability to monitor the live application. I integrated **Opik** to:

* **Monitor Prompts**: I tracked the complete trace of each user query, from the initial prompt to the final answer, allowing me to see exactly how the agent used its tools and arrived at a decision.

* **Evaluate Performance**: I used Opik's evaluation framework to measure the quality and effectiveness of the agentic RAG system, providing critical feedback for future improvements.
