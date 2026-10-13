# CourseMind

> **Your AI study buddy.**

CourseMind is an AI study assistant that answers questions from your lecture notes with source citations, generates quizzes, and tracks your weak topics. Built with LangChain, LangGraph and RAG.

🚧 **Status:** Work in progress. Built step by step while learning LLM orchestration.

---

## Features

- [ ] **Upload course materials:** lecture slides and PDFs
- [ ] **Ask questions:** answers are grounded in your own notes (RAG)
- [ ] **Source citations:** every answer shows where it came from (e.g. *Week 5 slides, p. 12*)
- [ ] **Topic summaries:** short summaries of any lecture or topic
- [ ] **Exam prep mode:** generates quizzes, grades your answers and tracks weak topics (LangGraph agent)
- [ ] **Visual understanding:** reads diagrams, formulas and handwritten notes (multimodal LLM)
- [ ] **Evaluation:** a test set to measure answer accuracy

## Tech Stack

| Layer | Tools |
|---|---|
| LLM orchestration | LangChain, LangGraph |
| Retrieval | RAG, vector database (Chroma) |
| Models | OpenAI API (open-source models planned) |
| Language | Python |

## Project Structure

```
coursemind/
├── data/raw/          # Your lecture PDFs (not committed)
├── eval/              # Evaluation questions and results
├── notebooks/         # Experiments
├── src/coursemind/    # Source code
├── .env.example       # Environment variable template
└── requirements.txt
```

## Getting Started

```bash
git clone https://github.com/esra-yasar/coursemind.git
cd coursemind
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env             # then add your API keys
```

## Roadmap

1. Basic RAG over lecture PDFs
2. Source citations in answers
3. Topic summaries
4. Quiz agent with LangGraph
5. Multimodal support for slides and handwritten notes
6. Evaluation set and accuracy report

## Author

**Esra Yaşar** · [GitHub](https://github.com/esra-yasar) · [LinkedIn](https://linkedin.com/in/esrayasar)
