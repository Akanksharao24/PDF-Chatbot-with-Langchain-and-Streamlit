# PDF ChatBot Using Mistral-7B-Instruct

Welcome to the PDF ChatBot project! This chatbot leverages the Mistral-7B-Instruct model and the LangChain framework to answer questions about the content of PDF files. By following this README, you'll learn how to set up and run the chatbot using Streamlit.

## Table of Contents
1. [Overview](#overview)
2. [Installation](#installation)
3. [How to Run](#how-to-run)
4. [Explanation of Code](#explanation-of-code)
5. [Resources](#resources)
6. [References](#references)

## Overview
This project aims to create a conversational agent that can answer questions about PDF documents. It utilizes:
- **Streamlit** for the web interface.
- **LangChain** for handling conversational AI and retrieval.
- **Mistral-7B-Instruct** model for generating responses.
- **FAISS** for creating a vector store to manage document embeddings.

## Installation
To get started, you need to have Python installed. Follow these steps to set up the project:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Akanksharao24/PDF-Chatbot-with-Langchain-and-Streamlit
   cd pdf-chatbot
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

## How to Run
After installing the dependencies, you can run the chatbot using Streamlit:

```bash
streamlit run app.py
```

This will launch a local web server, and you can interact with the chatbot via your web browser.

## Explanation of Code
Here's a breakdown of the main components in the code:

1. **Session State Initialization:**
   The `initialize_session_state` function sets up the session state to manage conversation history.

2. **Conversation Chat Function:**
   The `conversation_chat` function handles sending user queries to the conversational chain and updating the history.

3. **Display Chat History:**
   The `display_chat_history` function manages the user interface, displaying past queries and responses.

4. **Conversational Chain Creation:**
   The `create_conversational_chain` function sets up the language model and retrieval chain using the FAISS vector store.

5. **Main Function:**
   The `main` function handles file uploads, document loading, text splitting, embeddings creation, and initializing the conversational chain.

### Sample Interaction
1. **Upload PDFs:**
   Upload one or more PDF files via the sidebar.
   
2. **Ask Questions:**
   Enter questions about the uploaded documents, and the chatbot will generate responses based on the content.

## Resources
To better understand the technologies used in this project, here are some helpful resources:

- [Streamlit Documentation](https://docs.streamlit.io/)
- [LangChain Documentation](https://langchain.readthedocs.io/)
- [FAISS Documentation](https://faiss.ai/)
- [Hugging Face Embeddings](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.1-GGUF/tree/main)
- [other Documents](https://www.irjmets.com/uploadedfiles/paper//issue_7_july_2023/43587/final/fin_irjmets1690455507.pdf) 

## References
The following papers and articles provide a deeper insight into the methodologies and technologies utilized in this project:

- [streamlit]([https://arxiv.org/abs/1702.08734](https://github.com/mistralai/cookbook/tree/main/third_party/streamlit))

By following this guide, you'll be able to set up and run a PDF chatbot capable of answering questions about your documents. Enjoy exploring the capabilities of conversational AI!
