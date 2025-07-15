# Day 16 — TensorFlow

**Date:** July 14, 2025

---

## Overview

Today’s focus was on **TensorFlow**, Google’s open-source framework for building and deploying **Machine Learning (ML)** and **Deep Learning (DL)** models at scale.  
TensorFlow makes it easy to design, train, convert, optimize, and run ML models across devices — from powerful servers to mobile and embedded systems.

---

## Key Concepts

- **What is TensorFlow?**
  - Developed by Google Brain for scalable ML & AI.
  - Supports NLP, Computer Vision, Time Series, Reinforcement Learning.

- **Key Features:**
  - **Scalability:** From PC to mobile, embedded devices.
  - **Ecosystem:** TensorFlow Core, Keras, TFLite, TensorFlow.js, TFX, TensorFlow Hub.
  - **Autograd:** Automatic differentiation for backpropagation.
  - **Multi-language Support:** Python, C++, Java, JavaScript.
  - **Model Serving & Optimization:** Tools for efficient deployment & serving.

---

## Typical TensorFlow Workflow

1️ **Train a Model**  
- Build & train with TensorFlow or Keras.  
- Use relevant datasets, validate for high accuracy.

2️ **Convert the Model**  
- Use **TFLite Converter** to produce `.tflite` files for edge devices.

3️ **Optimize the Model**  
- Apply quantization, pruning, weight clustering to reduce size and speed up inference.

4️ **Deploy the Model**  
- Deploy `.tflite` models on Android, iOS, Raspberry Pi, microcontrollers.

5️ **Run Inference**  
- Use **TensorFlow Lite Interpreter** for real-time predictions offline on the edge.

---

## Files

- `Day16.pdf` — Detailed notes on TensorFlow features, workflow & tools.

---

## Next Steps

- Build a simple TensorFlow/Keras model.
- Convert it to `.tflite` and test on a mobile device or Raspberry Pi.
- Try TensorFlow.js to run models in a web browser.

---

> **"TensorFlow lets you build AI that runs everywhere — from servers to sensors."**

