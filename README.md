# LeAP: Learnable Adaptive Permutation for Feature Selection in Heterogeneous and Sparse Recommender Systems

## Getting Started
### Dataset
The dataset are available at: [huggingface](https://huggingface.co/datasets/yihong-1101/DRS-dataset/tree/main) for the purpose of peer review.

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