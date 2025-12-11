# Dimensionality Reduction: PCA vs t-SNE on Synthetic 50D Dataset

This project compares two dimensionality reduction techniques—Principal Component Analysis (PCA) and t-distributed Stochastic Neighbor Embedding (t-SNE)—on a synthetic high-dimensional dataset.

## Overview

The notebook generates a synthetic 50-dimensional dataset with 4 distinct Gaussian clusters and evaluates how well PCA and t-SNE can preserve cluster structure when reducing dimensionality to 2D for visualization.

## Key Features

- **Synthetic Dataset Generation**: Creates a 50-dimensional dataset with 4 classes (400 samples each, 1600 total samples)
- **PCA Analysis**: Linear dimensionality reduction with variance analysis
- **t-SNE Analysis**: Non-linear dimensionality reduction with different perplexity values (30 and 50)
- **Quantitative Comparison**: Uses silhouette scores to compare embedding quality
- **Visualizations**: Multiple plots including scatter plots, scree plots, correlation heatmaps, and pair plots

## Requirements

See `requirements.txt` for the complete list of dependencies.

Main libraries:
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Installation

1. Clone this repository:
```bash
git clone <repository-url>
cd <repository-name>
```

2. Install the required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Open the Jupyter notebook:
```bash
jupyter notebook notebook.ipynb
```

2. Run all cells to execute the complete analysis.

## Project Structure

```
.
├── notebook.ipynb          # Main analysis notebook
├── README.md               # This file
├── requirements.txt        # Python dependencies
└── .gitignore             # Git ignore rules
```

## Results Summary

The analysis compares:
- **PCA (2D)**: Linear projection onto first two principal components
- **t-SNE (perplexity=30)**: Non-linear embedding with perplexity 30
- **t-SNE (perplexity=50)**: Non-linear embedding with perplexity 50

Silhouette scores are computed to quantitatively assess cluster separation in each embedding.

## Key Findings

- PCA captures the majority of variance in the first few components
- t-SNE provides different visualizations depending on perplexity settings
- Both methods reveal cluster structure, with varying degrees of separation

## Author

Sai Krishna Nallavula

## License

This project is part of a Machine Learning and Neural Networks course assignment.
