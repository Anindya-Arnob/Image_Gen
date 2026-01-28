# Image_Gen
# Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Anindya-Arnob/Image_Gen/blob/main/Img_gen_arc.ipynb)
# FLUX.2-Klein Image Generator (Colab Optimized)

An interactive Jupyter Notebook designed to run the **FLUX.2-klein-4B** model by Black Forest Labs. This tool features a built-in UI for easy prompt engineering and style selection, optimized for environments with limited VRAM (like Google Colab T4 GPUs).

## ✨ Features

* **Model:** Powered by `FLUX.2-klein-4B`, a lightweight yet high-quality diffusion model.
* **Interactive UI:** Built with `ipywidgets` for a seamless "enter prompt and click" experience.
* **Style Presets:** Includes 6 built-in art styles:
    * Realistic (8k, Cinematic)
    * 3D Cartoon (Pixar-style)
    * Studio Ghibli (Hand-drawn/Watercolor)
    * Neon Noir (Cyberpunk)
    * Oil Painting (Classical)
    * Pixel Art (16-bit retro)
* **Memory Optimization:** Uses `bitsandbytes` and `attention_slicing` to ensure it fits on a standard 16GB T4 GPU.

## 📝 Important Note on Memory

The notebook includes a `PYTORCH_CUDA_ALLOC_CONF` setting to manage memory fragmentation. If you encounter "Out of Memory" errors, try reducing the output `width` and `height` in the generation function (currently set to 512x1112 for mobile-portrait aspect ratios).

---
*Disclaimer: This project is for educational/creative purposes. Users are responsible for adhering to the license terms of the FLUX model family.*
