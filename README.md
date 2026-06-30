# GAN-Based Image Generation and Image-to-Image Translation
The report file consist of most of the information about the implementation.

This repository contains the implementation of two Generative AI lab tasks using PyTorch:

1. **Task 1:** GAN-based fruit image generation and classification comparison using real vs. synthetic data.
2. **Task 2:** Image-to-image translation using supervised Pix2Pix and unsupervised CycleGAN.

The main objective is to understand how GAN-generated data performs compared with original data, and how supervised and unsupervised image translation models differ in quality, training cost, and practical usefulness.

---

## Project Overview

This project explores two important applications of Generative Adversarial Networks:

### Task 1: Fruit Image Generation Using AC-GAN

An **Auxiliary Classifier GAN (AC-GAN)** is implemented from scratch to generate fruit images for three classes:

- Apple
- Banana
- Orange

After generating synthetic fruit images, a custom CNN classifier is trained and evaluated under different scenarios:

- Training only on original real images
- Training only on GAN-generated synthetic images
- Comparing classification accuracy and training time
- Studying how different amounts of data affect model accuracy and computational cost

### Task 2: Satellite-to-Map Image Translation

Two image-to-image translation models are implemented and compared:

- **Pix2Pix** — supervised image-to-image translation using paired satellite-map images
- **CycleGAN** — unsupervised image-to-image translation using unpaired domain translation logic

Both models are evaluated visually and quantitatively using:

- PSNR
- SSIM
- FID
- Training time
- Model size

---

## Repository Files

```text
.
├── Fruite.zip
├── task1-3(1) (1).ipynb
├── task2 (1).ipynb
├── GenAI_Lab1_Report_revised (1).pdf
└── README.md


Task 1. Use GAN to implement the image generator and compare the performance of the model trained on synthesized data versus non-synthesized data.

Implement data generator for given classes data (transfer learning is not allowed). Evaluate its performance.
Implement and train a classification model to categorize images. Evaluate the classification model's performance when trained on:
Only original data.
Only synthesized data.
(optional) non-generative algorithms are used for data augmentation.
Perform analysis regarding amount of given data in accuracy of classification results and computational time (use different amount of data, to get the pattern, how models accuracy depends in different training scenarios).

Task 2. Implement Image to Image translation and compare results for different types of solutions.

Implement supervised learning approach (Pix2PixHD, Pix2Pix, ...) for image generation for provided dataset and problem (transfer learning is not allowed). Describe the model used, the training process, and the results.
Implement unsupervised learning approach (CycleGAN, ...) for image generation for provided dataset and problem (transfer learning is not allowed). Describe the model used, the training process, and the results.
Perform results analysis and evaluation of both supervised and unsupervised techniques: Analyze the generated images visually and quantitatively (e.g., FID, SSIM, PSNR). Compare computational efficiency (e.g., training time, model size).
