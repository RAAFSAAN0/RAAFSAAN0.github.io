---
layout: blog_post
title: 'Comparative Analysis of U-Net Variants for Brain Tumor Segmentation'
date: 2025-01-02
tags:
  - TensorFlow
  - PyTorch
  - Medical Imaging
  - BraTS20
---

This project presents a comparative study of 3D U-Net, Residual 3D U-Net, and U-Net 3+ for brain tumor segmentation using the BraTS20 brain MRI dataset. The models were evaluated using Dice, Jaccard, and mIoU metrics, with U-Net 3+ achieving the strongest overall segmentation performance among the evaluated architectures.

# Overview

This project focuses on the comparative analysis of three U-Net-based deep learning architectures for brain tumor segmentation from MRI scans. The study examines how different architectural designs affect segmentation performance on the BraTS20 dataset.

# Models Evaluated

The following architectures were implemented and compared:

- **3D U-Net**
- **Residual 3D U-Net**
- **U-Net 3+**

# Evaluation

Model performance was evaluated using three segmentation metrics:

- **Dice Score**
- **Jaccard Index**
- **mIoU**

These metrics were used to assess how accurately each model segmented tumor regions in brain MRI scans.

# Results

Among the evaluated architectures, **U-Net 3+ achieved the strongest overall segmentation performance**. The comparison demonstrates the impact of architectural improvements and multi-scale feature aggregation on medical image segmentation.

# Technologies

**TensorFlow** · **PyTorch** · **Medical Imaging** · **BraTS20**
