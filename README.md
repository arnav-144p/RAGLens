# RAGLens

A lightweight project for evaluating **Retrieval-Augmented Generation (RAG)** pipelines.

RAG systems can generate convincing answers even when the retrieved context is poor or the answer is not grounded in the source documents. This project explores how to measure the quality of both **retrieval** and **generated responses**.

## What it evaluates

### Retrieval

Measures whether the system retrieves useful and relevant context for a given query.

### Response

Measures whether the generated answer is relevant, grounded in the retrieved context, and answers the question correctly.

## Pipeline

**Documents → Chunking → Retrieval → Context → LLM → Answer → Evaluation**

The project experiments with different evaluation metrics to understand where a RAG pipeline performs well and where it fails.

## Tech Stack

* Python
* LlamaIndex
* LLMs
* Embeddings
* RAG
* RAG Evaluation

## Goal

The goal is to understand **how to objectively evaluate a RAG system**, rather than judging its quality only by manually looking at a few generated answers.

## Key Takeaways

* Retrieval quality directly affects answer quality.
* Different chunking and embedding strategies can produce different results.
* LLM-based evaluation can help automate large-scale testing.
* A good RAG system needs evaluation at both the **retrieval and generation** stages.

## References

* [LlamaIndex](https://docs.llamaindex.ai/)
* [OpenAI RAG Evaluation](https://github.com/openai/openai-cookbook/blob/main/examples/evaluation/Evaluate_RAG_with_LlamaIndex.ipynb)
