# Image_Gen
# Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Anindya-Arnob/Image_Gen/blob/main/Img_gen_arc.ipynb)
# FLUX.2-Klein Image Generator & Watermarker
This repository features an optimized implementation of the FLUX.2-klein-4B model. It combines a high-quality image generation UI with a sophisticated DWT-based watermarking system for digital asset protection.

# ✨ Key Features
1. Advanced Image Generation: Powered by black-forest-labs/FLUX.2-klein-4B, utilizing bitsandbytes and attention_slicing to run smoothly on standard T4 GPUs.
2. Interactive Arc UI: A built-in interface using ipywidgets allows for real-time prompt engineering and style selection.
3. Time-Bound Watermarking: A specialized security feature that embeds a cryptographic "time-stamp" into images.
4. DWT Embedding: Uses Discrete Wavelet Transform (Haar) to hide metadata in the frequency domain.
5. Cryptographic Verification: Combines a secret key with a UNIX timestamp and SHA-256 hashing for secure detection.
6. Style Presets: Toggle between Realistic, 3D Cartoon, Studio Ghibli, Neon Noir, Oil Painting, and Pixel Art.

# 🛠️ Installation
The notebook automates the environment setup, including:
Core AI Libraries: diffusers, transformers, accelerate.
Image Processing: opencv-python, pywavelets, numpy.

# 🚀 Quick Start
Open in Colab: Click the badge above to launch the environment.
Authentication: Run the login cell and provide your Hugging Face token.

Generate:
Enter your prompt in the Textarea.
Choose a style and click Generate Image.
Protect: Run the Watermark section to embed a secret key and timestamp into your generated output.

# 📝 Technical Notes
VRAM Management: The notebook sets PYTORCH_CUDA_ALLOC_CONF to expandable_segments:True to prevent memory fragmentation on Colab.
Output Dimensions: Default generation is set to 512x1112 for portrait-style results.
Watermark Sensitivity: The detection threshold is set to 0.08 by default to balance robustness and accuracy.

Disclaimer: This project is for educational/creative purposes. Users are responsible for adhering to the license terms of the FLUX model family.
