### Building AI infrastructure from first principles, not API wrappers.

Currently: fine-tuning a Mistral-7B classifier (QLoRA) to turn unstructured
infrastructure log telemetry into structured root-cause analysis, evaluated
with a vLLM-accelerated eval harness. → [LINK NEEDED]

Recently merged: a fix to OpenHands' [software-agent-sdk](https://github.com/OpenHands/software-agent-sdk)
resolving a Pydantic `exclude_none` bug that was silently dropping token
limits in the condenser.

Also built from scratch (no frameworks):
- A raw Python ReAct agent loop → [LINK NEEDED]
- Backpropagation, following Karpathy's micrograd → [LINK NEEDED]

**Stack:** Python · PyTorch · PEFT/LoRA · vLLM · FastAPI

[Portfolio](https://my-portfolio-pink-gamma-52.vercel.app/)
