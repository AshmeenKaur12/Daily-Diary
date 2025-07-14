# Llama 3 on Ubuntu — Setup Guide

**Date:** July 11, 2025  
**Document:** Day15 11-07-2025.pdf

---

## Overview

**Llama 3**, Meta’s latest open-source AI model, is a flexible, high-performance large language model for tasks like NLP, chatbots, and more. This guide explains how to set up and run **Llama 3** on **Ubuntu** using **Ollama**.

---

## Prerequisites

- **GPU:** Nvidia GPU with **8GB VRAM** minimum (**12GB+ recommended**)
- **OS:** Ubuntu **20.04** or similar Linux distro
- **Python:** 3.8 or newer
- **CUDA:** Nvidia CUDA toolkit installed & configured

---

## Steps to Install and Run

### 1️ Update Your System

```bash
sudo apt update && sudo apt upgrade -y
```
Install curl:
```bash
sudo apt install curl
```
