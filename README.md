<h1 align="center">Victor Chukwudi Robinson</h1>
<p align="center">
  <b>ML and AI engineer · London, UK</b><br>
  MSc AI and Data Science, University of East London<br>
  I build retrieval, vision and document-checking systems, and I report how they perform, including where they fail.
</p>
<p align="center">
  <a href="PORTFOLIO_LINK">Portfolio</a> ·
  <a href="https://www.linkedin.com/in/robinson-victor">LinkedIn</a> ·
  <a href="https://doi.org/10.5281/zenodo.23473886">Dissertation (DOI)</a>
</p>
<p align="center">
  <a href="https://doi.org/10.5281/zenodo.23473886"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.23473886.svg" alt="DOI"></a>
  <img src="https://img.shields.io/badge/Open%20to-ML%20%26%20AI%20engineer%20roles-1E4FD6?style=flat-square" alt="Open to ML and AI engineer roles">
  <img src="https://img.shields.io/badge/Based%20in-London%2C%20UK-0E1A2B?style=flat-square" alt="London, UK">
</p>

---

## What I'm working on now

| | |
|---|---|
| **AI/ML placement, Mobex UK** | Developing the retrieval layer of an AI voice agent for inbound business calls, in a team of four students led by Dr Amin Karami. |
| **[doc-compare](https://github.com/Robinson7070/doc-compare)** | An open project that checks a purchase order, an invoice and a delivery note against each other and quotes the exact lines that disagree. Built test-first, with a hold-out set I have not looked at yet. |

## Selected work

### Agentic RAG for supply chain document checking (MSc dissertation)
[Code](https://github.com/Robinson7070/agentic-rag-supply-chain-dissertation) · [DOI 10.5281/zenodo.23473886](https://doi.org/10.5281/zenodo.23473886)

A system that compares purchase orders, invoices and delivery notes and flags mismatches. A deterministic pipeline produces every scored result, so runs are reproducible. A LangChain ReAct agent sits on top for interactive questions.

```mermaid
flowchart LR
    A[PO · Invoice · Delivery note] --> B[Structure-aware chunking]
    B --> C[FAISS index<br/>dense + exact-match]
    C --> D[Regex extraction]
    D --> E[Rule comparison]
    E --> F[(Scored results, JSON)]
    G[LangChain ReAct agent] -.interactive questions.-> C
```

| What worked | What did not |
|---|---|
| 20 of 20 synthetic sets classified correctly, 0 false positives, 0 false negatives. | Recall fell to **0.57** on a harder 100-set corpus, traced to regex field extraction. |
| Defined a custom **Hop Completeness** metric (0.975) for multi-document reasoning. | A single-hop baseline comparison on 6 cases (6/6 vs 4/6) gave p = 0.50: too few cases to claim a difference. |
| Wilson 95% interval reported for the 20-set result: [0.80, 1.00]. | Cross-set retrieval contamination matched one purchase order to a delivery note from another set. |

### doc-compare (in progress)
[Code](https://github.com/Robinson7070/doc-compare)

Rule-based three-way document checker in Python. Reads PDFs, scans and phone photos (OCR with Tesseract), and **refuses to guess**: if a document's line totals do not add up to its printed subtotal, it reports "needs review" instead of inventing findings.

- 8 of 8 development sets correct, including a scanned set. Two hold-out sets still unseen.
- Known weakness: poor phone photos of screens. The tool flags those for review rather than answering wrongly.

### Malaria cell classification
[Code](https://github.com/Robinson7070/malaria-cell-classification-deep-learning)

Compared a custom CNN, EfficientNetB3 and a Vision Transformer on 27,558 cell images. The CNN reached **96.52% accuracy and 97.68% recall**. Grad-CAM and Attention Rollout show what each model looked at.

### Malaria detection API
[Code](https://github.com/Robinson7070/malaria-detection-api)

A FastAPI service that returns a prediction, a confidence score and a Grad-CAM heatmap for each uploaded image, so a reviewer can see why the model answered as it did.

### Also
- [pdf-rag-chatbot](https://github.com/Robinson7070/pdf-rag-chatbot): ask questions about any PDF using LangChain, OpenAI and FAISS
- [distributed-ml-pyspark](https://github.com/Robinson7070/distributed-ml-pyspark): eight PySpark MLlib exercises across regression, classification, NLP and time series, up to 1M rows

## Tools

<table>
<tr><td><b>Languages and data</b></td><td>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/SQL-4B5563?style=for-the-badge" alt="SQL">
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
</td></tr>
<tr><td><b>Machine learning</b></td><td>
<img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" alt="Scikit-learn">
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow">
<img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white" alt="Keras">
<img src="https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="PySpark">
</td></tr>
<tr><td><b>LLM and retrieval</b></td><td>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain">
<img src="https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge" alt="FAISS">
<img src="https://img.shields.io/badge/OpenAI%20API-412991?style=for-the-badge&logo=openai&logoColor=white" alt="OpenAI API">
<img src="https://img.shields.io/badge/Hugging%20Face-B8860B?style=for-the-badge&logo=huggingface&logoColor=white" alt="Hugging Face">
</td></tr>
<tr><td><b>Vision, OCR and explainability</b></td><td>
<img src="https://img.shields.io/badge/CNNs-4B5563?style=for-the-badge" alt="CNNs">
<img src="https://img.shields.io/badge/Vision%20Transformers-4B5563?style=for-the-badge" alt="Vision Transformers">
<img src="https://img.shields.io/badge/Grad--CAM-4B5563?style=for-the-badge" alt="Grad-CAM">
<img src="https://img.shields.io/badge/Tesseract%20OCR-4B5563?style=for-the-badge" alt="Tesseract OCR">
</td></tr>
<tr><td><b>Engineering</b></td><td>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI">
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
<img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter">
</td></tr>
</table>

## How I work

- I build the test set before the system, and keep a hold-out set I do not tune against.
- I report the weak number next to the strong one.
- I tag the exact version that produced each result.

Open to ML and AI engineer roles in the UK. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/robinson-victor).
