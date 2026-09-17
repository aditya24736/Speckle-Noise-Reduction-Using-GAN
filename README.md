# 🩺 Speckle Noise Reduction Using Generative Adversarial Networks

> A deep learning-based approach for reducing speckle noise in ultrasound images using Generative Adversarial Networks (GANs).

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red?logo=keras)](https://keras.io/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![Computer Vision](https://img.shields.io/badge/Domain-Computer%20Vision-green)]()
[![Medical Imaging](https://img.shields.io/badge/Domain-Medical%20Imaging-purple)]()

---

## 📌 Overview

Ultrasound imaging is widely used because it is non-invasive, relatively inexpensive, and provides real-time imaging. However, ultrasound images are commonly affected by **speckle noise**, which can reduce image quality and make important anatomical structures more difficult to analyze.

This project explores the use of **Generative Adversarial Networks (GANs)** for ultrasound image denoising. The model consists of two neural networks:

- **Generator** – learns to generate a cleaner version of a noisy ultrasound image.
- **Discriminator** – attempts to distinguish between real images and generated images.

Through adversarial training, the generator learns to produce increasingly realistic and visually improved images.

---

## 🎯 Objectives

The main objectives of this project are:

- Reduce speckle noise present in ultrasound images.
- Improve the visual quality of ultrasound images.
- Explore GANs for medical image denoising.
- Train a generator to produce denoised images.
- Use a discriminator to improve the quality of generated images.
- Evaluate the generated images using **PSNR** and **SSIM**.
- Investigate the potential of deep learning for ultrasound image enhancement.

---

## 🧠 Methodology

The overall workflow of the project is:

```text
Ultrasound Images
       │
       ▼
Data Preparation
       │
       ▼
Data Augmentation
       │
       ▼
Noisy Ultrasound Images
       │
       ▼
   ┌───────────────┐
   │    Generator  │
   └───────┬───────┘
           │
           ▼
   Denoised / Generated
        Image
           │
           ▼
   ┌───────────────┐
   │ Discriminator  │
   └───────┬───────┘
           │
           ▼
   Adversarial Training
           │
           ▼
   Improved Generator
           │
           ▼
     Denoised Image
           │
           ▼
      PSNR / SSIM
