## SAX implementation & Experiment Replication

This repository contains SAX implementation and the replication of key experiments described in:  
[A Symbolic Representation of Time Series, with Implications for
Streaming Algorithms](https://www.cs.ucr.edu/~eamonn/SAX.pdf)
(Jessica Lin, Eamonn Keogh, Stefano Lonardi, Bill Chiu, DMKD 2003)

## Overview

The code demonstrates:
* SAX (Symbolic Aggregate approXimation) implementation:  
   - Z-normalization  
   - Piecewise Aggregate Approximation (PAA)  
   - Discretization into symbols (with breakpoints for equiprobable regions under a Gaussian curve)  
   - A lower-bounding distance measure for SAX (MINDIST)  
* Hierarchical clustering (both Euclidean and SAX-based distances).  
* 1-NN classification (leave-one-out) with Euclidean and SAX-based distances.  
* Index-like experiments (not full indexing structures, but distance-based retrieval) to show speed-up via SAX pruning.  
* **Extra experiment:** Two-level SAX approach to further prune candidates in a query-by-content setting.


## Run

1. Install Python dependencies (e.g., via pip): 
```bash
pip install numpy scipy matplotlib
```
1. Run the jupyter notebook
