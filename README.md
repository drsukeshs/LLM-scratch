# LLM-scratch
Small-Scale Transformer LLM from Scratch with Generative Text Capabilities and Wikipedia-Style Output Demonstrations

### Overview

This project implements a GPT-style transformer from scratch (approx. 165M parameters) following Sebastian Raschka’s approach.
It is trained lightly (~2.5 epochs) on the Wikitext-103M dataset. The goal is to demonstrate:

  + Building a transformer model from scratch

  + Training a generative language model

  + Generating text that preserves basic grammar, sometimes holds context, and exhibits mild hallucinations

!!Note: This model is not fully trained, outputs are for demonstration and educational purposes only.

### Features

  + 24-layer transformer, 512-dim embeddings, 8 attention heads

  + Trained on ~2.5 epochs of Wikitext-103M (~100M tokens): paused pretraining as loss plateau observed at 1.9-1.93

  + Generates text in Wikipedia-like style, with mild hallucinations

  + Examples include topics like "United States", "The United States is a country", "Cars need newer", "Artificial intelligence"

  + Outputs show context drift, punctuation quirks, and nonsense elements — typical for lightly trained GPT

### Limitations

  + The model is lightly trained (~2.5 epochs) on Wikitext-103M, so context retention is very limited.

  + Outputs often veer off-topic and contain hallucinations or nonsensical phrases.

  + Grammar is mostly preserved, but punctuation is sometimes misused due to partial training.

  + The model is small-scale (24 layers, 512-dim) and cannot compete with modern large LLMs in fluency or reasoning.

  + Not designed for production; for educational and demonstration purposes only.

### Future Work

  + Increase training epochs or dataset size to improve context retention and coherence.

  + Implement fine-tuning on domain-specific text (e.g., medical, legal, or scientific corpora).

  + Integrate multimodal inputs such as images or structured data for richer generative capabilities.

  + Explore QLoRA or LoRA techniques to reduce memory footprint while fine-tuning.

  + Add quantitative metrics (perplexity, BLEU scores) and visualizations of training curves.

  + Experiment with prompt engineering and controlled generation to reduce hallucinations.
