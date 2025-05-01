---
layout: page
permalink: /teaching/
title: teaching
description: 
nav: true
nav_order: 2
---

## Spring 2025: EN.553.744 – Data Science Methods for Large-Scale Graphs (new class!)
nal processing, graph neural networks (GNNs), graphon theory and transferability, and scalable training techniques for large graphs. Students engage with both foundational theory and practical implementation using PyTorch and PyTorch Geometric.
This graduate course introduces mathematical and computational methods for analyzing graph-structured data at scale.

**Lectures**  

Lectures 1–10 cover graph signal processing, graph Fourier transforms, graph filters, multilayer GNNs, spectral clustering, and stochastic block models.
Lectures 11–20 build toward expressivity and stability of GNNs, Lipschitz filter design, graphon models, and convergence and transferability results.
Lecture 21 introduces generative models for graphs, including GraphRNNs, and graph transformers.

Below is a list of handwritten lecture notes, Colab notebooks, and lab assignments. 

| Lecture | Description | Notes |
|---------|-------------|-------|
| Lecture 1 | Intro to GSP; graph diffusion processes; graph Laplacian and graph frequencies | [PDF](/assets/teaching/744/Lecture%201.pdf) |
| Lecture 2 | Interpretation of Laplacian; total variation energy; graph Fourier transform | [PDF](/assets/teaching/744/Lecture%202.pdf) |
| Lecture 3 | Graph convolutions and their theoretical properties | [PDF](/assets/teaching/744/Lecture%203.pdf) |
| Lecture 4 | Filter design, ERM on graphs, types of graph learning problems | [PDF](/assets/teaching/744/Lecture%204.pdf) |
| Lecture 5 | Graph perceptrons, multi-layer perceptrons, full-fledged GNNs | [PDF](/assets/teaching/744/Lecture%205.pdf) |
| Lecture 6 | Stochastic block model; spectral clustering; GNNs for detecting communities | [PDF](/assets/teaching/744/Lecture%206.pdf), [Colab](https://colab.research.google.com/drive/1BOci3lgVX9fVwy9SEGTA20oZAh0ib-Xn#scrollTo=a4711Id8GFAq)|
| Lecture 7 | Community detection miscellanea; sparse matrix multiplications | [PDF](/assets/teaching/744/Lecture%207.pdf), [HW1](/assets/teaching/744/EN_553_744_HW1.pdf) |
| Lecture 8 | MPNN, GCN, ChebNet, GraphSAGE are all convolutional GNNs | [PDF](/assets/teaching/744/Lecture%208.pdf) |
| Lecture 9 | GAT; expressivity in graph-level tasks; graph isomorphism and WL test | [PDF](/assets/teaching/744/Lecture%209.pdf), [Colab](https://colab.research.google.com/drive/1YaugbgRDo1nFAl4ZsYC-amKOgp_3-Uhm?usp=sharing)|
| Lecture 10 | Expressivity continued and GIN | [PDF](/assets/teaching/744/Lecture%2010.pdf) |
| Lecture 11 | Limitations of WL test and GIN; white inputs for improved expressivity | [PDF](/assets/teaching/744/Lecture%2011.pdf), [Colab](https://colab.research.google.com/drive/12_CDhE4fh0xuLwbIwediOJPlecrumiAf?usp=sharing) |
| Lecture 12 | Stability of GNNs to graph perturbations | [PDF](/assets/teaching/744/Lecture%2012.pdf) |
| Lecture 13 | Perturbation types; Lipschitz and integral Lipschitz filters | [PDF](/assets/teaching/744/Lecture%2013.pdf), [HW2](/assets/teaching/744/EN_553_744_HW2.pdf) |
| Lecture 14 | Graphons and homomorphism densities | [PDF](/assets/teaching/744/Lecture%2014.pdf) |
| Lecture 15 | Cut norm and convergence to graphons | [PDF](/assets/teaching/744/Lecture%2015.pdf) |
| Lecture 16 | Graphon signal processing: Fourier transform | [PDF](/assets/teaching/744/Lecture%2016.pdf), [Colab](https://colab.research.google.com/drive/10DCmAealM8huWhMFVCzN2tjZUNKgSubY?usp=sharing) |
| Lecture 17 | Graphon signal processing: convolutions | [PDF](/assets/teaching/744/Lecture%2017.pdf) |
| Lecture 18 | Convergence of graph convolutions | [PDF](/assets/teaching/744/Lecture%2018.pdf) |
| Lecture 19 | Non-asymptotic convergence and transferability | [PDF](/assets/teaching/744/Lecture%2019.pdf) |
| Lecture 20 | Transferability rates and learning by transference | [PDF](/assets/teaching/744/Lecture%2020.pdf), [HW3](/assets/teaching/744/EN_553_744_HW3.pdf) |
| Lecture 21 | Graph generative models and graph transformers | [PDF](/assets/teaching/744/Lecture%2021.pdf) |

---

## Spring 2024: EN.553.439/639 – Time Series Analysis

This course introduces methods for analyzing and forecasting time series data, including autoregressive (AR), moving average (MA) ARMA, ARIMA and seasonal models. Applications include finance, climate science, and engineering. Materials based on "Time Series Analysis with Applications in R" by Cryer and Chan, and on previous iterations taught by [Dr. Fred Torcaso](https://engineering.jhu.edu/faculty/federico-torcaso/) and [Dr. Sergey Kushnarev](https://www.linkedin.com/in/sergey-kushnarev-94460511).

---

## Fall 2023 and 2025: EN.553.413/613 – Applied Statistics and Data Analysis

Co-taught with [Dr. Sergey Kushnarev](https://www.linkedin.com/in/sergey-kushnarev-94460511) (2023) and [Dr. Kaiying O'Hare](https://sites.google.com/view/kaiying-xie) (2025). This course provides a practical introduction to statistical modeling and inference, covering linear regression, hypothesis testing, ANOVA, and non-parametric methods. Students work with real datasets and statistical software for data-driven decision making. Materials based on "Applied Linear Statistical Models" by Kutner, Nachtsheim, Neter and Li.