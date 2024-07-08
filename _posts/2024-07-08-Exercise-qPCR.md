---
layout: post
title: Exercise qPCR
date: '2024-07-08'
categories: Analysis, Protocols
tags: qPCR
---


# Analyzing qPCR Data

## Ct (Cycle Threshold) Values
Ct is the number of cycles needed for the fluorescent signal to exceed the background level. Lower Ct values indicate higher target nucleic acid amounts.

|                      | ubi   | Rac1  | RhoA  | CDC42 | Rock1 | Vegf  | VegfR | RhoGap24l/2 |
| -------------------- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----------- |
| DMSO Control         | 20.72 | 25.65 | 29.13 | 28.45 | 28.28 | 29.71 | 28.61 | 29.48       |
| Inhibitor treatment  | 19.89 | 25.34 | 28.41 | 27.38 | 28.01 | 28.85 | 28.36 | 30.45       |


## ΔCt (Delta Ct) Values
ΔCt is the difference between the Ct of the target gene and the reference gene, normalizing for variations in starting material.

|                      | Rac1 | RhoA | CDC42 | Rock1 | Vegf | VegfR | RhoGap24l/2 |
| -------------------- | ---- | ---- | ----- | ----- | ---- | ----- | ----------- |
| DMSO Control         | 4.93 | 8.41 | 7.73  | 7.56  | 8.99 | 7.89  | 8.76        |
| Inhibitor treatment  | 5.45 | 8.52 | 7.49  | 8.12  | 9.02 | 8.47  | 10.56       |


## ΔΔCt (Delta Delta Ct) Values
ΔΔCt is the difference between the ΔCt of the experimental sample and the ΔCt of the control, allowing relative gene expression calculation.

| Genes | Rac1 | RhoA | CDC42  | Rock1 | Vegf   | VegfR | RhoGap24l/2 |
| ----- | ---- | ---- | ------ | ----- | ------ | ----- | ----------- |
| ΔΔCt  | 0.52 | 0.11 | \-0.24 | 0.56  | \-0.07 | 0.58  | 1.80        |


## Relative Quantification
Measures changes in gene expression relative to a control using the 2^(-ΔΔCt) method.

| Genes | Rac1 | RhoA | CDC42 | Rock1 | Vegf | VegfR | RhoGap24l/2 |
| ----- | ---- | ---- | ----- | ----- | ---- | ----- | ----------- |
| RQ    | 0.70 | 0.93 | 1.18  | 0.69  | 1.05 | 0.67  | 0.29        |

---

