# 🚀 Modern AI with Unsloth.ai

This repository contains a complete, multi-notebook series demonstrating **modern fine-tuning and reinforcement learning techniques** using **Unsloth.ai** across diverse use cases.
Each use case includes: a runnable Colab notebook, dataset notes, clear inputs/outputs, and a **YouTube video walkthrough** showing the code tour, training run, and inference demo.

---

## 🎯 Goals

1. Show end-to-end workflows in Unsloth.ai for:
   • Full fine-tuning of small LLMs
   • Parameter-efficient fine-tuning (LoRA)
   • Preference-based Reinforcement Learning (RL) with chosen datasets
   • GRPO-style reasoning RL with model-generated answers
   • Continued pretraining to extend model knowledge (e.g., new language)

2. Provide reproducible notebooks and structured artifacts suitable for grading and future reuse.

---

## 📚 References & Hints

• Unsloth Notebooks Hub (Kaggle/Colab):
[https://github.com/unslothai/notebooks](https://github.com/unslothai/notebooks)

• Unsloth Finetuning Guide:
[https://docs.unsloth.ai/get-started/fine-tuning-llms-guide](https://docs.unsloth.ai/get-started/fine-tuning-llms-guide)

• Reinforcement Learning Guide:
[https://docs.unsloth.ai/get-started/reinforcement-learning-rl-guide](https://docs.unsloth.ai/get-started/reinforcement-learning-rl-guide)

• GRPO Reasoning Tutorial:
[https://docs.unsloth.ai/get-started/reinforcement-learning-rl-guide/tutorial-train-your-own-reasoning-model-with-grpo](https://docs.unsloth.ai/get-started/reinforcement-learning-rl-guide/tutorial-train-your-own-reasoning-model-with-grpo)

• Unsloth R1 Reasoning Blog:
[https://unsloth.ai/blog/r1-reasoning](https://unsloth.ai/blog/r1-reasoning)

• Continued Pretraining:
[https://docs.unsloth.ai/basics/continued-pretraining](https://docs.unsloth.ai/basics/continued-pretraining)

• Export to Ollama:
[https://docs.unsloth.ai/tutorials/how-to-finetune-llama-3-and-export-to-ollama](https://docs.unsloth.ai/tutorials/how-to-finetune-llama-3-and-export-to-ollama)

• Example Kaggle notebook:
[https://www.kaggle.com/code/kingabzpro/fine-tuning-llms-using-unsloth](https://www.kaggle.com/code/kingabzpro/fine-tuning-llms-using-unsloth)

• LoRA with Ollama (templates):
[https://sarinsuriyakoon.medium.com/unsloth-lora-with-ollama-lightweight-solution-to-full-cycle-llm-development-edadb6d9e0f0](https://sarinsuriyakoon.medium.com/unsloth-lora-with-ollama-lightweight-solution-to-full-cycle-llm-development-edadb6d9e0f0)

---

## 🧪 Use Cases (Colabs)

a) Colab 1 — Full Finetuning (Small Model)
• Model: smolLM2 135M (or unsloth/gemma-3-1b-it-unsloth-bnb-4bit) with full_finetuning enabled
• Task: choose coding or chat; demonstrate compatible chat templates
• Deliverables: training run, evaluation samples, inference examples, YouTube walkthrough

b) Colab 2 — LoRA Parameter-Efficient Finetuning
• Same dataset and task as Colab 1, but convert to LoRA
• Compare runtime, GPU memory, and output quality vs. full FT
• Deliverables: hyperparameter notes, side-by-side sample outputs, YouTube walkthrough

c) Colab 3 — Reinforcement Learning with Preferences
• Dataset contains input, preferred output, rejected output (pairwise or listwise)
• Show reward signal design and training stability heuristics
• Deliverables: training curves, preference accuracy snapshots, qualitative comparisons, YouTube walkthrough

d) Colab 4 — GRPO Reasoning RL
• Use problem-only datasets; model generates answers; optimize via GRPO
• Highlight reasoning traces, token budget, and stop sequences
• Deliverables: sample problems, rationales, reward trajectory, YouTube walkthrough

e) Colab 5 — Continued Pretraining (New Language)
• Extend base model’s vocabulary/knowledge on a curated corpus for a new language or domain
• Show tokenizer/encoding considerations and eval prompts pre/post CPT
• Deliverables: corpus sourcing and cleaning notes, perplexity or proxy metrics, qualitative outputs, YouTube walkthrough

Optional Enhancements (documented in extras/):
• Continue fine-tuning from a custom checkpoint
• Mental-health chatbot case study with Phi-3 (ethical guardrails, safe-completion prompts)
• Export finetuned model to Ollama and demonstrate local inference

---

## 🧰 Models You May Reference (Open Weights)

Choose at least the small model for Colab 1 and reuse across others when appropriate:

• smolLM2 135M

• unsloth/gemma-3-1b-it-unsloth-bnb-4bit

• Llama 3.1 (8B), Llama 3 (8B)

• Mistral v0.3 (7B), Mistral NeMo (12B)

• Gemma 2 (2B, 9B)

• Phi-3 / Phi-3.5 (mini/medium)

• Qwen2 (7B)

• TinyLlama

**Note:** For grading and reproducibility, prioritize smaller models for full FT; use larger models for LoRA or RL when feasible.

---

## 🧾 Datasets & Formatting

• Clearly document the dataset source and license in each folder’s dataset_notes.md.

• For chat/coding tasks, include the prompt/response schema and any chat template used.

• For RL with preferences, store each sample with input, preferred, rejected output, and any metadata (source, difficulty).

• For GRPO, list problem statements, acceptance criteria, and reward function.

• For continued pretraining, describe corpus cleaning, deduplication, and tokenization notes.

---

## ✅ Deliverables Checklist

For each Colab folder:

• A Colab notebook that completes successfully end-to-end

• Short README (dataset_notes.md or corpus_prep.md) describing inputs, schema, and evaluation

• At least three qualitative examples of before/after behavior

• Training artifacts: logs, charts, or screenshots in results/

• A YouTube video walkthrough link in video/ with:
– Problem statement and dataset explanation
– Code tour line-by-line for important cells
– Live training run or loaded logs with commentary
– Inference demos showing inputs and outputs
– Summary of lessons learned and limitations

---

## 🔬 Evaluation & Reporting

**Quality**
• Human-readable examples with success/failure notes
• Optional automatic metrics (e.g., exact match on reasoning tasks, BLEU/ROUGE for text, preference accuracy for RL)

**Efficiency**
• GPU type and runtime
• Batch sizes, sequence lengths, LoRA ranks
• Memory observations and stability tips

**Comparisons**
• Full FT vs. LoRA: cost, speed, output quality
• SFT vs. RL vs. GRPO outcomes on the same prompts

---

## 🛠 Environment & Dependencies

• Google Colab (T4/A100/L4 where available)

• Unsloth.ai libraries and their documented dependencies

• Optional: Kaggle integration for datasets or running Kaggle notebooks

• Note any special accelerator/runtime selection in the top of each notebook

---

## 🔄 Reproducibility Notes

• Fix random seeds where possible; log package versions

• Save and reference checkpoints and tokenizer versions

• Document any cloud storage used for artifacts

• When exporting to Ollama, record the exact export command, model name, and inference settings in extras/export_to_ollama_notes.md

---

## 🔒 Ethics & Safety

• If you build sensitive assistants (e.g., mental-health), include clear disclaimers and safe-completion prompts

• Filter or anonymize personal data in training corpora

• Respect dataset licenses and cite all sources
