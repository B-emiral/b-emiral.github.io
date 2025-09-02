---
layout: default
title: Bilgehan Emiral - Academic Portfolio
---

# Portfolio

Welcome! This portfolio showcases projects, publications, and professional interests in Computer Science, focusing on Artificial Intelligence and Machine Learning.

## [[Portfolio Project](https://github.com/B-emiral/Portfolio)]
a lightweight, extensible LLM runtime built on a Ports & **Adapters** architecture with **async before/after hooks** (anyio). Profiles (via profiles.toml) map environments to provider/model and hooksets; the LLMClient orchestrates calls through an adapter (Anthropic, OpenAI etc.), then runs hooks for logging, **Langfuse tracing**, and **MongoDB persistence**. Outputs are parsed and validated against **Pydantic v2 models**, with clean separation of retries: network-level in the adapter, JSON parsing-only at the task layer. The system favors explicit, minimal payloads and idempotent trace handling, making it suitable for production-grade observability and schema-enforced workflows.

- Language & Tooling
  - Python 3.12
  - Poetry (in-project virtualenv)
- Core Libraries
  - Pydantic v2 (data models & validation)
  - pydantic-settings (environment config)
  - AnyIO (async runtime)
  - Tenacity (retries with backoff)
  - Loguru (hook)
- LLM Layer
  - Ports & Adapters pattern (custom AnthropicAdapter, OpenAI Adapter, etc.)
  - Runner (LLMClient)
- Guarding & Repair
  - Guardrails (Pydantic schema repair/validation)  <- hook
- Observability
  - Langfuse SDK <- hook
- Persistence
  - MongoDB <- hook
  - Pydantic schema (LLMCall) for insert validation
- Configuration
  - profiles.toml (profiles → provider/model, hooksets → before/after)
- Analytics package
  - DuckDB
  - Polars
- Data package
  - SQLModel
  - SQLAlchemy



## Academic Publications

