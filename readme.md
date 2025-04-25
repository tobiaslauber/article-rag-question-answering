# RAG Project

This project implements a **Retrieval-Augmented Generation (RAG)** pipeline for answering questions based on a provided dataset of articles.

## Project Structure

- **`data/`**  
  Contains the datasets used in the project:
  - Raw and cleaned CSV files of articles.
  - An evaluation dataset provided to students for testing the RAG system.

- **`articles/`**  
  Contains the articles converted to `.txt` files to simplify processing and retrieval.
  The folder gets created, when we run the ArticlesExtractor class. We can find the code in the `RAG.ipynb` notebook in the section __exporing the dataset__.

- **`databases/`**  
  Stores the 12 different vector databases:
  - Built using either **FAISS** or **Chroma**.
  - Created with **6-layer** or **12-layer** chunking.
  - Chunked by **characters**, **tokens**, or **recursive** methods.
  
  All possible combinations add up to 12 databases.

- **`requirements.txt`**  
  Lists all the Python packages required to run the project.

- **`RAG.ipynb`** and **`RAG.html`**  
  The main notebook and its exported HTML version:
  - Walks through the complete RAG workflow.
  - Includes data preprocessing, database building, retrieval logic, model integration, and evaluation.
  - Contains detailed explanations, visualizations, and analysis at each step.

## How to Run

1. Install the required packages:
   ```bash
   pip install -r requirements.txt
    ```

## Usage of ChatGPT

All of the work in this project is my own.  
ChatGPT was occasionally used as a writing assistant to help rephrase or improve the readability of text that I originally wrote.  
Any output from ChatGPT was always carefully reviewed, edited, and verified by me, since it can sometimes silently introduce unintended changes.