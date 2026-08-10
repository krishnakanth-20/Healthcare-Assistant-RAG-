#  Healthcare AI Assistant using Retrieval-Augmented Generation (RAG)

An AI-powered Healthcare Question Answering System that combines **Large Language Models (LLaMA-2)** with **Retrieval-Augmented Generation (RAG)** to provide accurate, evidence-based medical responses using the **Merck Manuals** as the knowledge source. The system retrieves relevant medical content before generating answers, improving reliability and reducing hallucinations.

---

##  Project Overview

Healthcare professionals often need quick access to trusted medical information for diagnosis and treatment decisions. Traditional Large Language Models rely only on pre-trained knowledge, which may be outdated or unsupported by medical references.

This project addresses that challenge by implementing a **Retrieval-Augmented Generation (RAG)** pipeline that retrieves relevant information from the **Merck Manuals** before generating responses using **LLaMA-2 13B Chat**.

---

##  Objectives

- Build an AI-powered healthcare assistant.
- Retrieve relevant information from the Merck Manuals.
- Generate accurate, context-aware medical responses.
- Reduce hallucinations through document retrieval.
- Evaluate responses using Groundedness and Relevance metrics.

---

##  Technologies Used

- Python
- Google Colab
- LangChain
- LLaMA-2 13B Chat (GGUF)
- llama-cpp-python
- Hugging Face Hub
- Sentence Transformers
- Chroma Vector Database
- PyMuPDF
- Pandas

---

## Dataset

**Knowledge Source:**
- Merck Manuals (Medical Reference PDF)

**Dataset Details**
- More than **4,000 pages**
- Covers diseases, diagnosis, treatment, medications, and clinical procedures
- Used as the knowledge base for document retrieval

---

## ⚙ Project Workflow

```
Medical PDF
      │
      ▼
Load PDF using PyMuPDF
      │
      ▼
Text Chunking
      │
      ▼
Sentence Embeddings
      │
      ▼
Chroma Vector Database
      │
      ▼
Similarity Search
      │
      ▼
Relevant Medical Context
      │
      ▼
LLaMA-2 13B Chat
      │
      ▼
Evidence-Based Medical Response
```

---

## Model Pipeline

### 1. Prompt Engineering
- Uses LLaMA-2 without document retrieval.
- Generates answers from pretrained knowledge.

### 2. Retrieval-Augmented Generation (RAG)
- Retrieves relevant medical content from the Merck Manuals.
- Supplies retrieved context to the LLM.
- Produces evidence-based responses.

---

## Evaluation Metrics

The generated responses are evaluated using:

- Groundedness Score
- Relevance Score

The evaluation compares:

- Prompt Engineering
- Retrieval-Augmented Generation (RAG)

---

## Results

| Model | Performance |
|---------|-------------|
| Prompt Engineering | Generates medically relevant responses but lacks supporting evidence. |
| RAG | Produces accurate, grounded, and evidence-based responses using retrieved medical documents. |

---

## Best Model

**Retrieval-Augmented Generation (RAG)**

### Why RAG?

- Higher Groundedness
- Better Relevance
- Reduced Hallucination
- Context-aware Responses
- Evidence-based Medical Information
- Trusted Clinical Knowledge

---

## Sample Workflow

```
User Question
      │
      ▼
Retriever
      │
      ▼
Relevant Medical Chunks
      │
      ▼
LLaMA-2
      │
      ▼
Evidence-Based Answer
```

---

## References

- Merck Manuals
- LangChain Documentation
- Hugging Face
- Chroma DB
- Sentence Transformers
- LLaMA-2

---

## Author

**Krishnakanth R**

Final Year B.E. Computer Science and Engineering

---

## Conclusion

This project demonstrates that integrating **Retrieval-Augmented Generation (RAG)** with **LLaMA-2** significantly improves the quality of medical question answering. By retrieving trusted information from the **Merck Manuals**, the system generates responses that are more accurate, relevant, and grounded in authoritative medical knowledge. Compared with traditional prompt engineering, the RAG-based approach provides greater transparency, minimizes hallucinations, and is better suited for real-world healthcare decision support applications.