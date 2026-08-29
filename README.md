<div align="center">

# Venkat Adithya

**AI Engineer building LLMs, RAG systems, and agentic infrastructure from scratch.**
B.Tech AI & Data Science @ Shiv Nadar University · 2027

</div>

---

##  Currently Building

Fine-tuning a **Mistral-7B classifier (QLoRA)** to turn unstructured infrastructure log
telemetry into structured root-cause analysis. Scaling a hand-curated dataset to 500
examples with a 10% holdout, evaluated against a dedicated harness.

→ [Phase_2/LoRA](https://github.com/vnktadithya/Learning-Log/tree/main/Phase_2/LoRA)

---

## Built From Scratch — No Frameworks

Every project below is raw Python. No LangChain, no LlamaIndex, no third-party agent
framework, no API integrations.

**[ReAct Agent](https://github.com/vnktadithya/ReAct_Agent)**
A ReAct (Reason → Act → Observe) loop running a local `Llama-3.2-1B-Instruct` GGUF model
via `llama-cpp-python`, CPU-only. Hand-rolled action parser, tool dispatcher, and a
circuit breaker that halts on *any* repeated `(action, param)` pair anywhere in run
history — not just the immediately preceding step.

**[KV Cache VRAM Calculator](https://github.com/vnktadithya/LLM-inference-math)**
Derived the KV cache memory formula from first principles, then verified it empirically
against `Llama-3.2-1B-Instruct` on a Colab T4 — including the Grouped Query Attention
trap: using `num_attention_heads` instead of `num_key_value_heads` overestimates cache
size by exactly the GQA ratio (4x for this model).

**[Micrograd](https://github.com/vnktadithya/Learning-Log/tree/main/Phase_1/Micrograd)**
Karpathy-style scalar autograd engine, implemented line by line: a `Value` class with
`__add__`, `__mul__`, `tanh`, and a manual backward pass verified against finite-difference
gradient checks.

---

## Open Source

**[OpenHands/software-agent-sdk #4435](https://github.com/OpenHands/software-agent-sdk/pull/4435)** — *merged*
Fixed a bug where the condenser's `max_tokens` wasn't inheriting the LLM's effective max
input tokens, silently truncating context on specific launch paths. Merged by a core
maintainer.

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

**ML / Fine-Tuning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![PEFT/LoRA](https://img.shields.io/badge/PEFT%20%2F%20LoRA-6A0DAD?style=for-the-badge)
![QLoRA](https://img.shields.io/badge/QLoRA-4B0082?style=for-the-badge)

**Local Inference**

![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![llama.cpp](https://img.shields.io/badge/llama.cpp-black?style=for-the-badge)
![GGUF](https://img.shields.io/badge/GGUF%20Q4__K__M-333333?style=for-the-badge)

**Tools**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)

---

<div align="center">

### Connect

[GitHub](https://github.com/vnktadithya) · vnktadithya@gmail.com · [LinkedIn](www.linkedin.com/in/venkat-adithya-gajjarapu-9310a4314)

</div>
