# LLM From Scratch

A decoder-only Large Language Model implemented from scratch using PyTorch, covering the complete pipeline from text tokenization and dataset preparation to transformer training and text generation.

## 🚀 Overview

This project implements the core components of a modern LLM without relying on pre-built transformer architectures. The goal is to understand and implement how language models process text, learn contextual representations, and generate new text.

### Key Components

- Custom text/token processing and dataset preparation
- Token and positional embeddings
- Multi-Head Self-Attention
- Causal attention masking
- Transformer decoder blocks
- Feed-Forward Neural Networks
- Residual connections and Layer Normalization
- Next-token prediction
- Cross-entropy loss optimization
- Autoregressive text generation
- Model training and evaluation using PyTorch

## 🧠 Architecture

The model follows a decoder-only Transformer architecture:

```text
Input Text
    ↓
Tokenization
    ↓
Token Embeddings
    +
Positional Embeddings
    ↓
Transformer Decoder Blocks
    ├── Multi-Head Self-Attention
    ├── Add & Norm
    ├── Feed-Forward Network
    └── Add & Norm
    ↓
Linear Projection
    ↓
Vocabulary Logits
    ↓
Next Token Prediction
    ↓
Generated Text
