# Fundamental Stock Analysis with LLMs and Qualitative Data

**Course:** Final Year Project (Proposal Phase)  

## Abstract  
This project explores the use of natural language processing techniques, specifically Large Language Models (LLMs), for fundamental stock analysis by leveraging qualitative data in corporate financial reports and disclosures. It addresses information overload faced by retail investors by automating collection, processing, and interpretation of unstructured texts. The system employs a multi-agent architecture integrating web scraping of financial reports, LLM-based summarization of lengthy documents, and embedding the resulting summaries into a vector database to enable semantic search and efficient information retrieval. Using vector embeddings and retrieval-augmented generation, the system acts as a “virtual analyst” that retrieves relevant information and synthesizes coherent responses to complex investor queries about a company’s fundamentals.

## Project Overview  
- **Objective:** Develop a prototype “virtual stock analyst” tool that automates qualitative fundamental analysis of companies.  
- **Key Features:**  
  - Ingest annual and quarterly reports from Bursa Malaysia.  
  - Summarize and interpret PDF reports using Google Gemini and OpenAI.  
  - Store summaries in MongoDB/GridFS and Pinecone vector index for semantic retrieval.  
  - Support user queries over embedded summaries via Pinecone and LLM back-end.

## Technical Details  
- **Language:** Python  
- **Frameworks & Libraries:**  
  - Streamlit for UI  
  - requests, curl_cffi, BeautifulSoup for web scraping  
  - pymongo, gridfs for MongoDB integration  
  - openai, tiktoken for embeddings  
  - pinecone-client for vector database  
  - google-generativeai for summarization  
- **Datastores:** MongoDB, Pinecone  
- **Models:**  
  - Embedding: `text-embedding-3-small` (OpenAI)  
  - Summarization: `gemini-2.5-pro-preview-06-05` (Google)  
  - Chat: GPT-4.1-nano (for Q&A synthesis)

