# LeAP: Learnable Adaptive Permutation for Feature Selection in Heterogeneous and Sparse Recommender Systems

## Getting Started

### Dataset
The preprocessed DRS dataset is available on Huggingface:
- Dataset: [DRS-dataset](https://huggingface.co/datasets/yihong-1101/DRS-dataset)
- Download the dataset to the `quick_data` directory

Note: `utils/datasets.py` describes how we transform the original ERASE dataset [ERASE_Dataset](https://huggingface.co/datasets/Jia-py/ERASE_Dataset) to our dataset, in order to achieve a smaller storage and much more efficient read files speed.

2. **Generate preprocessed datasets**: Run the data generation script to create optimized parquet files with smaller storage and faster loading:
   ```bash
   cd data
   python utils/datasets.py
   ```
   This will generate preprocessed datasets in `quick_data/` as parquet files with accompanying JSON metadata files.

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