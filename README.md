
# Scholarship Finder Chatbot

## Project Description

This project is an intelligent chatbot that answers questions about scholarships using a dataset collected through web scraping.

It uses Retrieval-Augmented Generation (RAG) to retrieve relevant scholarship information and generate answers based on the collected data.

## Dataset

The dataset contains 104 scholarship records and 8 columns:

- Name
- Sponsor
- Type
- Region
- Study Level
- Amount
- Deadline
- Application Link

The data was collected from the Open Scholarships API.

## Installation

Install the required libraries:

```bash
pip install pandas sentence-transformers faiss-cpu google-genai gradio
```

## How to Run

1. Open the project notebook in Google Colab.
2. Upload the scholarship dataset CSV file.
3. Add your Gemini API key to Colab Secrets using the name GEMINI_API_KEY.
4. Run the notebook cells in order.
5. Launch the Gradio interface and ask questions about scholarships.

## Technologies Used

- Python
- Pandas
- Sentence Transformers
- FAISS
- Google Gemini 3.5 Flash Lite
- Gradio
- Retrieval-Augmented Generation (RAG)

## Features

- Semantic search using vector embeddings.
- Relevant scholarship retrieval using FAISS.
- AI-generated answers using Gemini.
- Sources and application links in answers.
- Refusal when information is not available in the dataset.
- Simple Gradio user interface.

## Model Note

The project uses Gemini 3.5 Flash Lite through the official Google GenAI SDK because Gemini 2.5 Flash Lite was unavailable for the API key used during development.
