# 🔐 Watermarking Notebooks

This folder contains early code and notebooks used to replicate baseline watermarking methods and adversarial attacks as described in the ShieldMnt/invisible-watermark repository.

## 📁 Files

- `main.py`: Run full pipeline for watermark embedding, distortion, and decoding
- `watermark_utils.py`: Utility functions used across all methods

## ⚠️ Dependencies

Some functions rely on modules from the [ShieldMnt/invisible-watermark](https://github.com/ShieldMnt/invisible-watermark) repository.

To run these locally:

```bash
git clone https://github.com/ShieldMnt/invisible-watermark.git
cd invisible-watermark
pip install -r requirements.txt
