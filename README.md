# Assignment 3: Denoising Diffusion Probabilistic Model

## Objective:
Implemented a Denoising Diffusion Probabilistic Model (DDPM) for denoising MNIST data, based on the paper "Denoising Diffusion Probabilistic Models" by Jonathan Ho, Ajay Jain, and Pieter Abbeel from UC Berkeley ([arXiv:2006.11239v2](https://arxiv.org/abs/2006.11239v2)).

## Tasks Completed:

1. **Model Initialization:**
   - Implemented the `__init__` function in the `MNISTDiffusion` class.
   - Initialized the UNet model using the provided `_cosine_variance_schedule` function.

2. **Forward Diffusion:**
   - Utilized the reparameterization trick for the forward pass.
   - Implemented the `forward` and `_forward_diffusion` functions.
   - Sampled `t` uniformly from the timesteps for each training sample.

3. **Reverse Diffusion:**
   - Implemented reverse diffusion using trainable mean and variance parameters from the UNet model.
   - Developed the `_reverse_diffusion` function.

4. **Image Sampling:**
   - Implemented the sampling procedure.
   - Developed the `sampling` function to generate noise and run reverse diffusion for each sample.
   - Returned the entire trajectory of samples.

5. **Model Training:**
   - Selected hyperparameters such as learning rate, batch size, epochs, and timesteps.
   - Chose optimizer, loss function, and learning rate scheduler.
   - Displayed 36 final samples using provided code.

## Additional Tasks:
- Visualized a sample diffusion trajectory demonstrating noise turning into a clean sample.
- Labeled each image with corresponding denoising step.
- Ensured code is well-documented and organized for reproducibility.

**Note:** Please refer to the provided code and documentation for detailed implementation and explanations.
