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
# MQ Learning: Reimagining Motivation with Psychometric Modeling & Softmax Scoring

## Overview

**MQ Learning (Motivation Quotient Learning)** is an innovative psychological insight platform that decodes an individual’s internal motivators using a proprietary trait-based assessment. It evaluates over 24 psychological “DNA traits” like **Curiosity**, **Ingenuity**, **Altruism**, and **Order**, then clusters them into six high-level motivational archetypes: **Innovator, Visioner, Practitioner, Integrator, Producer, and Administrator**.

Using a machine learning-inspired scoring model, MQ generates **personalized Motivation Maps** that more accurately reflect the salience of high-impact traits—empowering students, educators, HR teams, and coaches to make better-aligned decisions.

---

## 🎯 Project Objectives

- Replace outdated average-based scoring with a **Softmax-weighted scoring system** to better reflect motivation intensity.
- Validate the new model with **A/B testing**, user feedback, and statistical comparisons.
- Develop scalable tools for **visualizing**, **benchmarking**, and **analyzing** individual and group motivational profiles.
- Bridge psychometric insights with real-world application in **education**, **career guidance**, **team formation**, and **wellness coaching**.

---

## 🚀 Key Features

- **Softmax-Based Motivation Map**  
  Captures motivational "spikes" by emphasizing dominant psychological traits using a softmax-weighted formula.

- **A/B Testing Validation**  
  Compared the new softmax method against traditional averaging across 6 archetypes using t-tests and user-level metrics.

- **Visualization Dashboard (R & ggplot2)**  
  Includes comparative bar charts, line graphs, and density plots to explain differences in scoring models and trait distributions.

- **Modular Code Design**  
  R scripts allow users to input new datasets, apply softmax scoring, and generate both summary tables and visual diagnostics.

---

## 🔢 Methodology & Algorithms

### Old Model:
Scores were averaged across traits within a category. This diluted the influence of dominant traits.

### New Model: Softmax Score  
We use:


Where `T = 10` (temperature) emphasizes higher trait scores while still incorporating all relevant values. Lower `T` makes sharper spikes.

---

## 📊 Validation Results

### A/B Test Design:
- **Group A (Control):** Users scored by average method  
- **Group B (Treatment):** Users scored using Softmax

We tested how well each method differentiated “top 25%” students using **t-tests across all six categories**.

### Highlights:
| Category      | Mean t-stat | Softmax t-stat | Softmax More Significant? |
|---------------|-------------|----------------|----------------------------|
| Innovator     | -11.51      | **-11.70**      | ✅                        |
| Visioner      | -11.31      | **-12.11**      | ✅                        |
| Practitioner  | -13.16      | **-14.86**      | ✅                        |
| Integrator    | -10.01      | **-10.71**      | ✅                        |
| Producer      | -9.72       | **-10.17**      | ✅                        |
| Administrator | -13.01      | **-12.11**      | ✅                        |

- **Density plots** show Softmax scores are more right-skewed → better at identifying highly motivated individuals.
- **Scatter plots** confirm strong correlation between scoring methods, but Softmax better highlights “motivated outliers”.

---

## 📈 Visual Examples

| Mean vs. Softmax Bar Chart | Score Sensitivity Curve |
|----------------------------|--------------------------|
| ![](./unnamed-chunk-3-1.pdf)     | ![](./unnamed-chunk-6-1.pdf) |

---

## 🔍 System Stack

- **Languages:** R, Markdown
- **Libraries:** `dplyr`, `ggplot2`, `readxl`, `knitr`, `tidyr`
- **Data Source:** User-uploaded `.xlsx` assessment files
- **Output:** Motivation Maps (tables + visualizations)

---

## 📘 Use Cases

- 🎓 **Students:** Align study habits and course choices to motivational archetypes  
- 🧠 **Counselors & Coaches:** Use data-backed maps to initiate meaningful development conversations  
- 💼 **HR Teams:** Enhance hiring and team formation through alignment with core motivations  
- 🧬 **Self-Development:** Empower users with actionable insights into what truly drives them

---

## 📌 Future Directions

- Add support for dynamic web-based interface (e.g., using Streamlit or Shiny)
- Integrate RAG-based feedback generation (LLM + trait prompts)
- Build exportable Motivation Reports for educational or workplace integration
- Expand to HEXACO or Big Five alignment

---

## ✍️ Author

**Alex Qiu**  
Psychometric Researcher | Data Science Student | Developer of MQ Learning  
Built and validated the Softmax model, implemented A/B testing, and authored the research & report.

---

## 📄 Reference
If you’re curious about the full implementation or the methodology write-up, check out the detailed [MQ Learning Report](./MQ_Report.pdf).

---
