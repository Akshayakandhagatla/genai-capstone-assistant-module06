# GenAI Study & Placement Assistant — Module 06 Capstone Project

An end-to-end Generative AI web application built for **Module 06: GenAI Capstone Project** during my Virtual Internship at **Codomax Digital Solutions**.

## Architecture Diagram

```mermaid
flowchart LR
    U[User Query] --> A[AI Agent Router]
    A -->|Math / Checklist| T[Deterministic Tools]
    A -->|Knowledge Query| R[RAG Retriever]
    R --> KB[(Knowledge Base Chunks)]
    KB --> P[Prompt Engineering + Role]
    T --> OUT[Final Response UI]
    P --> LLM[Gemini LLM API / Local Fallback]
    LLM --> OUT
