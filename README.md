<div align="center">

# Venkat Adithya

**I build LLM agents and the evals that show whether they work.**
B.Tech AI & Data Science @ Shiv Nadar University · 2027

</div>

---

## Open Source — [OpenHands/software-agent-sdk](https://github.com/OpenHands/software-agent-sdk)

Harness-level bug fixes in the OpenHands agent SDK, each shipped with regression tests.

- **[#4435](https://github.com/OpenHands/software-agent-sdk/pull/4435)** · merged — The context condenser's `max_tokens` wasn't inheriting the LLM's effective max input tokens, silently truncating context on specific launch paths.
- **[#4566](https://github.com/OpenHands/software-agent-sdk/pull/4566)** · merged — The global `load_memory` preference reached only one of three conversation launch paths. Centralized the fix; 5 regression tests.
- **[#4876](https://github.com/OpenHands/software-agent-sdk/pull/4876)** · merged — `load_skills_from_agent_server()` discarded the caller's `AgentContext`. A follow-up bug I found and filed after #4566; 5 regression tests.
- **[#5690](https://github.com/OpenHands/software-agent-sdk/pull/5690)** · in review — Concurrent plugin requests could corrupt `.installed.json`. File lock plus atomic write.

---

## Projects

**[RCA LoRA Scaling Study](https://github.com/vnktadithya/rca-lora-scaling-study)** — does more fine-tuning data help?
Controlled QLoRA ablation on Mistral-7B: training set scaled 20 → 474 examples, with LoRA config, quantization, and prompt format held fixed. Scored by a 3-tier harness I built: JSON validity, embedding similarity, calibrated LLM-as-judge. The first two tiers called it a near-tie. The judge scored the 474-example model lower (2.00 vs 2.21, n = 53 held-out), and manual cross-checks confirmed fabricated technical content in 8 of 9 cases. More data didn't help at fixed adapter capacity.

**[ReAct Agent](https://github.com/vnktadithya/ReAct_Agent)** — a raw-Python ReAct loop on a local `Llama-3.2-1B-Instruct` GGUF via `llama-cpp-python`, CPU-only. No agent framework: hand-rolled action parser, tool dispatcher, step budget, and a circuit breaker that halts on the first repeated `(action, param)` pair anywhere in run history.

**[KV Cache VRAM Calculator](https://github.com/vnktadithya/LLM-inference-math)** — the KV cache formula derived from first principles and verified on a T4 against `Llama-3.2-1B-Instruct`. It matched direct cache-tensor inspection exactly (25.31 MB), while `torch.cuda.max_memory_allocated()` reported 48.10 MB. Covers the GQA trap: using `num_attention_heads` instead of `num_key_value_heads` overestimates the cache 4×.

**[Siamese Bi-Encoder](https://github.com/vnktadithya/siamese-bi-encoder-from-scratch)** — a toy Sentence-BERT setup trained from an empty embedding table. Perfect test AUC across 3 seeds hid a test MSE 750–1,500× the train MSE.

---

<div align="center">

vnktadithya@gmail.com · [LinkedIn](https://www.linkedin.com/in/venkat-adithya-gajjarapu-9310a4314)

</div>
