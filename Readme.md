<div align="center">

<!-- Animated Header Banner -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Abdus-Sami&fontSize=60&fontColor=00d4ff&fontAlignY=38&desc=AI%20%7C%20BI%20Engineer%20%7C%20Researcher&descAlignY=60&descColor=a0e9ff&animation=fadeIn"/>

<!-- Typing SVG -->
<a href="https://github.com/Abdus-Sami01">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3000&pause=800&color=00D4FF&center=true&vCenter=true&multiline=false&width=800&lines=AI+%2F+BI+Engineer+%40+Bluecascade;Multi-Modal+Learning+Researcher;LLM+%7C+MLOps+%7C+Deep+Learning;Turning+raw+data+into+intelligent+systems" alt="Typing SVG" />
</a>

<br/><br/>

<!-- Profile Badges -->
[![GitHub](https://img.shields.io/badge/GitHub-Abdus--Sami01-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Abdus-Sami01)
[![Email](https://img.shields.io/badge/Email-Contact%20Me-00d4ff?style=for-the-badge&logo=gmail&logoColor=white)](mailto:muhammadabdulsami7@gmail.com)
[![Kaggle](https://img.shields.io/badge/Kaggle-Profile-20beff?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/muhammadabdulsami)
[![Profile Views](https://komarev.com/ghpvc/?username=Abdus-Sami01&style=for-the-badge&color=00d4ff&label=PROFILE+VIEWS)](https://github.com/Abdus-Sami01)

</div>

---

## 🧠 Who Am I

I'm an **AI/BI Engineer at Bluecascade** and an active researcher in **multi-modal learning**, currently a **4th-semester BS Artificial Intelligence student (CGPA 3.81/4.0)** at Emerson University, Multan. I build systems that don't just predict — they reason, explain, and generalize.

My work spans the full AI lifecycle: from novel architecture design and model training to MLOps pipelines, BI dashboards, workflow automation, and production deployment. I've contributed to **PhD-level multi-modal AI research** integrating vision, language, and audio — and I'm currently pursuing work on **conflict-aware continual multi-modal learning for medical AI**.

> *"The best model is not the one with the most parameters — it's the one that generalizes to the real world."*

---

## 💼 Professional Experience

### 🔵 AI / BI Engineer — Bluecascade *(Current)*
> Full-time | Real-world production systems

- Architecting and deploying end-to-end AI and Business Intelligence solutions for clients
- **Automated an intra-departmental decision-making pipeline** using **n8n + Airtable + JavaScript**, slashing decision turnaround time from ~60 seconds to under 20 seconds — a **>65% latency reduction** in a live production environment
- Building BI dashboards and data flows that surface actionable intelligence from raw operational data
- Managing ML model deployment with MLOps practices including CI/CD integration and containerization

---

### 🔬 Assistant Researcher — PhD Multi-Modal Learning Project *(Supervised Research)*
> Independent | Advanced AI Research

- Contributed to a PhD-level research project focused on **multi-modal learning** combining vision and NLP
- **Designed and implemented a novel Transformer-based architecture** for dual-image medical report generation featuring:
  - **Bilinear Cross-View Fusion** — outer-product feature interaction between two image views for automatic importance weighting, replacing naive concatenation
  - **Gated Cross-Attention Decoder** — a learnable scalar gate (`σ(w)`) per decoder layer that dynamically balances self-attention vs. cross-attention contributions, allowing the model to learn how much to attend to image features vs. prior generated tokens
  - **Three independent Transformer decoders** (indication / findings / impression) sharing a single fused image encoder — enabling section-aware, clinically structured report generation
  - **Dual decoding strategies** — greedy decoding for speed and beam search (configurable beam size) for quality, evaluated against BLEU, METEOR, ROUGE-1/L, CIDEr, and **RadGraph-F1** (clinical correctness metric)
- Integrated **CheXNet (DenseNet121)** pretrained on chest X-rays as the vision backbone with support for ImageNet weights, custom CheXNet weights, and fine-tuning modes
- Implemented **Grad-CAM explainability** for visual grounding of model attention on X-ray images
- Used **Bio\_ClinicalBERT** tokenizer for clinical text tokenization, with masked loss and masked accuracy to handle variable-length padded sequences correctly

---

### 🟠 AI/ML Intern — DeveloperHub Corporation *(Dec 2024 – Feb 2025)*
- Built ML/DL pipelines on real-world datasets covering financial anomaly detection, medical image cancer classification, and NLP-based text classification
- Deployed models via **Flask** REST APIs and optimized data preprocessing pipelines for production throughput
- Worked on **stock market anomaly detection** using time-series modeling

---

### 🟡 Machine Learning Intern — Cognifyz Technologies *(Jan 2025 – Mar 2025)*
- Built and deployed ML models for real-time restaurant data analysis
- Improved accuracy of **recommendation systems** using regression and classification algorithms with feature engineering on structured tabular data

---

### 🟢 Computer Vision & NLP Intern — CodeAlpha *(Feb 2025 – Apr 2025)*
- Developed a **QA chatbot** and **language translation models** using NLP pipelines
- Created a **prompt-to-music generation tool** leveraging generative AI
- Implemented real-time **object detection** using **YOLO** architecture

---

## 🔭 Current Research

### 🧬 Conflict-Aware Continual Multi-Modal Learning for Medical AI *(In Progress)*
Investigating how multi-modal AI models (vision + language) can learn sequentially from new medical data **without catastrophically forgetting** prior knowledge — with a specific focus on **conflict detection** between modalities during continual learning. This targets a core open problem in clinical AI: how to keep models up-to-date in dynamic hospital environments without full retraining.

---

## 🚀 Featured Projects

### 🩻 Dual-View Chest X-Ray Report Generator
> *Multi-Modal Deep Learning | Medical AI | NLP*

A full Transformer-based system that takes **two X-ray views** (frontal + lateral) and generates structured radiology reports (indication, findings, impression) with clinical correctness evaluation.

**Architectural novelties:**
- Bilinear cross-view image fusion (outer-product interaction)
- Gated cross-attention with per-layer learnable α gate
- Triple-decoder architecture for section-aware generation
- Evaluated with RadGraph-F1 for entity-relation clinical accuracy

`TensorFlow` `Bio_ClinicalBERT` `CheXNet` `Grad-CAM` `Beam Search` `RadGraph`

---

### 🤖 Codesage-AI — AI-Powered Code Reviewer Extension
> *VSCode Extension | NLP | Developer Tools*

A VSCode extension that reviews code in real-time using Hugging Face models for linting suggestions and optimization hints — bringing AI pair-programming directly into the editor.

`JavaScript` `Python` `VS Code API` `Hugging Face` `NLP`

---

### 📐 AI Math Tutor App
> *Flask Web App | NLP | Education AI*

An interactive web application that solves and explains math problems from basic arithmetic to advanced calculus, and a chatbot interface.

`Flask` `HTML` `Data Visualization` `NLP` `Transfer Learning`

---

## 🛠️ Tech Stack

<div align="center">

### Languages & Core
![Python](https://img.shields.io/badge/Python-Expert-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Novice-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Intermediate-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

### AI / ML / DL
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

### LLMs & NLP
![Transformers](https://img.shields.io/badge/Transformers-LLM%20%7C%20BERT%20%7C%20GPT-yellow?style=flat-square)
![BioClinicalBERT](https://img.shields.io/badge/Bio_ClinicalBERT-Medical%20NLP-red?style=flat-square)
![CheXNet](https://img.shields.io/badge/CheXNet-Medical%20Vision-blueviolet?style=flat-square)

### MLOps & Deployment
![Docker](https://img.shields.io/badge/Docker-Learning-2496ED?style=flat-square&logo=docker&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-2088FF?style=flat-square&logo=github-actions&logoColor=white)

### Automation & BI
![n8n](https://img.shields.io/badge/n8n-Workflow%20Automation-EA4B71?style=flat-square&logo=n8n&logoColor=white)
![Airtable](https://img.shields.io/badge/Airtable-18BFFF?style=flat-square&logo=airtable&logoColor=white)

### Tools & Platforms
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=flat-square&logo=kaggle&logoColor=white)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=white)
![VSCode](https://img.shields.io/badge/VSCode-007ACC?style=flat-square&logo=visual-studio-code&logoColor=white)

</div>

---

## 📊 GitHub Stats

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=Abdus-Sami01&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=00d4ff&icon_color=00d4ff&text_color=a0e9ff"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Abdus-Sami01&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00d4ff&text_color=a0e9ff"/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Abdus-Sami01&theme=tokyonight&hide_border=true&background=0d1117&ring=00d4ff&fire=00d4ff&currStreakLabel=a0e9ff" alt="GitHub Streak"/>

</div>

---

## 🏅 Certifications

| Certification | Issuer |
|---|---|
| Artificial Intelligence, Deep Learning & Communication | NAVTTC |
| AI Agents & Transformers | Hugging Face |

---

## 📈 What I'm Working On

- 🔬 **Conflict-Aware Continual Multi-Modal Learning** — medical AI research (active)
- 🚀 Releasing new **open-source projects** on GitHub soon
- 📦 Deepening **MLOps** practices — model versioning, monitoring, and deployment pipelines
- 🧩 Exploring **agentic AI** systems using LLMs with tool-use and memory

---

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=120&section=footer&animation=fadeIn"/>

**"Building AI that understands the world — one modality at a time."**

⭐ *If you find my work interesting, consider starring a repo — it means a lot!*

</div>
