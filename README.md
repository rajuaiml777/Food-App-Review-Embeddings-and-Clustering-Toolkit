# Food App Review Embeddings, Visualizations, and Clustering

![Food App Review Embeddings](images/food-app-review-embeddings.jpg)

## Overview
This repository contains code and resources related to generating embeddings for a food app review dataset using the Sentence Transformer model (specifically, the all_MiniLm_L6_v2 variant). The embeddings are visualized in 2D and 3D vector spaces using UMAP and Plotly, and k-means clustering is applied to the embeddings.

## Getting Started
To get started with this project, follow these steps:

1. **Clone the repository**: 
   ```
   git clone https://github.com/your_username/food-app-reviews.git
   ```
2. ** Install dependencies:** 
```
pip install -r requirements.txt
```

## Table of Contents
1. [Use SentenceTransformers to Generate Embeddings](#use-sentencetransformers-to-generate-embeddings)
2. [Visualise the Embeddings through Dimensionality Reduction](#visualise-the-embeddings-through-dimensionality-reduction)
3. [Cluster and Visualise the Embeddings with Plotly](#cluster-and-visualise-the-embeddings-with-plotly)
4. [Visualise the Embeddings in 3D](#visualise-the-embeddings-in-3d)
5. [Getting Started](#getting-started)

## 1. Use SentenceTransformers to Generate Embeddings
Sentence Transformers are advanced natural language processing models that encode sentences into high-dimensional vectors. These vectors encapsulate the semantic nuances of text, offering a robust foundation for various text-related tasks, such as clustering, classification, and more.

### The Hugging Face Connection
Hugging Face, a pioneering platform in NLP, hosts an array of pre-trained models, including Sentence Transformers, that can be readily employed for diverse applications. `sentence-transformers` is a library that provides easy methods to compute embeddings (dense vector representations) for sentences, paragraphs, and images. Texts are embedded in a vector space such that similar text is close, which enables applications such as semantic search, clustering, and retrieval.

### Sentence Transformers Models
Hugging Face's Sentence Transformers collection includes an assortment of models designed to cater to different use cases. From general-purpose models like BERT and RoBERTa to specialized models fine-tuned for specific tasks, the library provides a plethora of choices for generating embeddings that align with your data's context.

### The Mini-LM-6-v2 models
In this demonstration, we'll use a model from the MiniLM-L6-v2 range of Sentence Transformer models to generate embeddings.

Specifically, we will try out the all-MiniLM-L6-v2 model. The all-MiniLM-L6-v2 sentence transformer, trained on a large dataset of over 1 billion training pairs, is a model that maps sentences and paragraphs to a 384-dimensional dense vector space. The all-MiniLM-L6-v2 model is designed as a general-purpose model and offers good quality embeddings. It can be used for tasks like clustering or semantic search.

## 2. Visualise the Embeddings through Dimensionality Reduction
Modern datasets often consist of numerous features or attributes, which creates a high-dimensional space in which our data resides. However, when trying to comprehend or visualize such data directly, we run into limitations – our brains struggle to visualize beyond three dimensions, and traditional visualization methods might not accurately represent the relationships between data points in high-dimensional spaces.

UMAP, which stands for Uniform Manifold Approximation and Projection, is a dimensionality reduction technique that reveals local and global data relationships. It transforms high-dimensional data into a lower-dimensional space, helping us visualize clusters, trends, and similarities.

UMAP is a powerful tool in Python that can help us perform dimensionality reduction.

## 3. Cluster and Visualise the Embeddings with Plotly
Let's now try and interpret the embedding space. We will first cluster the data points to check similar sentences. Clustering is a vital technique that groups similar data points together based on their closeness to each other.

### From Embeddings to Clusters
By applying clustering algorithms to our embeddings, we can group together similar embeddings, effectively creating clusters of related data points. This process enables us to uncover meaningful categories or classes within our data and helps us interpret what the clusters actually mean.

## 4. Visualise the Embeddings in 3D
Let's now try to visualize the same embeddings in 3D. The process is almost exactly the same. This time, we will use the UMAP function to reduce the dimension to 3 instead of 2.

### Visualization in 3D
Visualizing embeddings in 3D offers an additional perspective compared to 2D visualization. It can reveal more intricate patterns and relationships within the data, potentially leading to deeper insights.

## 5. Evaluation and Next Steps
After visualizing the embeddings and clusters, it's essential to evaluate the results and consider potential next steps. This may include further analysis of the clusters, refinement of the visualization techniques, or exploration of additional methods to extract insights from the data. Additionally, considering the practical applications of the findings and how they can be utilized to improve the food app experience is crucial.

