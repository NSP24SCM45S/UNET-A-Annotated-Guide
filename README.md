# UNET-A-Annotated-Guide

Based on: U-Net: Convolutional Networks for Biomedical Image Segmentation

By :- Olaf Ronneberger, Philipp Fischer, Thomas Brox

Venue :- MICCAI (Medical Image Computing and Computer-Assisted Intervention)

Table of Contents
Abstract
Background
Challenges in biomedical image segmentation
Overview of U-Net architecture
Key breakthroughs of U-Net that address segmentation challenges
Model Architecture
Double Convolution Layer
Contracting Path (Encoder):
Expansive Path (Decoder):
Skip Connections: Role and function within the network
Bottleneck:(The Bridge)
Final Layer: Purpose and impact on segmentation output
Synthesis of Architecture: How All Parts Come Together
Model Training
Data Loading and Preprocessing for Model Training
Training Loop and Sub-Parts
Hyperparameter Tuning for GPU config
Model Evaluation
Minimal Working Example (MWE-CPU)
Evaluation with adjusted U-Net Model
Experiments and Results
Output from the adjusted minimal model using CPU under partial load
Performance metric visualisaton for the adjusted minimal model using CPU under partial load
Output from the original model using GPU under full load
Performance metric visualisaton for the adjusted minimal model using GPU under full load
Observed Limitations of CPU training
Limitations and Weaknesses of U-Net
