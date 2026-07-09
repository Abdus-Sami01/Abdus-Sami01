<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Samiullah&fontSize=64&fontColor=00d4ff&fontAlignY=38&desc=I%20build%20AI%20you%20can%20check%2C%20not%20just%20trust&descAlignY=60&descColor=a0e9ff&animation=fadeIn"/>

<a href="https://github.com/Abdus-Sami01">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3200&pause=900&color=00D4FF&center=true&vCenter=true&width=820&lines=AI+Engineer+%40+Bluecascade;Neuro-symbolic+AI+researcher;Author+of+HALO+%28JMLR%29+and+AXPEN;LLMs+%2B+Z3+%2B+reinforcement+learning" alt="Typing SVG" />
</a>

<br/><br/>

[![GitHub](https://img.shields.io/badge/GitHub-Abdus--Sami01-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Abdus-Sami01)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-samiullah--ai-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/samiullah-ai/)
[![ResearchGate](https://img.shields.io/badge/ResearchGate-Papers-00CCBB?style=for-the-badge&logo=researchgate&logoColor=white)](https://www.researchgate.net/publication/404931584_HALO_Hallucination-Aware_Logic_Oracle_for_Neuro-Symbolic_LLM_Verification)
[![Email](https://img.shields.io/badge/Email-Contact-00d4ff?style=for-the-badge&logo=gmail&logoColor=white)](mailto:muhammadabdulsami7@gmail.com)
[![Kaggle](https://img.shields.io/badge/Kaggle-Profile-20beff?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/muhammadabdulsami)

</div>

---

## About

Most machine learning hands you an answer and asks you to trust it. I'm more interested in systems that can **show their work** — where a model's output is checked against formal rules, not just assumed to be right because it sounds right.

I'm an AI engineer at **Bluecascade** and a BS Artificial Intelligence student at Emerson University, Multan (CGPA **3.77/4.0**). My research pairs neural networks with **SMT solvers (Z3)** and **reinforcement learning** so their behavior is verifiable. Two papers so far — **HALO** and **AXPEN** — and on the engineering side I ship GenAI and computer-vision systems that real users actually use.

---

## 🔬 Research

> **HALO — Hallucination-Aware Logic Oracle for Neuro-Symbolic LLM Verification** · *under review, JMLR 2026* · [paper](https://www.researchgate.net/publication/404931584_HALO_Hallucination-Aware_Logic_Oracle_for_Neuro-Symbolic_LLM_Verification)

There's a class of LLM hallucination that fact-checkers can't see: every claim looks individually plausible, but together they violate a domain law (a drug that's 89.7% effective *and* near-zero toxicity — each fine, jointly impossible). HALO extracts the claims, hands them to a **Z3 SMT solver**, and asks whether they're satisfiable against an axiom library. The claim extractor runs at **95.2% F1**, and it flags cases that RAG, SelfCheckGPT, and semantic-entropy methods miss entirely.

`Z3 / SMT` · `LLM verification` · `neuro-symbolic`

<br/>

> **AXPEN — Formally Constrained Autonomous Penetration Testing via Neuro-Symbolic RL** · *preprint, 2026* · [code](https://github.com/Abdus-Sami01/RL_Guided_Pentesting)

<img src="https://raw.githubusercontent.com/Abdus-Sami01/RL_Guided_Pentesting/main/paper/figures/animations/anim8_hero_banner.gif" width="90%" alt="AXPEN — an LLM-built, Z3-verified action mask driving a GraphSAGE PPO policy across an unseen network"/>

RL pentesting agents memorise the network they trained on and fall apart when it changes. AXPEN constrains the policy with logic instead: an **LLM reads CVE text and writes formal preconditions**, **Z3** compiles them into an action mask, and that mask wraps a **GraphSAGE PPO** policy whose weights transfer to any host count. Trained on 3 hosts, it reaches **0.92 zero-shot attack-success** on an unseen 8-host network (+0.907 over the unmasked baseline, *p* < 1e-3). Simulation-only, and it reports its negative results as carefully as its wins.

`GPT-4o → Z3 mask` · `GraphSAGE PPO` · `zero-shot transfer`

---

## 🚀 Featured Projects

### 🔎 [Nexus-Insight](https://github.com/Abdus-Sami01/nexus-insight) — a research agent that fact-checks itself
An 11-node LangGraph pipeline that runs a 4-phase **Chain-of-Verification**: it atomises a claim, gathers evidence across the web, PDFs, arXiv and PubMed, then pits a **Proposer against a Skeptic** to resolve contradictions. Local PII redaction, token budgeting, circuit breakers, and Groq/Ollama routing. Runs in Docker.
`LangGraph` `FastAPI` `RAG` `Groq` `Ollama`

### 🩻 Dual-View Chest X-Ray Report Generator — multi-modal medical AI
A Transformer that reads a **frontal + lateral** X-ray and writes a structured radiology report (indication / findings / impression). The interesting parts:
- **Bilinear cross-view fusion** — outer-product interaction between the two views instead of naive concatenation, so the model weights view importance itself
- **Gated cross-attention** — a learnable per-layer gate that balances self- vs cross-attention
- **Three section-aware decoders** sharing one fused image encoder
- **CheXNet (DenseNet-121)** backbone, **Bio_ClinicalBERT** tokenizer, **Grad-CAM** for visual grounding, scored with **RadGraph-F1** for clinical correctness

`TensorFlow` `Bio_ClinicalBERT` `CheXNet` `Grad-CAM` `RadGraph`

### 🧩 [MuaLLM](https://github.com/Abdus-Sami01/MuaLLM) — a language model from scratch
A ~20M-parameter decoder-only LM built from the tokenizer up, then taught to chat by **distilling a local open-weight teacher** (top-k logit KD from SmolLM2) — no paid APIs, hobbyist compute. Four swappable attention kernels (**softmax, linear, RWKV, Mamba-2**) benchmarked head-to-head on identical everything-else.
`PyTorch` `Knowledge distillation` `RWKV` `Mamba`

### 🤖 [CodeSage AI](https://github.com/Abdus-Sami01/codesage-ai) — AI code review in your editor
A **published VS Code extension** ([Marketplace](https://marketplace.visualstudio.com/items?itemName=SamiullahAtta.codesage-ai)) that streams expert code reviews — security audits, performance tuning, bug checks — inline as you write, powered by DeepSeek.
`TypeScript` `VS Code API` `DeepSeek`

---

## 💼 Experience

**AI Engineer — Bluecascade** · *Sep 2025 – present*
Built **Neonizer** ([live](https://neonizer.epiccraftings.com)): upload one logo → a manufacturing mock-up and a full break-even price quote, automatically. I wrote the CV measurement stack behind it (PNG/SVG/CorelDraw input, content-tight cropping, distance-transform tube-width estimation, RANSAC line fitting) and internal BI pipelines that cut **~70%** off the team's decision time.

**Undergraduate Research Assistant — multi-modal learning** · *2024 – 2025*
Built the dual-view report generator above with a PhD researcher; studied CLIP, ALIGN, BLIP-2, ViLBERT.

**Earlier internships** — DeveloperHub · Cognifyz · CodeAlpha · *2024 – 2025*
Anomaly detection, medical-image classification, NLP, recommendation systems, YOLO object detection — most shipped behind Flask.

---

## 🛠️ Tech

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![HuggingFace](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Z3](https://img.shields.io/badge/Z3%20SMT-6f42c1?style=flat-square)
![LangGraph](https://img.shields.io/badge/LangGraph-FF6B35?style=flat-square)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)

*Also: scikit-learn · GraphSAGE/GNNs · PPO/RL · LangChain · GPT-4o · Groq · Ollama · FAISS · spaCy · Whisper · YOLO · Redis · n8n · Airtable*

</div>

---

## 📜 Certifications

**Build Your Own Small Language Model From Scratch** — Google · **AI Agents & Transformers** — Hugging Face · **AI, Deep Learning & Communication** — NAVTTC

---

<div align="center">

<img height="165em" src="https://github-readme-stats.vercel.app/api?username=Abdus-Sami01&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=00d4ff&icon_color=00d4ff&text_color=a0e9ff"/>
<img height="165em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Abdus-Sami01&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00d4ff&text_color=a0e9ff"/>

<img src="https://streak-stats.demolab.com/?user=Abdus-Sami01&theme=tokyonight&hide_border=true&background=0d1117&ring=00d4ff&fire=00d4ff&currStreakLabel=a0e9ff" alt="streak"/>

<img src="https://github-profile-trophy.vercel.app/?username=Abdus-Sami01&theme=tokyonight&no-frame=true&no-bg=true&margin-w=4&column=7" alt="trophies"/>

<br/><br/>

**📬 Open to** research collaborations in neuro-symbolic AI & LLM verification · AI/ML engineering roles · [reach out](mailto:muhammadabdulsami7@gmail.com)

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=110&section=footer"/>

</div>
