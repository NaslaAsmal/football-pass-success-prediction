# football-pass-success-prediction
# Football Pass Success Classification Using a Directed GCN
Submitted by: Nasla K

Register Number: 2026PHD21005 
Course: DSC622 Graph Algorithms and Mining
Programming Language: Python

Environment: Anaconda Jupyter Notebook
## Project Overview
This project implements a Graph Neural Network-based approach to classify football passes as successful or unsuccessful using StatsBomb Open Data from the FIFA Women's World Cup 2023.

## Dataset
- Data source: StatsBomb Open Data
- Competition: FIFA Women's World Cup 2023
- Matches: 64
- Total passes: 59,469

## Methodology
1. Data collection and preprocessing
2. Pass-level feature extraction
3. Match-wise training, validation and test splitting
4. Directed graph construction
5. Directed GCN-style message passing
6. Class-weighted model training
7. Model evaluation

## Model Architecture
- Input features: 10
- Hidden layers: 32 and 16
- Output classes: 2
- Optimiser: Adam
- Learning rate: 0.001
- Training epochs: 60

## Results

| Metric | Test Result |
|---|---:|
| Accuracy | 77.66% |
| Macro F1-score | 0.73 |
| Weighted F1-score | 0.79 |

## Technologies Used
- Python
- Pandas and NumPy
- Scikit-learn
- PyTorch
- PyTorch Geometric
- JupyterLab

## Important Note
The model classifies recorded pass outcomes using pass attributes, including destination coordinates, pass length and angle. It is not a prediction made before the pass is attempted.

## Dataset Source
[StatsBomb Open Data](https://github.com/statsbomb/open-data)

## Project Notebook
[Footballpassprediction.ipynb](./Footballpassprediction.ipynb)
