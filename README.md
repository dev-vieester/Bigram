# Bigram

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10%2B-3776AB.svg" alt="Python 3.10+" />
  <img src="https://img.shields.io/badge/PyTorch-2.x-EE4C2C.svg" alt="PyTorch" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626.svg" alt="Jupyter" />
</p>

A lightweight Python project that explores character-level bigram statistics and demonstrates how simple probabilistic language models can learn patterns from a names dataset.

## Overview

This repository contains a Jupyter Notebook that:

- downloads a public dataset of names
- inspects the data structure and word statistics
- counts character-to-character transitions (bigrams)
- builds a frequency table for common letter pairs
- creates a transition matrix using PyTorch
- demonstrates how language patterns emerge from repeated sequences

The project is intentionally simple and educational, making it a great example of how probabilistic modeling works at the character level.

## Features

- Character-level bigram frequency analysis
- Dataset exploration for names
- Transition matrix creation in PyTorch
- Easy-to-follow notebook workflow
- Beginner-friendly implementation for learning ML and language modeling basics

## Repository Structure

```text
Bigram/
├── Bigram.ipynb      # Main notebook for analysis and modeling
├── README.md         # Project documentation
├── requirements.txt  # Dependency list
├── .gitignore        # Local environment and generated file exclusions
└── names.txt         # Downloaded during notebook execution (generated locally)
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/dev-vieester/Bigram.git
cd Bigram
```

### 2. Create a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
# .venv\Scripts\activate    # Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter

```bash
jupyter notebook
```

Then open `Bigram.ipynb` and run the cells in order.

## Workflow

The notebook demonstrates a typical learning flow:

1. Download a list of names
2. Inspect word length and dataset size
3. Count adjacent character pairs
4. Identify the most frequent bigrams
5. Build a matrix of transitions
6. Use the matrix to reason about probable character sequences

## Example of the analysis

The notebook reveals common transitions such as:

- `an`
- `ar`
- `el`
- `ri`
- `na`

These patterns show how a basic character model captures structure in names and language-like sequences.

## Requirements

- Python 3.10+
- PyTorch
- Jupyter Notebook
- requests

## Notes

This project is designed for educational purposes and experimentation. It is a compact example of how bigram statistics can be used to understand and model text generation at a low level.

## Future Improvements

Possible enhancements include:

- adding a function to generate names from the learned matrix
- visualizing bigram distributions
- extending the model to trigrams
- comparing different text datasets and results

## Author

Created and maintained by the repository owner.
