# MQ Learning 🎯  
*AI-Powered Trait Feedback Using LLMs + Psychometric Modeling*

## Overview

MQ Learning is a psychological assessment tool built to help users understand their **motivational traits**—like curiosity, independence, altruism, and more—through a personalized 20-minute test. The platform uses **Large Language Models (LLMs)** with **Retrieval-Augmented Generation (RAG)** to generate real-time feedback grounded in behavioral research.

Our goal is to bridge the gap between AI-driven personalization and traditional psychometrics, offering a fun, data-backed way to reflect on how we learn, work, and grow.

---

## 🔍 Key Features

- ✍️ **20-minute psychological test** with research-aligned questions  
- 🧠 **LLM feedback generation** tailored to user trait scores  
- 📚 **RAG pipeline** fetches relevant theory and examples for adaptive outputs  
- 📊 Visual trait reports benchmarked against global data  
- 🧩 Use cases: education, career alignment, HR tools, coaching, relationships

---

## 📌 How It Works

1. **Users complete an assessment** (Likert-style + scenario-based questions)
2. **Trait scores** (e.g. for independence, altruism, curiosity) are calculated
3. A **prompt pipeline** feeds these scores + user context into an LLM
4. LLM generates **adaptive feedback** using RAG (theory + real-world analogies)
5. Results are returned with **visuals, comparisons**, and takeaways

---

## 💻 Tech Stack

- `Python` (scikit-learn, NumPy, pandas)
- `OpenAI API` + `LangChain`
- `RAG (Retrieval-Augmented Generation)`
- `Markdown` + `Streamlit` (for UI prototyping)
- `Matplotlib` (for trait visualization)

---

## 🧪 Sample Trait Feedback

<img src="./demo/trait_feedback_sample.png" width="600"/>

---

## 🧠 Example Use Case

Let’s say you score high in **independence** and low in **team-driven curiosity**.  
Your feedback might say:

> "You tend to explore problems on your own terms, often preferring self-direction over external validation. People like you thrive in flexible environments with space to initiate and adapt. Compared to peers, your curiosity feels more inward-driven—less about collaboration, more about mastery."

> However, you can always ask the RAG model for advice, comparisons, statistics, graphs etc. Give it a try!

---

## 📂 Repository Breakdown

| Folder        | Description |
|---------------|-------------|
| `app/`        | LLM prompt pipeline, RAG logic, prompt templates |
| `data/`       | Sample (anonymized) trait data |
| `notebooks/`  | Jupyter notebooks for scoring and exploratory analysis |
| `demo/`       | Sample outputs and images |
| `requirements.txt` | Required Python libraries |

---
