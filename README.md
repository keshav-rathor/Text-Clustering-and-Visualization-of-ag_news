
# AG News Clustering and Visualization

## Overview

This project involves clustering and visualizing AG News articles using text embeddings. We utilize state-of-the-art models for embedding extraction and employ advanced techniques for dimensionality reduction and clustering. The project demonstrates various approaches to understanding and visualizing textual data, including PCA, UMAP, and interactive 3D plots.

## Features

- **Text Embeddings**: Uses DistilBERT to convert news articles into dense vector representations.
- **Clustering**: Applies KMeans clustering to group articles based on their embeddings.
- **Dimensionality Reduction**: Utilizes PCA and UMAP for reducing the dimensionality of embeddings to visualize clusters.
- **Visualization**:
  - 2D scatter plots using PCA and UMAP.
  - Interactive 3D scatter plots with Plotly.

## Dataset

- **AG News**: The dataset consists of news articles categorized into four classes: World, Sports, Business, and Science/Technology. For simplicity, we use a subset of 100 samples from the training set.

## Installation

To run this project, ensure you have the following packages installed:

```bash
pip install transformers datasets sklearn matplotlib torch umap-learn plotly
```

## Usage

1. **Loading and Preparing Data**:
   - We use the `datasets` library to load the AG News dataset.
   - Texts from the dataset are tokenized and embedded using DistilBERT.

2. **Embedding Extraction**:
   - The DistilBERT model converts texts into embeddings. We use the [CLS] token representation for clustering.

3. **Clustering**:
   - KMeans clustering is applied to the embeddings to group the articles into clusters.

4. **Visualization**:
   - **PCA Visualization**: Reduced dimensionality to 2D and plotted using Matplotlib.
   - **UMAP Visualization**: Reduced dimensionality to 2D and plotted using Matplotlib.
   - **3D Interactive Plot**: Plotted using Plotly for a more interactive exploration of clusters.

## Example Visualizations

### 2D PCA Visualization

![PCA Visualization](path/to/pca_visualization.png)

### 2D UMAP Visualization

![UMAP Visualization](path/to/umap_visualization.png)

### 3D Interactive Plot

![3D Plot](path/to/3d_plot.html)

## Results

- **PCA Visualization**: Shows how the clusters are distributed in a 2D space.
- **UMAP Visualization**: Provides a more nuanced view of cluster separations.
- **3D Interactive Plot**: Allows for interactive exploration of clusters and their distributions.

