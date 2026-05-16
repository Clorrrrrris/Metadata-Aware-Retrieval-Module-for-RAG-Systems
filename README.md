# Graph-Guided Retrieval for Textbook-based RAG Systems

A lightweight metadata-aware Retrieval-Augmented Generation (RAG) system that combines dense vector retrieval with hierarchical graph expansion for educational question answering and summarization.

## Overview

This project explores how textbook structure can improve retrieval quality in RAG systems. Instead of relying solely on embedding similarity, the system builds a metadata graph from textbook chapter and section hierarchies and performs graph-guided retrieval expansion before re-ranking.
The project was evaluated on the OpenStax Psychology 2e textbook using both fine-grained QA and chapter-level summarization tasks.
