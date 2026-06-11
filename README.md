# 🛡️ AI Pipeline Red Team Architect Lab

CS graduate from Kenya building practical skills in AI security. This repo tracks my 12-month self-study using only free tools (Colab, Kaggle, Hugging Face free tier, local Docker).

---

## Goal
Develop specialized skills in attacking and defending AI pipelines (offensive red teaming + production hardening) to reach high-value remote opportunities.

---

## 12-Month Roadmap

### Block 1: Foundations – Tensor Attacks & Low-Level AI (Months 1–3)
**Focus:** Tensors, gradients, model internals.

- [ ] Linear algebra, embeddings, attention, autograd
- [ ] PyTorch operations and basic adversarial attacks (FGSM/PGD)
- [ ] Safetensors, model formats, Docker setup
- [ ] Free GPU usage (Colab/Kaggle)

**Milestone:** AdversarialForge  
End-to-end training-to-inference pipeline with poisoning injection, attacks, and vLLM serving. Tested on free tiers.

### Block 2: Offensive Red Teaming (Months 4–6)
**Focus:** Breaking AI systems.

- [ ] Prompt injections, agent hijacks, multi-turn attacks
- [ ] Model extraction, data leakage, supply-chain exploits
- [ ] PyRIT, Garak, LangChain

**Milestone:** PipelineKiller  
RAG/agent system with automated attack scripts and success metrics.

### Block 3: Defensive Hardening (Months 7–9)
**Focus:** Building resilient systems.

- [ ] Runtime detection, adversarial training
- [ ] Guards, model signing, monitoring
- [ ] Llama Guard, NeMo Guardrails, Prometheus

**Milestone:** IronPipeline  
Hardened version of Block 2 system with layered defenses and attack comparison.

### Block 4: Integrated Platform (Months 10–12)
**Focus:** Full red/blue automation.

- [ ] Continuous attack-defense loops
- [ ] GitOps, observability, compliance

**Milestone:** ForgeDefender  
Complete system that tests, fixes, and deploys AI pipelines securely.

---

## Repository Structure
```text
├── Block1-AdversarialForge/
├── Block2-PipelineKiller/
├── Block3-IronPipeline/
├── Block4-ForgeDefender/
├── docs/          # Diagrams and reports
├── notes/         # Cheat sheets
└── scripts/       # Free-tier setup
