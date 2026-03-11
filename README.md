# LeAP: Learnable Adaptive Permutation for Feature Selection in Heterogeneous and Sparse Recommender Systems

## Getting Started
### Dataset
The dataset are available at: [[MEGA_LINK](https://mega.nz/file/n8hBHJjb#GCaqxo-tZV61HiP7LoEXu3zCvDX2k6LKcZ77Om-eYIw)] for the purpose of peer review.

If you encounter a transfer quota limit, please try again after a few hours or use a VPN.

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