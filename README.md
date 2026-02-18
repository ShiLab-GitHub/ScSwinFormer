# Introduction:

This repository contains the data and python script in support of paper: [scFormer: A Transformer-Based Cell Type Annotation Method for scRNA-seq Data Using Smooth Gene Embedding and Global Features.](https://doi.org/10.1021/acs.jcim.4c00616 ) This work focuses on the annotation of scRNA-seq data using the Transformer-based deep learning model scFormer. Published in Journal of Chemical Information and Modeling.

# Requirement:

```
Python==3.8.0
PyTorch >= 1.5.0
numpy==1.22.4
pandas==1.2.2
scipy==1.8.1
sklearn==1.9.1
Scanpy==1.9.1
```

# Usage:

python scFormer.py

in which

```
k=2000 Pre-processing selection of 2000 highly variable genes
s=The length of Smooth gene embedding dimension
scFormer(input_size, output_size)
input_size = n_top_genes
output_size = labels_size
```

Before running scFormer,please modify your file path and names (two files: the preprocessed scRNA-seq data file and its cell-type file). Please make sure your data file format: count matrix dimension is (genes*cells), label dimension is (1*cells).

Example data can be found in https://figshare.com/s/7651fa9725807dfb3dbc, Save to file path 'data/Adipose/'.

# Citation:
Please cite our paper if you use the code.
