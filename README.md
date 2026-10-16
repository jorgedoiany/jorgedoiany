<h1 align="center">
  Hey, I'm Jorge Peguero 👋
</h1>

<p align="center">
  <strong>AI Engineer · LLM, RAG & Agentic Workflows</strong><br>
  Auditable AI · Dominican Republic
</p>

<p align="center">
  <a href="https://readme-typing-svg.herokuapp.com">
    <img src="https://readme-typing-svg.herokuapp.com?font=Inter&size=22&pause=1000&color=38BDF8&center=true&vCenter=true&width=700&lines=AI+Engineer;LLM%2C+RAG+%26+Agentic+Workflows;LangGraph+%26+MCP;Auditable+AI">
  </a>
</p>

---

## 🧠 About Me

AI Engineer focused on LLM, RAG and agentic systems that are traceable and testable. M.Sc. in Artificial Intelligence (UNIR): program completed Feb. 2026, degree conferral expected 2027.

- **Transgenia (AI Engineer Intern, Sep. 2025 – Jan. 2026):** built an internal LLM contract-analysis MVP that cut contract review time by ~65% (from 25 to 6–8 minutes) across 20+ contracts, and reduced token usage by 85–90% through prompt compression and context control. Model calls are audit-logged for traceability.
- **On my own:** a LangGraph MVP that separates deterministic validation from RAG-based legal reasoning, with a citation validation layer, and an MCP server with a Strands agent on Amazon Bedrock for an Amazon hackathon.
- **Dominican Republic Film Commission (DGCINE), Data Analyst, since May 2021:** I designed the rule-based validation logic and reviewed 100% of more than 700 validation case files for a fiscal incentive program that has approved more than $326M USD, identifying 2,539+ non-admissible expenses (~$470K USD).

---

## 📂 AI Projects

### 🎬 Film Tax Credit Compliance Engine (MVP)
**LangGraph · RAG · Ollama · Python**

Agentic MVP built with LangGraph that supports tax credit eligibility decisions for Dominican audiovisual productions under Art. 39. It combines deterministic, SQL-driven financial validation with RAG-based legal reasoning on a local LLM (Ollama). A citation validation layer restricts the LLM to cite only retrieved legal text, so every cited source is traceable to the legal text. Verified with 4/4 passing tests covering expense validation, compliance flow and citation integrity.

🔗 https://github.com/jorgedoiany/film-tax-credit-agent

---

### 🧩 Amazon Hackathon: MCP Server and Agent (MVP)
**MCP · Strands Agents · Amazon Bedrock · FastAPI** · *private repository*

MCP server (FastMCP, Streamable HTTP) with four stateful tools and SQLite-backed project state, so a project can be built across several conversation turns. A Strands agent, using Claude on Amazon Bedrock as the model provider, connects to the tools through a FastAPI client that simulates a voice assistant. It reuses deterministic validation engines from the Film Tax Credit Compliance Engine, wrapped with adapters that label every figure as self-reported and not validated. Covered by 50 pytest tests across the engines, adapters and MCP tools over a real client session.

---

### 📄 Dominican Film Data Pipeline (MVP)
**OCR · Document Intelligence · PostgreSQL**

Document intelligence pipeline built over 2,543 DGCINE fiscal-incentive resolutions spanning 14 years. It combines direct parsing, Tesseract OCR (which handled 96.6% of documents) and GPT-4o Vision on Azure OpenAI as a fallback for low-quality scans. Confidence scoring across 15 critical fields flags low-confidence records for manual review, and entity normalization covers RNC validation, currency parsing, ISO date standardization and OCR artifact correction. A manual review of 50+ documents that initially failed extraction revealed three template versions across the 14 years, and rewriting the extraction patterns for each made most of them parse correctly. Data is stored in a 5-table relational schema (SQLite, migrated to PostgreSQL on Supabase), and incremental processing cut monthly runs from 60–90 minutes to under 5 seconds for already-processed documents.

🔗 https://github.com/jorgedoiany/dominican-film-data-pipeline

---

### 🎥 Film Location Recommender (MVP, M.Sc. thesis)
**NLP · Hybrid Recommendation · Streamlit**

Semantic search MVP built for my M.Sc. thesis at UNIR (*"Sistema de recomendación de locaciones cinematográficas mediante PLN y aprendizaje automático"*, defended). The user enters a narrative scene description and the system returns ranked film location suggestions from a dataset of 208 film locations from the Dominican Republic, using a hybrid NLP approach that combines TF-IDF with MiniLM and XLM-R sentence embeddings. The hybrid model reached a mean similarity score of 0.815 versus 0.13 for the TF-IDF baseline (6.3x) across 12 test queries, with inference in under 2 seconds. Built with Python, spaCy, Sentence-Transformers, scikit-learn and Streamlit.

🔗 https://github.com/jorgedoiany/film-location-recommender-pilot

---

### 🛰️ Amazon Deforestation Segmentation (MVP)
**Classical Computer Vision · Temporal Analysis · OpenCV**

Classical computer vision MVP that estimates vegetation loss in natural-color Landsat frames of the BR-163 corridor (Pará, Brazil), using 20 annual frames (2000–2019) from a NASA Earth Observatory time-lapse. Compares three methods: a Sobel gradient baseline, HSV vegetation loss, and HSV + LAB with cloud masking and morphological cleaning. A time-series engine over 19 annual transitions identifies acceleration, peak-loss periods and persistent deforestation. Includes CLI tools, a Python API, a synthetic data generator and 115 pytest tests (76% coverage). Built with Python, OpenCV, NumPy and scikit-image.

🔗 https://github.com/jorgedoiany/amazon-deforestation-segmentation

---

### 🌙 Low-Light Image Enhancement (early MVP)
**Computer Vision · Image Processing · Evaluation Metrics**

Classical computer vision pipeline comparing Gamma Correction, CLAHE and Single-Scale Retinex (SSR), evaluated with PSNR and SSIM. Includes CLI execution, a Jupyter demo notebook and structured CSV output per run.

🔗 https://github.com/jorgedoiany/low-light-image-enhancement

---

## 🛠️ Technical Stack

### 🤖 LLMs, Agents & AI
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/MCP-000000?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/OpenAI_API-412991?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/Azure_OpenAI-0078D4?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Amazon_Bedrock-232F3E?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
</p>

- LLM pipelines · RAG · Agentic workflows · Tool use · Prompt engineering · Strands Agents · Ollama
- NLP: TF-IDF · Sentence embeddings (MiniLM, XLM-R) · spaCy
- Computer vision and OCR: OpenCV · scikit-image · Tesseract OCR

---

### 🗄️ Data & Backend
<p>
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white"/>
</p>

- Data validation · Data quality · Relational schema design · REST APIs

---

### ⚙️ Tools & Workflow
<p>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  <img src="https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white"/>
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
</p>

---

## 📈 GitHub Contribution Activity

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=jorgedoiany&theme=github-dark&hide_border=true" />
</p>

---

## 📬 Contact

<p align="center">
  <a href="https://www.linkedin.com/in/jorge-peguero/">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:jorgedoiany@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=flat&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://github.com/jorgedoiany">
    <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white"/>
  </a>
</p>

---

<sub>Last updated: October 2026</sub>
