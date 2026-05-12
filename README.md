# 🎨 FLUX.2-Klein Image Generator

> AI-powered image generation with 6 artistic style presets —
> run entirely in Google Colab on a free T4 GPU.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Anindya-Arnob/Image_Gen/blob/main/Img_gen_arc.ipynb)
![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-Diffusers-yellow?style=for-the-badge&logo=huggingface&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Colab](https://img.shields.io/badge/Google%20Colab-T4%20GPU-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![License](https://img.shields.io/badge/License-Educational-brightgreen?style=for-the-badge)

---

## 📌 Overview

An AI image generation notebook powered by `black-forest-labs/FLUX.2-klein-4B`,
optimized to run smoothly on **free T4 GPUs** using 4-bit quantization and
attention slicing. Features an interactive UI with 6 built-in artistic style
presets for real-time prompt engineering.

---

## ✨ Key Features

- ⚡ **Optimized for Free GPUs** — 4-bit quantization via `bitsandbytes` +
  attention slicing fits the 4B model into Colab's free T4 VRAM
- 🎨 **6 Style Presets** — switch artistic styles with one click
- 🖥️ **Interactive UI** — built with `ipywidgets`, no external framework needed
- 🔤 **Real-time Prompt Engineering** — live text input with style augmentation
- 🖼️ **Portrait-Optimized Output** — default `512×1112` resolution

---

## 🎨 Style Presets

| Style | Description |
|-------|-------------|
| 🌄 Realistic | Photorealistic output |
| 🧊 3D Cartoon | Stylized 3D render look |
| 🌿 Studio Ghibli | Soft anime-inspired aesthetic |
| 🌆 Neon Noir | Dark cyberpunk atmosphere |
| 🖼️ Oil Painting | Classical painterly texture |
| 👾 Pixel Art | Retro 8-bit game style |

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| **Image Generation** | Diffusers, FLUX.2-Klein-4B, bitsandbytes |
| **Deep Learning** | PyTorch, Transformers, Accelerate |
| **UI** | ipywidgets |
| **Runtime** | Google Colab (T4 GPU) |
| **Language** | Python 3.10+ |

---

## 🚀 Quick Start

### Step 1 — Open in Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Anindya-Arnob/Image_Gen/blob/main/Img_gen_arc.ipynb)

> ⚠️ Set **Runtime → Change runtime type → T4 GPU** before running.

### Step 2 — Get a Hugging Face Token

1. Visit [huggingface.co](https://huggingface.co) and sign in
2. Go to **Profile → Settings → Access Tokens**
3. Click **"New token"** → name it `Colab` → set role to **Read**
4. Visit the [FLUX.1-schnell model page](https://huggingface.co/black-forest-labs/FLUX.1-schnell)
   and click **"Agree and access repository"** to accept the license

### Step 3 — Generate
