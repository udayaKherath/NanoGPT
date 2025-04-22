# NanoGPT: A Decoder-Only Transformer from Scratch

This repository contains an implementation of a decoder-only transformer model built from scratch using PyTorch, inspired by the architecture of GPT models. The model is designed for character-level language modeling and text generation.

## Overview

MiniGPT is a lightweight transformer model that learns to predict the next character in a sequence of text. The model consists of:

- Multi-head self-attention layers
- Feed-forward networks
- Layer normalization
- Positional embeddings
- Token embeddings

## Model Architecture

The architecture follows the standard decoder-only transformer design:

- **Embedding Layer**: Converts token IDs to vectors and adds positional embeddings
- **Transformer Blocks**: Self-attention and feed-forward networks with residual connections
- **Output Layer**: Projects to vocabulary size for next-token prediction

### Specifications

- Embedding Dimension: 384
- Number of Heads: 6
- Number of Layers: 6
- Vocabulary: Character-level
- Context Window: 256 tokens
- Dropout: 0.2

## Features

- Character-level tokenization
- Causal (masked) self-attention
- Text generation with multinomial sampling
- Training and validation loss tracking

## Requirements

- Python 3.6+
- PyTorch 1.0+
- CUDA-compatible GPU (recommended but not required)

## Output

### Training and Validation Loss
![Training and Validation Loss](./Capture1.png)

### Sample Output
![Sample Output Text](./Capture2.png)
