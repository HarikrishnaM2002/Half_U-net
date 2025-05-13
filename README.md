# Half-UNet for Multiclass Medical Image Segmentation

This repository implements a lightweight **Half-UNet** architecture in PyTorch for **multi-class semantic segmentation**, adapted for datasets such as liver and tumor segmentation with minimal GPU/memory overhead.

## 🚀 Overview

The project builds on insights from U-Net, UNet3+, and GhostNet, simplifying the decoder and using **full-scale feature fusion** and **Ghost modules** to reduce computational cost while maintaining performance.

## 🧠 Model Highlights

- ✅ Lightweight: Uses **Ghost modules** to reduce parameters and FLOPs.
- 🔁 Efficient full-scale **feature fusion via addition**, not concatenation.
- 🔥 Supports **3-class segmentation**: background, liver, tumor.
- 🧪 Includes **early stopping**, **checkpointing**, and **Dice score** evaluation.
- 🧰 Custom **data loader** and **augmentation pipeline** included.

---

## 📁 Dataset Structure

Place your dataset in the following structure:

project/
│

├── images/

│ ├── img_001.png

│ ├── ...

│

└── masks/

├── mask_001.png

├── ...

# Install dependencies
pip install -r requirements.txt
