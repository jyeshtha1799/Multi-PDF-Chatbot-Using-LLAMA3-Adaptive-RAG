# Multi-PDF Chatbot Using LLAMA3 & Adaptive RAG

## Overview

Welcome to the repository for my first Medium article on building a **Multi-PDF Chatbot** leveraging the latest in AI and machine learning technologies. This project showcases the integration of **LLAMA3**, **LangGraph**, and **Adaptive RAG** to create a powerful chatbot capable of processing and retrieving information from multiple PDF documents.

This repository contains all the necessary code to replicate the project, along with detailed comments and explanations to help you understand each step. Even though some portions of the code, especially those related to LLMs, are not explicitly included, they are described in a way that you can easily adapt and implement them.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Architecture](#architecture)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Features

- **PDF Document Handling**: Upload multiple PDF files and extract content efficiently.
- **Adaptive RAG Integration**: Utilize the latest retrieval-augmented generation framework to dynamically manage query complexity.
- **LLAMA3 Integration**: Leverage Meta's LLAMA3 for high-performance language understanding and generation.
- **LangChain & LangGraph**: Implement complex workflows and stateful applications using these powerful libraries.
- **Customizable Prompts**: Use `PromptTemplate` to fine-tune LLM interactions, including relevance grading, hallucination detection, and answer grading.
- **Graph-Based Workflow**: Implement a state graph for routing, retrieval, query transformation, and generating responses.
- **Web Search Augmentation**: Integrate Tavily's API for web search when the local vector store data is insufficient.

## Installation

### Prerequisites

- Python 3.8 or higher
- Pipenv or virtualenv for environment management
- API keys for Tavily, GPT4All, and LLAMA3 (if applicable)
- Streamlit for running the web application
- Access to LangChain and LangGraph libraries

### Setup

1. **Clone the repository**:

    ```bash
    git clone https://github.com/yourusername/multi-pdf-chatbot.git
    cd multi-pdf-chatbot
    ```

2. **Install dependencies**:

    ```bash
    pipenv install
    pipenv shell
    ```

3. **Set up environment variables**:

    Create a `.env` file in the root directory and add the following:

    ```bash
    TAVILY_API_KEY=your_tavily_api_key
    GPT4ALL_API_KEY=your_gpt4all_api_key
    LLAMA3_API_KEY=your_llama3_api_key
    ```

4. **Install LangChain and LangGraph**:

    Make sure you have LangChain and LangGraph installed in your environment. You can install them using the following commands:

    ```bash
    pip install langchain
    pip install langgraph
    ```

5. **Configure LLAMA3**:

    If you're using LLAMA3 with an API, ensure that you have the correct API key and endpoint. Set this up in your environment variables as shown above.

6. **Run the application**:

    ```bash
    streamlit run main.py
    ```

## Usage

1. **Upload PDF Files**: Use the sidebar to upload multiple PDF files.
2. **Ask Questions**: Type your question in the input field.
3. **Process**: Click the "Process" button to start the chatbot.
4. **View Responses**: The chatbot processes your query and returns a response based on the documents or web search.

## Architecture

This project is built using a combination of the following components:

- **LangChain**: For handling core AI model interactions and workflow management. LangChain allows you to integrate various models and tools into a unified workflow.
- **LangGraph**: To create and manage complex stateful applications. LangGraph provides the structure to implement stateful interactions and manage complex workflows in a chatbot.
- **LLAMA3**: A cutting-edge language model by Meta, used for understanding and generating human language. LLAMA3 is highly efficient and can be configured for various NLP tasks.
- **Adaptive RAG**: Ensures optimal retrieval strategies based on query complexity, enhancing the chatbot's ability to provide accurate and efficient responses.
- **Streamlit**: A web framework for deploying the chatbot as an interactive web app.

## Technologies Used

- **Python**: The primary language used for this project.
- **LLAMA3**: A language model by Meta.
- **LangChain**: For interacting with AI models and managing workflows.
- **LangGraph**: For building stateful applications.
- **Streamlit**: For building the user interface.
- **Tavily API**: For web search capabilities.
- **Chroma**: A vector store for efficient document retrieval.

## Contributing

Contributions are welcome! If you'd like to contribute, please fork the repository, make your changes, and submit a pull request. Ensure that your code is well-documented and thoroughly tested.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
