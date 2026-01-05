# UNET-A-Annotated-Guide

**Based on:**  
*U-Net: Convolutional Networks for Biomedical Image Segmentation*

**Authors:**  
Olaf Ronneberger, Philipp Fischer, Thomas Brox  

**Venue:**  
MICCAI (Medical Image Computing and Computer-Assisted Intervention)

---

## Table of Contents

1. [Abstract](#abstract)
2. [Background](#background)
3. [Challenges in Biomedical Image Segmentation](#challenges-in-biomedical-image-segmentation)
4. [Overview of U-Net Architecture](#overview-of-u-net-architecture)
5. [Key Breakthroughs of U-Net That Address Segmentation Challenges](#key-breakthroughs-of-u-net-that-address-segmentation-challenges)

6. [Model Architecture](#model-architecture)
   - [Double Convolution Layer](#double-convolution-layer)
   - [Contracting Path (Encoder)](#contracting-path-encoder)
   - [Expansive Path (Decoder)](#expansive-path-decoder)
   - [Skip Connections: Role and Function Within the Network](#skip-connections-role-and-function-within-the-network)
   - [Bottleneck (The Bridge)](#bottleneck-the-bridge)
   - [Final Layer: Purpose and Impact on Segmentation Output](#final-layer-purpose-and-impact-on-segmentation-output)
   - [Synthesis of Architecture: How All Parts Come Together](#synthesis-of-architecture-how-all-parts-come-together)

7. [Model Training](#model-training)
   - [Data Loading and Preprocessing for Model Training](#data-loading-and-preprocessing-for-model-training)
   - [Training Loop and Sub-Parts](#training-loop-and-sub-parts)
   - [Hyperparameter Tuning for GPU Configuration](#hyperparameter-tuning-for-gpu-configuration)

8. [Model Evaluation](#model-evaluation)
   - [Minimal Working Example (MWE – CPU)](#minimal-working-example-mwe--cpu)
   - [Evaluation with Adjusted U-Net Model](#evaluation-with-adjusted-u-net-model)

9. [Experiments and Results](#experiments-and-results)
   - [Output from the Adjusted Minimal Model Using CPU Under Partial Load](#output-from-the-adjusted-minimal-model-using-cpu-under-partial-load)
   - [Performance Metric Visualization for the Adjusted Minimal Model Using CPU Under Partial Load](#performance-metric-visualization-for-the-adjusted-minimal-model-using-cpu-under-partial-load)
   - [Output from the Original Model Using GPU Under Full Load](#output-from-the-original-model-using-gpu-under-full-load)
   - [Performance Metric Visualization for the Adjusted Minimal Model Using GPU Under Full Load](#performance-metric-visualization-for-the-adjusted-minimal-model-using-gpu-under-full-load)

10. [Observed Limitations of CPU Training](#observed-limitations-of-cpu-training)
11. [Limitations and Weaknesses of U-Net](#limitations-and-weaknesses-of-u-net)

