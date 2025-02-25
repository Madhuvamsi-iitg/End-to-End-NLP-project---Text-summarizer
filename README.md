

### End-to-End NLP Project with Hugging Face and Transformers: Text Summarization

This project is an end-to-end Natural Language Processing (NLP) solution focused on **text summarization**, leveraging the power of Hugging Face's Transformers library. The goal is to automate the process of generating concise and meaningful summaries from lengthy dialogues, using state-of-the-art pre-trained models and fine-tuning them on a custom dataset.

#### Key Features:
- **Project Structure**: A robust and modular project structure was developed, including `.github workflows`, configuration files (`config`, `params.yaml`), logging, exception handling, and utility functions for seamless development and deployment.
- **Dataset**: The `Samsung/samsum` dataset from Hugging Face was used, which contains dialogues and their corresponding summaries, making it ideal for summarization tasks.
- **Model**: The `google-pegasus-cnn_dailymail` model, a pre-trained transformer-based model optimized for summarization, was fine-tuned on the custom dataset to improve performance.
- **Pipelines**: End-to-end pipelines were implemented, including:
  - **Data Ingestion**: Loading and preprocessing the dataset.
  - **Data Transformation**: Preparing the data for model training.
  - **Model Training**: Fine-tuning the Pegasus model on the `samsum` dataset.
  - **Model Evaluation**: Using **ROUGE scores** to evaluate the quality of the generated summaries against reference summaries.
  - **Prediction**: Generating summaries for new input dialogues.
- **Metrics**: ROUGE (Recall-Oriented Understudy for Gisting Evaluation) scores were used to measure the overlap between generated and reference summaries, ensuring high-quality summarization.
- **Frontend**: A user-friendly web application was developed using **FastAPI**, allowing users to input dialogues and receive summarized outputs in real-time.

#### Applications:
This project can be applied in various real-world scenarios, such as:
- Summarizing customer support conversations.
- Condensing meeting transcripts or interviews.
- Generating concise summaries of long articles or documents.

#### Technologies Used:
- **Hugging Face Transformers**: For pre-trained models and NLP pipelines.
- **FastAPI**: For building the frontend application.
- **ROUGE Metrics**: For evaluating summarization quality.
- **GitHub Actions**: For CI/CD workflows.

This project demonstrates the complete lifecycle of an NLP application, from data preparation and model fine-tuning to deployment and evaluation, making it a comprehensive resource for text summarization tasks.



### workflows
1. Update config.yaml
2. params.yaml
3. Config entity
4. Configuration manager
5. Update the components -- Data Ingestion, Data transformation, Model trainer
6. Create our pipeline -- Training pipeline, prediction pipeline