# MQ Learning: AI-Powered Trait Feedback and Psychometric Modeling

## Project Overview

MQ Learning is a psychological assessment tool designed to measure and interpret individual motivational traits using a combination of psychometric methods and natural language processing. Users complete a 20-minute digital assessment that evaluates core dimensions such as independence, curiosity, altruism, and collaboration.

Using these inputs, the platform leverages Large Language Models (LLMs) with Retrieval-Augmented Generation (RAG) to generate tailored, research-backed feedback in real time. The goal is to provide users with accurate and actionable insights that can be applied to personal development, career alignment, team dynamics, and educational support.

This project was built as a student-led initiative exploring the intersection of behavioral science and machine learning.

Check out the website! 
[MQ LEARNING](https://mq.equalearning.net/)
---

## Objectives

- Design and deploy a psychometric engine capable of scoring behavioral traits based on structured questionnaire data.
- Generate adaptive and personalized written feedback using an LLM fine-tuned for psychological interpretation.
- Employ Retrieval-Augmented Generation (RAG) to enhance trait feedback with relevant research literature and real-world analogies.
- Visualize comparative trait scores and benchmarks across anonymized global datasets.

---

## Key Features

- **Real-Time Trait Feedback**: Personalized narratives are generated instantly after assessment completion.
- **RAG-Enhanced Prompting**: Trait feedback is dynamically constructed using modular prompts and external knowledge bases.
- **User Comparison Visuals**: Trait scores are benchmarked across a larger sample to offer perspective and context.
- **Use Case Versatility**: Designed for applications in education, coaching, hiring, personal development, and career counseling.

---

## System Workflow

1. **Assessment Completion**: Users respond to a set of Likert-scale and situational questions.
2. **Score Computation**: Individual trait scores are computed through a custom scoring function.
3. **Prompt Construction**: Trait scores are injected into pre-structured prompts along with behavioral labels and examples.
4. **RAG Pipeline**: Each prompt queries a vectorized knowledge base to retrieve trait-relevant material.
5. **LLM Response Generation**: A final LLM call returns written feedback for each trait, grounded in retrieved context.
6. **Output Delivery**: Feedback is rendered as a user-facing report with visual summaries.

---

## Technology Stack

- **Languages & Tools**: Python, Markdown
- **Libraries**: NumPy, pandas, scikit-learn, matplotlib, LangChain
- **APIs**: OpenAI API (for LLM integration)
- **Frameworks**: Streamlit (for prototype UI)
- **Data Formats**: JSON, CSV
- **Modeling Approaches**: Prompt engineering, trait vector scoring, response filtering

---


## Sample Output

A user scoring high in independence and moderate in altruism might receive feedback such as:

> "Your responses reflect a strong preference for autonomous learning and decision-making. You are likely to thrive in self-directed environments and may prefer minimal external supervision. While you often consider others, your primary drive stems from personal curiosity and initiative. This combination suggests a balance between introspective motivation and social awareness."

---

## 
View the report[MQ Learning Report](./MQ_report.pdf)

