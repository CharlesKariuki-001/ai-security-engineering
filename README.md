# 🛡️ AI Security Red Team Architect Lab

**12-Month Self-Study Program** — From Tensor Fundamentals to Professional AI Red/Blue Teaming  
**Charles Kariuki (Charles Mburu)** — Nairobi, Kenya | Started: June 2026

[![GitHub](https://img.shields.io/badge/GitHub-Profile-black?style=flat&logo=github)](https://github.com/CharlesKariuki-001)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://linkedin.com/in/charles-mburu)
[![X](https://img.shields.io/badge/X-@KariukiBuilds__-black?style=flat&logo=x)](https://x.com/KariukiBuilds__)

---

### 🎯 Mission
I am deliberately building **production-grade AI Security Engineering skills** using only free tools (Colab, Kaggle, Docker, GitHub).  

This lab runs **in parallel** with **[Vigilant AI](https://github.com/CharlesKariuki-001/VigilantAI)** — my practical fraud detection system for M-Pesa and East African mobile money. Every attack I learn makes Vigilant AI more robust. Every real-world fraud problem I solve deepens my red team skills.

**Goal by Month 12:** Have a portfolio that stands out globally — four major capstone projects (AdversarialForge, PipelineKiller, IronPipeline, ForgeDefender) + real product experience.

---

### 📍 Current Status (June 2026)
**Month 1 of 12 — Block 1: Foundations (Tensor Attacks & Low-Level AI)**

**Progress:**
- ✅ Week 1: Tensor basics, manual matrix multiplication, gradients & autograd
- 🔄 Week 2–4: Training loops, FGSM attack, data poisoning (in progress)
- ✅ Repo structure + professional documentation habit established
- ✅ Daily commits + public accountability

**Next Milestone:** Complete **AdversarialForge** (end-to-end training → poisoning → FGSM/PGD attacks → vLLM serving) by end of Month 3.

---

### 🗺️ 12-Month Roadmap

| Block | Months | Focus | Milestone Project | Status |
|-------|--------|-------|-------------------|--------|
| **1** | 1–3 | Tensor ops, training loops, adversarial attacks (FGSM, PGD), data poisoning, Safetensors, Docker | **AdversarialForge** | In Progress |
| **2** | 4–6 | Prompt injection, agent hijacking, RAG attacks, model extraction, PyRIT/Garak | **PipelineKiller** | Planned |
| **3** | 7–9 | Input/output guards, adversarial training, Llama Guard, NeMo Guardrails, monitoring | **IronPipeline** | Planned |
| **4** | 10–12 | Continuous red/blue loops, GitOps, OWASP LLM Top 10, compliance (NIST, CBK) | **ForgeDefender** | Planned |

**Full weekly breakdown** available in the [Master Build Document](https://github.com/CharlesKariuki-001/AI-Security-Red-Team-Lab/blob/main/docs/AI_Security_Pipeline_Master.md) (uploaded as reference).

---

### 🏗️ Repository Structure

```text
├── Block1-AdversarialForge/     # Current work (Weeks 1-12)
│   ├── week1/                   # Tensors, gradients, matrix mult
│   ├── week2/                   # Training loops & autograd
│   ├── week3/                   # FGSM + attack reports
│   └── ...
├── docs/                        # Architecture diagrams, reports, CV assets
├── notes/                       # Plain-English explanations & cheat sheets
├── scripts/                     # Colab launchers, Docker configs
├── requirements.txt
└── README.md
