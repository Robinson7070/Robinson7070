<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0E1A2B,100:1E4FD6&height=210&section=header&text=Victor%20Robinson&fontSize=54&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=ML%20%26%20AI%20Engineer%20%C2%B7%20London&descSize=20&descAlignY=60" alt="Victor Robinson, ML and AI Engineer, London" width="100%">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3200&pause=1100&color=1E4FD6&center=true&vCenter=true&width=760&height=40&lines=ML+and+AI+engineer+in+London;I+build+systems+that+show+their+working;20%2F20+on+the+test+sets.+0.57+on+the+hard+ones.+Both+reported.;Now+building+a+voice+agent+and+doc-compare" alt="ML and AI engineer in London. I build systems that show their working.">

<br>

<a href="PORTFOLIO_LINK"><img src="https://img.shields.io/badge/Portfolio-0E1A2B?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
<a href="https://www.linkedin.com/in/robinson-victor"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="https://doi.org/10.5281/zenodo.23473886"><img src="https://img.shields.io/badge/Dissertation%20DOI-1E4FD6?style=for-the-badge&logo=zenodo&logoColor=white" alt="Dissertation DOI"></a>

<img src="https://img.shields.io/badge/Open%20to-ML%20%26%20AI%20engineer%20roles-1E4FD6?style=flat-square" alt="Open to ML and AI engineer roles">

</div>

<br>

<table align="center">
<tr>
<td align="center" width="25%"><h2>20 / 20</h2>synthetic sets classified correctly</td>
<td align="center" width="25%"><h2>0.57</h2>recall on the harder 100 sets</td>
<td align="center" width="25%"><h2>96.52%</h2>malaria cell classifier accuracy</td>
<td align="center" width="25%"><h2>8 / 8</h2>doc-compare dev sets, scans included</td>
</tr>
</table>

## About me

I am an MSc AI and Data Science student at the University of East London. I come from Nigeria, trained as an electrical and electronic engineer, worked in IT, then moved into machine learning. Engineering taught me to ask how a thing fails before I trust it, and I bring that to every model I build.

What I care about is systems that can be checked: a test set built before the system, a hold-out I do not tune against, and the weak number reported next to the strong one. Long term I want to build products that businesses use and pay for.

Outside work I play football and write technical articles on Medium.

```text
whoami      Victor Chukwudi Robinson
location    London, UK (from Nigeria)
studying    MSc AI and Data Science, UEL, finishing May 2027
building    retrieval layer for a voice agent (Mobex UK), doc-compare
learning    evaluating RAG systems, reading text from messy documents
ask me      explainable models, document checking, honest evaluation
```

## My path

```mermaid
flowchart LR
    A["BEng Electrical and<br/>Electronic Engineering<br/>Nigeria, 2017-2022"] --> B["IT Officer<br/>Petronella Nigeria<br/>2023-2024"]
    B --> C["ML training<br/>ALX, 3MTT, Wedigraf<br/>2023-2025"]
    C --> D["MSc AI and Data Science<br/>University of East London<br/>2025-2027"]
    D --> E["Placement<br/>Mobex UK voice agent<br/>2026"]
    style A fill:#0E1A2B,color:#fff,stroke:#0E1A2B
    style B fill:#16335F,color:#fff,stroke:#16335F
    style C fill:#1B4390,color:#fff,stroke:#1B4390
    style D fill:#1E4FD6,color:#fff,stroke:#1E4FD6
    style E fill:#3B6DF0,color:#fff,stroke:#3B6DF0
```

## Currently

- **AI/ML placement at Mobex UK:** building the retrieval layer of an AI voice agent, in a team of four students.
- **[doc-compare](https://github.com/Robinson7070/doc-compare):** checks a purchase order, an invoice and a delivery note against each other, from PDFs, scans and photos.

## Projects

<table>
<tr>
<td width="50%" valign="top">
<h3>Agentic RAG for supply chain documents</h3>
MSc dissertation. Flags mismatches across purchase orders, invoices and delivery notes. A deterministic pipeline gives reproducible scores, and an agent answers questions on top.<br><br>
<b>Result:</b> 20/20 sets correct. <b>Limit:</b> recall 0.57 on 100 sets.<br><br>
<a href="https://github.com/Robinson7070/agentic-rag-supply-chain-dissertation">Code</a> · <a href="https://doi.org/10.5281/zenodo.23473886">DOI</a>
</td>
<td width="50%" valign="top">
<h3>doc-compare</h3>
Rule-based three-way document checker. Quotes the exact lines that disagree. If a read looks unreliable it says "needs review" instead of guessing.<br><br>
<b>Result:</b> 8/8 development sets. <b>Limit:</b> weak on poor phone photos; hold-out not run yet.<br><br>
<a href="https://github.com/Robinson7070/doc-compare">Code</a>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<h3>Malaria cell classification</h3>
Custom CNN vs EfficientNetB3 vs Vision Transformer on 27,558 images, with Grad-CAM and Attention Rollout.<br><br>
<b>Result:</b> CNN 96.52% accuracy, 97.68% recall.<br><br>
<a href="https://github.com/Robinson7070/malaria-cell-classification-deep-learning">Code</a>
</td>
<td width="50%" valign="top">
<h3>Malaria detection API</h3>
FastAPI service that returns a prediction, a confidence score and a Grad-CAM heatmap for each image.<br><br>
<b>Result:</b> an explainable model behind a working REST endpoint.<br><br>
<a href="https://github.com/Robinson7070/malaria-detection-api">Code</a>
</td>
</tr>
</table>

More: [pdf-rag-chatbot](https://github.com/Robinson7070/pdf-rag-chatbot) (ask questions about any PDF) · [distributed-ml-pyspark](https://github.com/Robinson7070/distributed-ml-pyspark) (8 algorithms, up to 1M rows)

## Skills

**Languages and data**<br>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"> <img src="https://img.shields.io/badge/SQL-4B5563?style=flat-square" alt="SQL"> <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="Pandas"> <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" alt="NumPy">

**Machine learning**<br>
<img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="Scikit-learn"> <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" alt="TensorFlow"> <img src="https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white" alt="Keras"> <img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="PySpark">

**LLM and retrieval**<br>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain"> <img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square" alt="FAISS"> <img src="https://img.shields.io/badge/OpenAI%20API-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI API"> <img src="https://img.shields.io/badge/Hugging%20Face-B8860B?style=flat-square&logo=huggingface&logoColor=white" alt="Hugging Face">

**Vision and OCR**<br>
<img src="https://img.shields.io/badge/CNNs-4B5563?style=flat-square" alt="CNNs"> <img src="https://img.shields.io/badge/Vision%20Transformers-4B5563?style=flat-square" alt="Vision Transformers"> <img src="https://img.shields.io/badge/Grad--CAM-4B5563?style=flat-square" alt="Grad-CAM"> <img src="https://img.shields.io/badge/Tesseract%20OCR-4B5563?style=flat-square" alt="Tesseract OCR">

**Engineering**<br>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"> <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git"> <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white" alt="Jupyter">

## Say hello

Open to ML and AI engineer roles in the UK. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/robinson-victor).

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1E4FD6,100:0E1A2B&height=110&section=footer" alt="" width="100%">
