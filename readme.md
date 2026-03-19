# GAN Image Generation on Fashion-MNIST

## Technical Skillset
Python  
PyTorch  
GANs (DCGAN, WGAN-GP, cGAN)  
Generative Modelling  
Wasserstein Loss  
Gradient Penalty  
Conditional Generation  
MiFID Evaluation  
Training Stability Analysis  
Model Iteration and Diagnostics  
NumPy  
Matplotlib  
Torchvision  
Reproducible ML Pipelines  

## Project Description

This project implements and evaluates three generative adversarial networks (DCGAN, WGAN-GP, and cGAN) on the Fashion-MNIST dataset. The work demonstrates iterative model development, where each version introduces a principled architectural or objective-function improvement to address instability, mode imbalance, and lack of controllability.

The project highlights practical deep learning engineering skills including GAN training, gradient penalty implementation, conditional generation, MiFID evaluation, and systematic experimentation. It reflects real-world workflows used in generative modelling research and production ML environments.

## Project Overview

### Objective
Investigate how architectural and loss-function choices affect training stability, generative fidelity, and class-specific controllability in GAN-based image synthesis.

### Dataset
Fashion-MNIST  
- 70,000 grayscale images  
- 10 clothing categories  
- Resized to 64x64  
- Normalised to [-1, 1]  

## Iterative Model Development

### Iteration 1: DCGAN (Baseline)
- Standard BCE adversarial loss  
- Transposed convolutions for upsampling  
- Exhibited instability, mode imbalance, and blurry textures  
- Served as a baseline reference  

### Iteration 2: WGAN-GP
- Replaced BCE with Wasserstein-1 distance  
- Added gradient penalty for Lipschitz constraint  
- Achieved the best training stability  
- Produced the lowest MiFID score and sharpest samples  

### Iteration 3: cGAN
- Added label conditioning to generator and discriminator  
- Enabled explicit class control  
- Improved structural consistency  
- Higher MiFID score due to reduced global distribution alignment  

## Key Contributions

- Implemented DCGAN, WGAN-GP, and cGAN architectures from scratch in PyTorch  
- Added gradient penalty for stable Wasserstein training  
- Designed conditional generation using label embeddings  
- Built reproducible training loops with fixed seeds  
- Generated visual grids and saved sample images for evaluation  
- Computed MiFID scores for quantitative comparison  
- Performed detailed analysis of stability, fidelity, and controllability  

## Results Summary

- WGAN-GP achieved the best overall generative fidelity and stability  
- cGAN enabled strong class-specific control  
- DCGAN provided a useful baseline but showed instability and blur  
- MiFID scores and qualitative grids confirmed the progression across iterations  

## Project Tags

gan, dcgan, wgan-gp, cgan, generative-models, pytorch, fashion-mnist, image-generation, mifid, deep-learning, visual-computing

## Contact

For questions or collaboration, feel free to reach out.