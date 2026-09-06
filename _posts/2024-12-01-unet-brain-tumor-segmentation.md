---
layout: blog_post
title: "Comparative Analysis of U-Net Variants for Brain Tumor Segmentation"
date: 2025-01-02
github: "https://github.com/RAAFSAAN0/Brain-Tumor-Segmentation"
description: "A comparative study of 3D U-Net, Residual 3D U-Net, and U-Net 3+ for brain tumor MRI segmentation using the BraTS20 benchmark."
tags:
  - TensorFlow
  - PyTorch
  - Medical Imaging
  - BraTS20
---

## Overview

This project presents a comparative study of different U-Net-based architectures for brain tumor segmentation from MRI scans. The study focuses on evaluating how distinct architectural modifications and skip connections impact segmentation accuracy across complex tumor sub-regions.

## Models Evaluated

The following three architectures were implemented, trained, and benchmarked:

- **3D U-Net:** Baseline volumetric convolutional architecture.
- **Residual 3D U-Net:** Incorporates residual blocks to improve gradient propagation across deeper layers.
- **U-Net 3+:** Leverages full-scale skip connections and deep supervision to capture multi-scale semantic features.

All models were evaluated using the **BraTS20** brain tumor segmentation dataset.

## Evaluation Metrics

Model performance was validated using standard volumetric segmentation metrics:

- **Dice Similarity Coefficient (DSC)**
- **Jaccard Index (IoU)**
- **Mean Intersection over Union (mIoU)**

These metrics quantify the overlap and boundary precision between predicted tumor masks and expert ground-truth segmentations.

## Results

**U-Net 3+** achieved the strongest overall segmentation performance across all evaluated metrics, particularly on enhancing and core tumor regions. The results demonstrate that full-scale feature aggregation provides substantial precision gains over standard volumetric skip connections in medical image segmentation.

## Technologies

- **Frameworks:** TensorFlow, PyTorch
- **Domain:** Medical Image Analysis, Semantic Segmentation
- **Dataset:** BraTS 2020 Benchmark
