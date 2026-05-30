# LeAP: Learnable Adaptive Permutation for Feature Selection in Heterogeneous and Sparse Recommender Systems

[![Conference](https://img.shields.io/badge/ECML%20PKDD-2026-blue)](https://2026.ecmlpkdd.org/)

This repository contains the official implementation of **LeAP**, as presented in our paper accepted at **ECML PKDD 2026**.

## Overview

Modern industrial recommender systems rely on thousands of heterogeneous features to achieve high-precision predictions. Efficient feature selection is critical to reduce computational costs, but existing methods struggle with dimensional heterogeneity, extreme feature sparsity, and the computational bottlenecks of traditional permutation methods.

**LeAP (Learnable Adaptive Permutation)** is a novel, model-agnostic plug-in module designed to address these challenges. By transforming the inefficient discrete permutation process into an end-to-end learnable mechanism, LeAP accelerates feature evaluation to `O(1)` complexity. Furthermore, it introduces an adaptive regularization strategy based on Permutation Divergence, which effectively handles dimension discrepancy and sparse features, driving feature gating scores to naturally polarize for direct, threshold-based pruning.

## Getting Started

### Datasets
The pre-processed public datasets used for evaluation are hosted on [Hugging Face](https://huggingface.co/datasets/yihong-1101/DRS-dataset/tree/main). Please download the datasets and place them in the root directory before running the experiments.

### Prerequisites
All required packages are listed in `requirements.txt`.

## Running Experiments

The experimental pipeline consists of two stages:

### 1. Search and Retrain Stage
Run all feature selection methods:
```bash
python search_and_retrain.py
```
Results will be saved in the `exp_save` directory.