*   **Optimizing Decision Trees for Strategic Decision-Making and Problem-Solving**
    *   Conference: *26th International Conference on Pattern Recognition (ICPR)*, Montréal, QC, Canada, August 2022.
    *   Published in: IEEE Xplore
    *   [[Paper PDF](static/PublishedPaperICPR26th@2208.pdf)] [[IEEE Link](https://ieeexplore.ieee.org/document/9956570)]

## Academic Projects

*   **Optimizing Decision Trees for Strategic Decision-Making and Problem-Solving** (M.Sc. Thesis)
    *   *Date:* Summer 2025
      * MECE-driven hierarchical decomposition for category tree generation
      * Tree-of-Thought/Graph-of-Thought style exploration with iterative refinement
      * Context-aware node expansion using sibling/“uncle” constraints to reduce overlap
      * Multi-criteria auto-grading (ME, CE, LA, RV) with rubric-based prompts
      * Acceptance thresholds and pruning as a multi-objective gating mechanism
      * Multi-sample generation per leaf with self-consistency voting/ranking
      * Beam-like top-k expansion under depth/size constraints
      * Repair/retry prompting loops for failed or low-scoring generations
      * Chained experiments across generations to assess iteration effects
      * Ablation studies isolating the impact of individual criteria (ME/CE/LA/RV)
      * Performance evaluation with F1, RMSE, and hit-rate; trade-off analysis
      * Pearson correlation analysis across criteria and metrics; heatmap visualization
      * Analysis of category-count vs. quality (e.g., corr(F1, Categories))
      * Config-driven, reproducible experiment orchestration
      * Parallel batched LLM requests with rate-limiting and backoff for robustness
      * Caching of external data/LLM responses to stabilize and accelerate runs
      * Structured reporting of results and comparative summaries across runs
  

*   **Building a Tool for Human-in-the-Loop Strategic Problem-Solving with LLMs** (M.Sc. Project)
    *   *Course:* Master-Praktikum: Ethical AI: Problems and Applications, TUM
    *   *Date:* Winter 2024
    *   *Description:* Developed an interactive, tree-based problem-solving tool leveraging LLMs to assist users in structuring and analyzing complex business cases
    *   Incorporating external knowledge retrieval and human feedback (RAG)
    *   [[Report PDF](static/LabProject2Report@2503.pdf)] [[Poster PDF](static/LabProject2Poster@2501.pdf)]

*   **Disinformation on Social Media: Truthsayer** (M.Sc. Project)
    *   *Course:* Master-Praktikum: Ethical AI: Problems and Applications, TUM
    *   *Date:* Summer 2024
    *   *Description:* Created "Truthsayer," a browser extension using NLP and LLMs to assess the truthfulness of YouTube video content in real-time by cross-referencing claims with Wikipedia data.
    *   [[Report PDF](static/LabProjectReport@2408.pdf)] [[Poster PDF](static/LabProjectPoster@2407.pdf)]

*   **Task-based & Social Conversational Agents** (M.Sc. Seminar Paper)
    *   *Course:* Master Seminar: Natural Language Processing: Methods and Applications, TUM
    *   *Date:* Winter 2024
    *   *Description:* Authored a research paper analyzing the evolution, techniques, and challenges of task-oriented and social dialogue systems, including the role of LLMs as conversational agents.
    *   [[Research Paper PDF](static/SeminarResearchPaper@2408.pdf)]

*   **Deep Hotel Recommender System Using Aspect-based Sentiment Analysis of Users' Reviews** (B.Sc. Graduation Thesis)
    *   *University Graduation Thesis:* Istanbul Technical University (ITU)
    *   *Date:* January 2022
    *   *Description:* Developed and evaluated a deep learning model combining multi-criteria collaborative filtering with aspect-based sentiment analysis of user reviews for hotel recommendations using the TripAdvisor dataset.
    *   [[Thesis Report PDF](static/GraduationProjectReport@2201.pdf)] [[Presentation PDF](static/GraduationProjectPresentation@2201.pdf)]

## Technical Skills

*   **Areas:** Machine Learning, Deep Learning, Natural Language Processing (NLP), Recommender Systems, Aspect-Based Sentiment Analysis, Large Language Models (LLMs), Ethical AI, Data Mining & Knowledge Discovery, Strategic Problem Solving, DevOps, Git, Jira, Github.
*   **Tools & Technologies:** Python, Keras, TensorFlow, NLTK, Scikit-learn, Pandas, React, TypeScript, Django
*   **Languages:** English (Fluent), Turkish (Native), German (Pre-Intermediate)

## Professional Interests
My real interest lies where AI, ML, and data science come together. I enjoy taking concepts and turning them into practical tools that solve actual problems. I'm especially drawn to the progress in NLP and the potential within LLMs for tasks like building better conversational systems. Creating models is key, but I'm also keen on the whole lifecycle – making sure ML systems are robust, deployable, and well-managed, which touches on MLOps. Finding valuable insights hidden in data and building effective, trustworthy AI solutions is what truly drives my work.

---

## Education

### **Master of Science (M.Sc.) in Informatics** 
*Technische Universität München (TUM), Munich, Germany*  
*April 2023 - September 2025*

**Key Coursework:**
- Data Mining and Knowledge Discovery
- Introduction to Deep Learning
- Natural Language Processing
- Advanced Natural Language Processing
- Master Seminar: Natural Language Processing - Methods and Applications
- Master Praktikum: Ethical AI - Problems and Applications
- Master Praktikum: Machine Learning for Natural Language Processing Applications

---

### **Bachelor of Science (B.Sc.) in Computer Engineering** 
*Istanbul Technical University (ITU), Istanbul, Turkey*  
*October 2018 - June 2022*  
**GPA: 3.11 / 4.00**

**Key Coursework:**
- Introduction to Scientific & Engineering Computing (C) [4.00 / 4.00]
- Object Oriented Programming [4.00 / 4.00]
- Analysis of Algorithms I [4.00 / 4.00]
- Analysis of Algorithms II [4.00 / 4.00]
- Data Structures
- Computer Operating Systems
- Computer Architecture
- Functional Programming (Haskell) [3.50 / 4.00]
- Software Engineering
- Database Systems [4.00 / 4.00]
- Computer Engineering Design I [4.00 / 4.00]
- Computer Engineering Design II [4.00 / 4.00]
