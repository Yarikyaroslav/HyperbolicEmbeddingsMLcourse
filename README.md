# HyperbolicEmbeddingsMLcourse
Here is the repository with the code for Hyperbolic Embeddings project.

# Comparison of Hyperbolic and Euclidean Embeddings for CIFAR Dataset Classification

This repository contains the code and analysis for comparing hyperbolic and Euclidean embeddings in the context of classifying images from the CIFAR dataset. The project explores the efficiency and effectiveness of these embeddings in capturing the underlying geometric structure of the data, potentially leading to improved classification performance.

## Project Overview

The CIFAR dataset consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class. This project aims to evaluate the performance of classification models that utilize hyperbolic embeddings, as opposed to traditional Euclidean embeddings, to represent the images in a geometric space that is more suited to capturing hierarchical and relational structures inherent in many types of data.

## Key Results

- Euclidean networks trains more stable, compare to the Hyperbolic; the latter shows big jumps in both cross-entropy loss and accuracy during the training.
- Euclidean networks learns faster.
- Nevertheless, one can achieve better score using Hyperbolic network than with the Euclidean one.
- We observe big Hyperbolic network to overfit more than Euclidean one.

## Repository Structure

- `HyperbolicCIFAR.ipynb`: Jupyter notebook containing all the experiments, analysis, and visualizations comparing hyperbolic and Euclidean embeddings.
- `requirements.txt`: A list of Python dependencies required to run the code.

## Getting Started

### Prerequisites

Ensure you have Python 3.6 or later installed on your system. Additionally, to run the code, you need to download "hyptorch" from the following repository:

[hyperbolic-image-embeddings](https://github.com/leymir/hyperbolic-image-embeddings)

### Installation

1. Clone this repository to your local machine or Google Colab environment via GitHub.
2. Install the required Python dependencies: pip install -r requirements.txt

### Running the Code

To reproduce the experiments and analysis, simply run the `HyperbolicCIFAR.ipynb` notebook:

- If using a local Jupyter setup:jupyter notebook HyperbolicCIFAR.ipynb

- If using Google Colab, upload the notebook and follow the Colab instructions to execute it.


## Acknowledgements

- Special thanks to the creators of the "hyptorch" library for providing the tools necessary for hyperbolic image embeddings.

