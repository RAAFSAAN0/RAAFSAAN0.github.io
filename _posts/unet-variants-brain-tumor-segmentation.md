---

layout: blog_post
title: "Comparative Analysis of U-Net Variants for Brain Tumor Segmentation"
date: 2025-01-02
tags:

* TensorFlow
* PyTorch
* Medical Imaging
* BraTS20
  excerpt: "A comparative study of 3D U-Net, Residual 3D U-Net, and U-Net 3+ for brain tumor segmentation using the BraTS20 dataset, evaluated with Dice, Jaccard, and mIoU metrics."

---

## Overview

This project presents a comparative analysis of different U-Net-based architectures for brain tumor segmentation from MRI scans. The study investigates the performance of **3D U-Net, Residual 3D U-Net, and U-Net 3+** using the **BraTS20** dataset.

The models were evaluated using **Dice Score, Jaccard Index, and mean Intersection over Union (mIoU)** to compare their segmentation performance. Among the evaluated architectures, **U-Net 3+ achieved the strongest overall performance**.

## Models Evaluated

The following three architectures were implemented and compared:

* **3D U-Net**
* **Residual 3D U-Net**
* **U-Net 3+**

## Evaluation

Model performance was evaluated using:

* **Dice Score**
* **Jaccard Index**
* **mIoU**

These metrics were used to measure how accurately each architecture segmented tumor regions from brain MRI scans.

## Results

The experimental comparison showed that **U-Net 3+ achieved the strongest segmentation performance** among the evaluated architectures. The results demonstrate the potential benefits of incorporating enhanced feature aggregation and multi-scale information into U-Net-based segmentation architectures.

## Technologies

**TensorFlow** · **PyTorch** · **Medical Imaging** · **BraTS20**
