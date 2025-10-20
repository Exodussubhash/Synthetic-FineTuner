# 🧠 Synthetic Fine-Tuner (QLoRA on Mistral-7B)

This mini-project demonstrates LoRA/QLoRA fine-tuning of **Mistral-7B-Instruct** on a Q&A dataset about *Transfer Learning & Transformers*.
It’s built as a portfolio project showing real-world LLM fine-tuning, evaluation, and efficient GPU usage.

---

### 🔍 Overview
- **Model**: mistralai/Mistral-7B-Instruct-v0.3  
- **Technique**: QLoRA (4-bit quantization + LoRA adapters)  
- **Dataset**: 200 questions about Transformers (from `transformers_200Qs_v11.pdf`)
- **Metrics**: Training loss, Eval loss, BLEU, Semantic Similarity (SBERT)
- **Tools**: Hugging Face Transformers, PEFT, bitsandbytes, Accelerate, W&B

---

### 🧩 Pipeline
1. **Data Extraction** → parse PDF into clean JSONL 
2. **QLoRA Fine-tuning**
3. **Evaluation** → (BLEU + cosine similarity)
4. **Results**
   - Train loss ↓ from 2.58 → 0.29  
   - Eval loss ≈ 2.08 → Perplexity ≈ 8.0  
   - Semantic similarity ≈ 0.86 average

---
