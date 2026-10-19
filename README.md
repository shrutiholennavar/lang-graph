# Agentic RAG with LangGraph 🦜🔍

Implementation of Reflective RAG, Self-RAG & Adaptive RAG tailored towards developers and production-oriented applications for learning LangGraph🦜🕸️.

This repository contains a refactored version of the original [LangChain's Cookbook](https://github.com/mistralai/cookbook/tree/main/third_party/langchain),

See Original YouTube video:[Advance RAG control flow with Mistral and LangChain](https://www.youtube.com/watch?v=sgnrL7yo1TE)

of [Sophia Young](https://x.com/sophiamyang) from Mistral & [Lance Martin](https://x.com/RLanceMartin) from LangChain



## Features

- **Refactored Notebooks**: The original LangChain notebooks have been refactored to enhance readability, maintainability, and usability for developers.
- **Production-Oriented**: The codebase is designed with a focus on production readiness, allowing developers to seamlessly transition from experimentation to deployment.
- **Test Coverage**: Comprehensive test coverage ensures the reliability and stability of the application, enabling developers to validate their implementations effectively.
- **Documentation**: Detailed documentation and branches guides developers through setting up the environment, understanding the codebase, and utilizing LangGraph effectively.


## What You'll Learn

- **Agentic RAG Implementation**: Build a system that can make intelligent decisions about retrieving information
- **Graph-Based Control Flow**: Use LangGraph to create sophisticated control flows for your RAG pipeline
- **Document Relevance Evaluation**: Implement logic to grade document relevance and detect hallucinations
- **Adaptive Information Retrieval**: Create a system that can switch between local knowledge and web search
- **State Management**: Implement proper state handling for complex information flows

##  Structure


| No # | Commit | Description | Key Components |
|------|--------|-------------|----------------|
| 1    | [**Start Here**] | Introduction to  Agentic RAG concepts | Overview of the project; Introduction to LangGraph and Agentic RAG architecture |
| 2    | [**Project Structure**] | Setting up the project foundation | Initialize project structure; Configure Poetry for dependency management |
| 3    | [**Ingestion**] | Setting up the vector database | Create ingestion pipeline; Implement vector store with Chroma and OpenAI embeddings |
| 4    | [**State**] | Defining the state management | Create GraphState class; Set up typed dictionaries for state tracking |
| 5    | [**Retrieve Node**] | Implementing the document retrieval | Build retrieve node; Connect retrieval to vector database |
| 6    | [**Grade Documents Node**] | Evaluating document relevance | Create document grading functionality; Implement decision logic for document relevance |
| 7    | [**Web Search with Tavily**] | Adding external search capability | Integrate Tavily search API; Implement fallback for insufficient local knowledge |
| 8    | [**Generation Node**] | Creating the answer generation component | Build generate node; Implement context-aware response generation |
| 9    | [**Graph**] | Constructing the complete LangGraph workflow | Connect all nodes into workflow; Implement conditional edges for adaptive behavior |
| 10   | [**Self-RAG**] | Adding self-evaluation capabilities | Implement hallucination detection; Create feedback loops for answer improvement |
| 11   | [**Router**] | Smart query routing | Create intelligent routing between retrieval and web search; Optimize entry point for different query types |
| 12   | [**Formatting**] | Final code formatting and cleanup | Code optimization; Final documentation improvements |

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file:

```bash
OPENAI_API_KEY=your_openai_api_key_here
TAVILY_API_KEY=your_tavily_api_key_here  # For web search capabilities
LANGCHAIN_API_KEY=your_langchain_api_key_here  # Optional, for tracing
LANGCHAIN_TRACING=true                      # Optional
LANGCHAIN_PROJECT=agentic-rag                  # Optional
```



## Prerequisites

- Python 3.10+
- Basic understanding of LLMs and RAG systems
- Familiarity with Python and vector databases (helpful but not required)


