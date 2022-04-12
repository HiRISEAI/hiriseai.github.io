---
layout: post
title:  "PyTorch Notes: PyTorch Tensors"  
date: 2022-3-3  
image: assets/images/ESP_011785_1875_4_1_notes.pytorch.png  
tags: [ AI, MinLab, notes.ML ]
---


**PyTorch has various components**.  

- `torch` has functionalities similar to NumPy with GPU support.
-  `torch.autograd` provides classes, methods, and functions for implementing automatic differentiation of arbitrary scalar valued functions. 
- `nn` is a neural network library in PyTorch.
- `optim` provides optimization algorithms that are used for the minimization and maximization of functions.
- `utils` has utility functions to load data; it also has other functions...
  

**Creating a tensor with all elements initialized with the same value**  
- `torch.zeros( )`: returns a tensor filled with the scalar value 0, with the shape defined by the variable argument size.  
- `torch.ones( )`: returns a tensor filled with the scalar value 1, with the shape defined by the variable argument size.
- `torch.eye( )`: reuturns a 2-D tensor with ones on the diagonal and zeros elsewhere.
- `torch.empty( )`: returns a tensor filled with uninitialized data. The shape of the tensor is defined by the variable argument size. 
- `torch.full( )`: creates a tensor size filled with `fill_value`. the tensor's dtype is inferred from `fill_value`.

**Tensor syntax**
- `torch.numel( )`: returns the total number of elements in the input tensor.
- `torch.rand( )`: returns a tensor filled with random numbers from a uniform distribution on the interval[0,1).
- `torch.randn( )`: returns a tensor filled with random numbers from a normal distribution with mean 0 and variance 1 (also called the standard normal distribution). The shape of the tensor is defined by the variable argument `size`.
- `torch.argmin( )`: returns the indices of the minimum value(s) of hte flattened tensor or along a dimension. If there are multiple minimal values then the indices of the first minimal value are returned.
- `torch.argmax( )`: returns the indices of the maximum value of all elements in the `input` tensor. If there are multiple maximal values then the indices of the first maximal value are returned.
- `torch.cat(tensors, dim=0)`: concatenates the given sequence of `seq` tensors in the given dimension. All tensors must either have the same shape (except in the concatenating dimension) or be empty. The inverse operation is `torch.split( )`.

The scripts can be seen here: 
- [https://github.com/rocks2021/Colabs-for-HiRISEAI/blob/main/pt1_pytorch_tensors.ipynb](https://github.com/rocks2021/Colabs-for-HiRISEAI/blob/main/pt1_pytorch_tensors.ipynb){:target="_blank"}  
- [https://github.com/rocks2021/Colabs-for-HiRISEAI/blob/main/pt2_pytorch_tensors.ipynb](https://github.com/rocks2021/Colabs-for-HiRISEAI/blob/main/pt2_pytorch_tensors.ipynb){:target="_blank"}  
- [https://github.com/rocks2021/Colabs-for-HiRISEAI/blob/main/pt3_pytorch_tensors.ipynb](https://github.com/rocks2021/Colabs-for-HiRISEAI/blob/main/pt3_pytorch_tensors.ipynb){:target="_blank"}
