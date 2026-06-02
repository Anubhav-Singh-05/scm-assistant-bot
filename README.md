# SCM Assistant Bot

## Overview

This project demonstrates the development of a Supply Chain Management Assistant using Flowise, Google Gemini, Pinecone and Supabase.

The objective was to ingest supply chain documents, generate embeddings, store them in a vector database, and create a Retrieval-Augmented Generation (RAG) chatbot.

---

## Technology Stack

- Flowise
- Google Gemini 2.0 Flash
- Google Gemini Embeddings
- Pinecone Vector Database
- Supabase PostgreSQL

---

## Documents Used

1. supplier_performance_data.csv
2. SupplyChain_Governance_Policy_v3.2.pdf

---

## Embedding Model

Model: gemini-embedding-001

Embedding Dimension: 3072

---

## Vector Database

Pinecone

Index Name:

supply-chain-rag

---

## Record Manager

Supabase PostgreSQL

---

## Chunk Configurations Tested

### Configuration 1

Chunk Size: 1000

Chunk Overlap: 200

Results:

- supplier_performance_data.csv → 800 chunks
- SupplyChain_Governance_Policy_v3.2.pdf → 16 chunks

### Configuration 2

Chunk Size: 500

Chunk Overlap: 100

Results:

- supplier_performance_data.csv → 4000 chunks
- SupplyChain_Governance_Policy_v3.2.pdf → 35 chunks

---

## Work Completed

- Created Flowise Document Store
- Loaded CSV and PDF documents
- Configured Recursive Character Text Splitter
- Configured Gemini Embeddings
- Connected Pinecone Vector Store
- Connected Supabase Record Manager
- Successfully generated chunks
- Successfully stored records in Pinecone
- Successfully stored upsertion records in Supabase

---

## Screenshots

All screenshots are available in the screenshots folder.

---

## Challenges Encountered

- Pinecone dimension mismatch errors
- Supabase connection issues
- SSL certificate issues
- Retriever configuration issues inside Flowise cloud

These issues were investigated and partially resolved during implementation.

---

## Future Improvements

- Complete Retriever integration
- Deploy public chatbot endpoint
- Add source citations
- Add conversational memory
- Add production deployment

## Chatflow Information

Chatflow Name: chatflow1

Chatflow ID:

d8e5d767-72bc-4e4b-a29a-4ee602e2224b

The chatflow was created successfully in Flowise and an API endpoint was generated. However, due to Flowise cloud configuration/retrieval issues, a complete exportable JSON workflow file could not be generated.
