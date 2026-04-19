# 🧠 NanoGPT — TinyStories Character-Level Model

A compact, efficient character-level GPT transformer trained on the [TinyStories](https://huggingface.co/datasets/roneneldan/TinyStories) dataset using [Karpathy's nanoGPT](https://github.com/karpathy/nanoGPT). This project demonstrates how to train, export, and deploy a language model on Hugging Face in just **~10 minutes on a free T4 GPU**.

---

## 📋 Overview

This notebook implements a complete pipeline for:
1. **Training** a lightweight transformer on character-level text
2. **Exporting** the model to Hugging Face Hub  
3. **Deploying** an interactive Gradio demo to Hugging Face Spaces

Perfect for learning LLM training workflows or as a starting point for custom language models.

---

## 🚀 Quick Links

| Resource | Link |
|----------|------|
| **Model Repository** | `ncncomplete/nanogpt-tinystories` on Hugging Face Hub |
| **Interactive Demo** | `ncncomplete/nanogpt-tinystories-demo` on Hugging Face Spaces |
| **Training Notebook** | [Open in Colab](https://colab.research.google.com/github/Karna14314/Nanogpt/blob/main/Nanogpt.ipynb) |

---

## 📊 Model Architecture

| Parameter | Value |
|-----------|-------|
| **Total Parameters** | ~1.6M |
| **Layers** | 6 |
| **Attention Heads** | 6 |
| **Embedding Dimension** | 192 |
| **Context Length** | 256 tokens |
| **Vocab Size** | 80 characters |
| **Training Iterations** | 2000 |
| **Data Type** | float16 |
| **Training Time** | ~10 minutes (Colab T4) |

---

## 📦 Installation

### Option 1: Google Colab (Recommended)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Karna14314/Nanogpt/blob/main/Nanogpt.ipynb)

Simply click the button above to run the entire pipeline in your browser—no local setup needed!

### Option 2: Local Installation
```bash
git clone https://github.com/karpathy/nanoGPT.git
cd nanoGPT
pip install -q torch tiktoken requests numpy huggingface_hub transformers gradio
