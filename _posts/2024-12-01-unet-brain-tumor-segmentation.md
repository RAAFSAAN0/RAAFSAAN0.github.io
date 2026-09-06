---
layout: blog_post
title: "Comparative Analysis of U-Net Variants for Brain Tumor Segmentation"
date: 2025-01-02
tags:
  - TensorFlow
  - PyTorch
  - Medical Imaging
  - BraTS20
---

## Overview

This project presents a comparative study of different U-Net-based architectures for brain tumor segmentation from MRI scans. The study focuses on evaluating how different architectural improvements affect the segmentation of brain tumor regions.

## Models Evaluated

The following three architectures were implemented and compared:

- **3D U-Net**
- **Residual 3D U-Net**
- **U-Net 3+**

The models were evaluated using the **BraTS20** brain tumor segmentation dataset.

## Evaluation

Model performance was evaluated using three commonly used segmentation metrics:

- **Dice Score**
- **Jaccard Index**
- **mIoU**

These metrics were used to compare the ability of each architecture to accurately segment tumor regions in brain MRI scans.

## Results

U-Net 3+ achieved the strongest overall segmentation performance among the evaluated architectures. The comparison also showed how architectural improvements to the standard U-Net can affect segmentation quality in medical imaging tasks.

## Technologies

**TensorFlow** · **PyTorch** · **Medical Imaging** · **BraTS20**
