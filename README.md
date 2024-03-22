# Comparison of Hyperbolic and Euclidean Embeddings for MNIST and CIFAR Dataset Classification

## Introduction
This project compares the performance of hyperbolic and Euclidean embeddings in the context of classifying images from the MNIST and CIFAR datasets. The project explores the efficiency and effectiveness of these embeddings in capturing the underlying geometric structure of the data, potentially leading to improved classification performance.

## Project Overview (CIFAR)
The CIFAR dataset consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class. This project aims to evaluate the performance of classification models that utilize hyperbolic embeddings, as opposed to traditional Euclidean embeddings, to represent the images in a geometric space that is more suited to capturing hierarchical and relational structures inherent in many types of data.

### Key Results (CIFAR)
- Euclidean networks trains more stable, compare to the Hyperbolic; the latter shows big jumps in both cross-entropy loss and accuracy during the training.
- Euclidean networks learns faster.
- Nevertheless, one can achieve better score using Hyperbolic network than with the Euclidean one.
- We observe big Hyperbolic network to overfit more than Euclidean one.

## Project Overview (MNIST)
The MNIST dataset consists of 70,000 tiny (28x28) grayscale images of handwritten digits, from zero to nine. This project aims to apply similar methodologies used for CIFAR dataset classification to evaluate the performance of hyperbolic and Euclidean embeddings on MNIST dataset.

### Key Results (MNIST)
- The Euclidean network achieves a test accuracy of 97%.
- The Hyperbolic network achieves a test accuracy of 96%.

## Repository Structure
- `HyperbolicCIFAR.ipynb`: Jupyter notebook containing all the experiments, analysis, and visualizations comparing hyperbolic and Euclidean embeddings for CIFAR dataset.
- `Hyperbolic_on_mnist_data.ipynb`: Jupyter notebook containing all the experiments, analysis, and visualizations comparing hyperbolic and Euclidean embeddings for MNIST dataset.
- `requirements.txt`: A list of Python dependencies required to run the code.

## Getting Started

### Prerequisites

Ensure you have Python 3.6 or later installed on your system. Additionally, to run the code, you need to download "hyptorch" from the following repository:

[hyperbolic-image-embeddings](https://github.com/leymir/hyperbolic-image-embeddings)

### Installation

1. Clone this repository to your local machine or Google Colab environment via GitHub.
2. Install the required Python dependencies: `pip install -r requirements.txt`

### Running the Code

To reproduce the experiments and analysis, simply run the respective notebooks:
- For CIFAR dataset: `HyperbolicCIFAR.ipynb`
- For MNIST dataset: `Hyperbolic_on_mnist_data.ipynb`

- If using a local Jupyter setup: `jupyter notebook HyperbolicCIFAR.ipynb` or `jupyter notebook Hyperbolic_on_mnist_data.ipynb`
- If using Google Colab, upload the notebooks and follow the Colab instructions to execute them.

## Acknowledgements
Special thanks to [leymir](https://github.com/leymir) for providing the "hyptorch" library necessary for hyperbolic image embeddings. Additionally, we would like to acknowledge the creators of the "geoopt" library for providing tools such as the Riemannian optimizer necessary for optimizing hyperbolic neural networks. You can find example scripts and notebooks demonstrating the usage of hyperbolic embeddings, such as the `mobius_linear_example.py` file [here](https://raw.githubusercontent.com/geoopt/geoopt/master/examples/mobius_linear_example.py) and the `hyperbolic_multiclass_classification.ipynb` notebook [here](https://github.com/geoopt/geoopt/blob/master/examples/hyperbolic_multiclass_classification.ipynb).
