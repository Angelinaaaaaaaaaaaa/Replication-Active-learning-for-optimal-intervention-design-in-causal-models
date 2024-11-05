# Replication-Active-learning-for-optimal-intervention-design-in-causal-models
DSC180 Project by Cici and Angelina
This is an replication for paper: Active learning for optimal intervention design in causal models (Nature Machine Intelligence, 2023). Specifically, we focused on replicating the experiment on synthetic data. \

## Installation
Follow the two steps illustrated below

1. create a conda environment using `environment.yaml` (all dependencies are included; whole process takes about 5 min):
```
conda env create -f environment.yml
```
2. install the current package in editable mode inside the conda environment:
```
pip install -e .
```

## Synthetic data
Run on a synthetic instance, e.g.:
```
python run.py --nnodes 5 --noise_level 1 --DAG_type path --std --a_size 2 --a_target 3 4 --acquisition greedy
```
After running, results will be stored in a folder, which contains of 3 pickle files. 
To visualze the results: 
```
python visualze_results.py
```
Source code folder: `./optint/`

