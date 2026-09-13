# RAG Financial Chatbot

A RAG chatbot built with **n8n** that answers questions using financial reports stored in a Pinecone vector database.

The project automatically gets new reports from Google Drive, processes them, creates embeddings using OpenAI, and stores them in Pinecone. The AI Agent then retrieves the relevant information to answer user questions.

## Features

* Automatically checks Google Drive for new reports
* Tracks processed files using Google Sheets
* Splits documents into smaller chunks
* Creates embeddings using OpenAI
* Stores and searches documents using Pinecone
* Uses an AI Agent to answer questions based on the reports

## Workflow

**Google Drive → Document Processing → OpenAI Embeddings → Pinecone → AI Agent → Answer**

## Technologies

* n8n
* OpenAI API
* Pinecone
* Google Drive
* Google Sheets
* RAG
* JavaScript

## Setup

1. Import `workflow.json` into n8n.
2. Add your own OpenAI, Pinecone, Google Drive, and Google Sheets credentials.
3. Configure your own Drive folder, Google Sheet, and Pinecone index.
4. Run the workflow to process the reports.
5. Use the chat trigger to ask questions about the reports.
