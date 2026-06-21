<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Samiullah&fontSize=64&fontColor=00d4ff&fontAlignY=38&desc=AI%20researcher%20and%20engineer%20%C2%B7%20neuro-symbolic%20AI&descAlignY=60&descColor=a0e9ff&animation=fadeIn"/>

<a href="https://github.com/Abdus-Sami01">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3200&pause=900&color=00D4FF&center=true&vCenter=true&width=820&lines=AI+Engineer+%40+Bluecascade;Neuro-symbolic+AI+researcher;Author+of+HALO+and+AXPEN;Checking+whether+models+are+actually+right" alt="Typing SVG" />
</a>

<br/><br/>

[![GitHub](https://img.shields.io/badge/GitHub-Abdus--Sami01-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Abdus-Sami01)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-samiullah--ai-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/samiullah-ai/)
[![ResearchGate](https://img.shields.io/badge/ResearchGate-HALO-00CCBB?style=for-the-badge&logo=researchgate&logoColor=white)](https://www.researchgate.net/publication/404931584_HALO_Hallucination-Aware_Logic_Oracle_for_Neuro-Symbolic_LLM_Verification)
[![Email](https://img.shields.io/badge/Email-Contact-00d4ff?style=for-the-badge&logo=gmail&logoColor=white)](mailto:muhammadabdulsami7@gmail.com)
[![Kaggle](https://img.shields.io/badge/Kaggle-Profile-20beff?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/muhammadabdulsami)

</div>

---

## About

I'm an AI engineer at **Bluecascade** and an undergrad in AI at Emerson University, Multan (CGPA 3.77/4.0). Most of my work comes back to one question: how do you tell when a model is actually right, not just convincing?

That's led me to pair neural networks with logic solvers (Z3) and reinforcement learning, so a model's output can be checked against rules instead of taken on faith. Two papers came out of it so far — **HALO** and **AXPEN** — both below. On the engineering side I build GenAI and computer-vision systems that ship to real users.

---

## Papers

🧠 **HALO: Hallucination-Aware Logic Oracle for Neuro-Symbolic LLM Verification** — *under review, JMLR 2026*
Pulls the factual claims out of an LLM's answer and checks each one against a Z3 logic solver. It catches a failure mode the usual detectors miss: claims that each look fine but together break a domain rule. Claim extractor hits 95.2% F1. [[preprint]](https://www.researchgate.net/publication/404931584_HALO_Hallucination-Aware_Logic_Oracle_for_Neuro-Symbolic_LLM_Verification)

🛡️ **AXPEN: Formally Constrained Autonomous Penetration Testing via Neuro-Symbolic RL** — *preprint, 2026*
An LLM reads CVE text and writes formal preconditions; Z3 turns those into an action mask over a GraphSAGE RL policy. Trained on a 3-host network, the agent reaches 0.92 attack-success on an 8-host network it never saw, where the unmasked baseline gets almost nothing. Sim-only (NASim), and honest about what didn't work.

---

## Projects

🔎 **[Nexus-Insight](https://github.com/Abdus-Sami01)** — a research agent that fact-checks itself
Breaks a claim into parts, gathers evidence from the web, PDFs, arXiv and PubMed, then runs a proposer and a skeptic against each other to settle contradictions. Local PII scrubbing, Groq/Ollama routing, runs in Docker.
`LangGraph` `FastAPI` `Chain-of-Verification`

🧩 **MuaLLM** — a small language model from scratch
An 8M-parameter model built from the tokenizer up: BPE, masked-language pretraining, a span head for QA. Then I swapped in three attention types (softmax, linear, RWKV) to compare speed vs accuracy. Trained on CPU.
`PyTorch` `RWKV` `Linear attention`

🩻 **Dual-View Chest X-Ray Report Generator** — multi-modal medical AI
A Transformer that takes a frontal + lateral X-ray and writes a structured radiology report (indication, findings, impression). Bilinear cross-view fusion, gated cross-attention, a decoder per section, evaluated with RadGraph-F1.
`TensorFlow` `Bio_ClinicalBERT` `CheXNet` `Grad-CAM`

🤖 **Codesage-AI** — code review in your editor
A VS Code extension that reviews your code with Hugging Face models while you write.
`JavaScript` `VS Code API` `Hugging Face`

---

## Experience

**AI Engineer — Bluecascade** *(Sep 2025 – present)*
- Built **Neonizer** ([neonizer.epiccraftings.com](https://neonizer.epiccraftings.com)): upload one logo, get back a manufacturing mock-up and a full price quote with the cost breakdown. Replaced a manual quoting process.
- Wrote the computer-vision measurement stack behind it (PNG/SVG/CorelDraw input, content-tight cropping, distance-transform tube-width estimation, RANSAC line fitting).
- Built internal BI pipelines that cut roughly 70% off the team's decision time.

**Undergraduate Research Assistant — multi-modal learning** *(2024 – 2025)*
- Worked with a PhD researcher on vision-language models; designed the dual-view report generator above.

**Earlier internships** — DeveloperHub, Cognifyz, CodeAlpha *(2024 – 2025)*
- Applied ML across anomaly detection, medical imaging, NLP, recommendation systems, and YOLO object detection.

---

## Tools I reach for

`Python` `PyTorch` `TensorFlow` `scikit-learn`
`Hugging Face` `LangGraph` `LangChain` `GPT-4o` `Groq` `Ollama` `RAG` `FAISS`
`Z3 SMT` `GraphSAGE / GNNs` `Reinforcement Learning (PPO)`
`OpenCV` `spaCy` `Whisper` `YOLO`
`FastAPI` `Flask` `Docker` `Git` `Redis` `n8n` `Airtable`

---

## Certifications

- **Build Your Own Small Language Model From Scratch** — Google
- **AI Agents & Transformers** — Hugging Face
- **Artificial Intelligence, Deep Learning & Communication** — NAVTTC

---

<div align="center">

<img height="170em" src="https://github-readme-stats.vercel.app/api?username=Abdus-Sami01&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=00d4ff&icon_color=00d4ff&text_color=a0e9ff"/>
<img height="170em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Abdus-Sami01&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00d4ff&text_color=a0e9ff"/>

</div>
