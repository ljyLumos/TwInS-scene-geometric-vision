# TwInS: Two-Stream Interactive Joint Learning for Scene Parsing and Geometric Vision

## Overview
This project explores the interaction between scene parsing and geometric vision tasks, including semantic segmentation, instance segmentation, stereo matching, and optical flow.  
The goal is to improve task performance by enabling bidirectional interaction between semantic context and geometric correspondence.

## Motivation
Traditional multi-task learning approaches often share a single encoder across tasks or use unidirectional feedback, limiting cross-task information exchange.  
TwInS introduces a **two-stream interactive framework** to enhance mutual guidance between tasks.

## Method
- **Scene Parsing Stream**: Provides semantic context and instance-level features.
- **Geometric Vision Stream**: Predicts stereo and optical flow correspondences.
- **Cross-Task Adapter**: Bridges hidden states from the geometric stream to the parsing stream for iterative refinement.

## My Contributions
- Conducted benchmark evaluation and visualization analysis across multiple models, including DFormerv2
- Experimentally validated the effectiveness of the Cross-Task Adapter for feature fusion.
- Analyzed quantitative improvements in scene parsing performance.

## Results
- **Semantic Segmentation:** The two-stream interactive framework improved semantic segmentation performance on Cityscapes, vKITTI2, and KITTI 2015 datasets, achieving up to **7.23% improvement in mIoU**.
- **Instance Segmentation:** Instance-level segmentation metrics improved up to **13.64% mAP**, demonstrating effective cross-task feature fusion.
- **Visualization Analysis:** Generated qualitative visualizations showing clearer object boundaries and better alignment of segmentation with geometric features.
- **Cross-Task Adapter Validation:** Experiments confirmed that the adapter effectively enhances interaction between scene parsing and geometric vision streams.

## Assets
![Framework](assets/framework.png)
![Qualitative Results](assets/qualitative_results.png)

## Notes on Code Availability
The full code is under internal collaboration review.  
This repository provides a structured overview, visual results, and detailed report for project evaluation.

## Keywords
Scene Parsing · Geometric Vision · Multi-task Learning · Stereo Matching · Optical Flow · Semantic Segmentation · Instance Segmentation

## Related Materials
- [Project Report](docs/report.pdf)
