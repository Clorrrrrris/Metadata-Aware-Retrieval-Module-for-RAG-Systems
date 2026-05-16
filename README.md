# Graph-Guided Retrieval for Textbook-based RAG Systems

A lightweight metadata-aware Retrieval-Augmented Generation (RAG) system that combines dense vector retrieval with hierarchical graph expansion for educational question answering and summarization.

## Overview

This project explores how textbook structure can improve retrieval quality in RAG systems. Instead of relying solely on embedding similarity, the system builds a metadata graph from textbook chapter and section hierarchies and performs graph-guided retrieval expansion before re-ranking.
The project was evaluated on the OpenStax Psychology 2e textbook using both fine-grained QA and chapter-level summarization tasks.


## Results

### Fine-grained QA Retrieval

- Recall@5 improved from **0.14 → 0.34**

- Hit@5 improved from **0.53 → 0.66**

### Chapter-level Summarization

- Recall@20 improved from **0.14 → 0.54**

- Hit@20 improved from **0.40 → 0.80**

### Efficiency

- Indexed a 751-page corpus in ~45 seconds

- Added only ~1 ms retrieval overhead compared to baseline vector search

## Tech Stack

- Python

- ChromaDB

- NetworkX

- Sentence Transformers

- MiniLM

- PyPDF2

- pdfplumber

## My Contributions

- Designed the metadata graph logic

- Implemented the graph-guided retrieval module

- Set up the LLM and retrieval environment

- Defined Recall and MRR evaluation metrics

- Wrote the Abstract, Introduction, Data, and Methodology sections

## Repository Structure

```text

data/           # Processed textbook and evaluation data

retrieval/      # Retrieval and graph expansion modules

evaluation/     # Benchmarking and evaluation scripts

notebooks/      # Experiment notebooks

report/         # Final project report
