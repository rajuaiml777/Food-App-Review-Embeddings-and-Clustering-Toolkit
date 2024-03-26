# Food App Review Embeddings and Clustering

## Overview

This repository contains code and resources related to generating embeddings for a food app review dataset using the Sentence Transformer model (specifically, the all_MiniLm_L6_v2 variant). The embeddings are visualized in 2D and 3D vector spaces using UMAP and Plotly. Additionally, k-means clustering is applied to the embeddings.

# Project Structure

data/: Contains the food app review dataset.

notebooks/: Jupyter notebooks for embedding generation, visualization, and clustering.

scripts/: Any additional scripts or utilities.

results/: Visualizations and clustering results.

README.md: This README file.

# Usage
## Data Preparation:
Place your food app review dataset in the data/ directory.

Preprocess the data (e.g., tokenization, cleaning) as needed.

# Embedding Generation:
Run the notebook in notebooks/1_generate_embeddings.ipynb.

Use the Sentence Transformer model (all_MiniLm_L6_v2) to create embeddings for the reviews.

# Visualization:
Explore the embeddings using UMAP and Plotly in notebooks/2_visualize_embeddings.ipynb.

Generate 2D and 3D scatter plots to visualize the review representations.

# Clustering:
Apply k-means clustering to the embeddings in notebooks/3_kmeans_clustering.ipynb.

Analyze the clusters and interpret the results.

# Results:
Save visualizations and clustering results in the results/ directory.

# Dependencies

Make sure you have the following Python libraries installed:

sentence-transformers

umap-learn

plotly

scikit-learn

# Acknowledgments

The Sentence Transformer model: Hugging Face Transformers

UMAP: UMAP-learn

Plotly: Plotly Python

Feel free to customize this README to suit your project’s specifics. Happy coding! 🚀
