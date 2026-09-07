---
layout: blog_post
title: "Behavioral and Explanation Instability of ResNet-50 Under Progressive Image Corruption"
date: 2026-03-01
tags: [PyTorch, Deep Learning, Computer Vision, Model Robustness, Explainable AI, Grad-CAM]
github: "https://drive.google.com/file/d/1R8HtH83uMluAxAaiHLqOZMQnsFbZ4mN_/view?usp=sharing"
description: "Evaluated an ImageNet-pretrained ResNet-50 across 75 corruption-severity conditions on CIFAR-10-C to detect early warning signals of accuracy failure using output distribution changes and Grad-CAM explanation instability."
---

## Overview

High classification accuracy on clean benchmarks does not guarantee reliability when models encounter real-world corruptions such as noise, blur, weather effects, and compression artifacts. In this study, we investigate how an ImageNet-pretrained **ResNet-50** behaves as image corruption becomes progressively more severe across the **CIFAR-10-C** benchmark (covering 15 corruption types and 5 severity levels).

Rather than treating model failure as a single event, we analyze output-level behavioral shifts—such as confidence change, prediction flip rates, and Jensen–Shannon divergence—alongside Grad-CAM spatial explanation instability to determine whether output signals can provide an early warning before performance significantly degrades.

---

## Key Highlights & Contributions

* **Comprehensive Benchmark Evaluation:** Evaluated ResNet-50 across 75 corruption–severity conditions (15 corruption types × 5 severity levels) on CIFAR-10-C.
* **Early Warning Detection:** Quantified how output-level signals change prior to accuracy drops. Behavioral instability measured via Jensen–Shannon divergence provided an early warning for **9 of 15 corruption types**, with an average lead of **2 severity levels** before model accuracy fell below 80%.
* **Explanation Instability:** Measured spatial evidence shift using Grad-CAM Intersection-over-Union (IoU) between clean and corrupted inputs, revealing a significant increase in mean instability from **0.1840 to 0.3339** as corruption increased.
* **Performance Impact:** Tracked a steep drop in overall classification accuracy from **97.53%** on clean images down to **64.16%** at the highest corruption severity level.

---

## Methodology & Metrics

1. **Confidence & Flip Rate:** Measured changes in top-1 maximum Softmax probabilities and the frequency at which corruption caused the predicted class to flip.
2. **Behavioral Instability (JSD):** Utilized Jensen–Shannon Divergence across full Softmax output distributions between clean and corrupted image pairs to capture subtle distributional shifts that top-1 accuracy misses.
3. **Grad-CAM Stability:** Evaluated spatial saliency map overlap (IoU) to observe how feature relevance maps destabilize under noise and atmospheric perturbations.

---

## Manuscript & Resources

* **Full Paper / Manuscript:** [Read the PDF on Google Drive](https://drive.google.com/file/d/1R8HtH83uMluAxAaiHLqOZMQnsFbZ4mN_/view?usp=sharing)
