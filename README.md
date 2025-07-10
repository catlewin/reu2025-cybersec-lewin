# REU: NSF REU 2025 – AI-Enabled Cybersecurity Research
**Project Title:** Watermark Robustness under Adversarial Attacks for Deepfake Detection

**Student Name:** Cat Lewin - University of Missouri-Kansas City

**Mentor Name:** Dr. Rui Duan

GitHub (complete watermark evaluation repository): [invisible-watermark-cat](https://github.com/catlewin/invisible-watermark-cat)

## Project Overview

**Watermark Robustness in Deepfake Detection**
This project focuses on evaluating the **robustness of invisible watermarking techniques** against a wide range of adversarial attacks with the goal of to building a systematic framework for testing how well watermarking methods like **DWT-DCT**, **DWT-DCT-SVD**, and **RivaGAN** can withstand both traditional and perceptual-based attacks. We also explore perceptual distortion using **LPIPS** and investigate emerging attack methods including denoising, rescaling, and embedding-based watermark removal.


## Progress Summary

### Week 2–3:
- Explored initial idea around speech-based deepfake detection using YouTube’s Content ID system.
- Found limitations with Content ID not reliably flagging speech-only content.

### Week 4–5:
- Pivoted to invisible watermarking.
- Implemented and tested 3 methods: DWT-DCT, DWT-DCT-SVD, and RivaGAN.
- Designed 8 threshold-based attacks (e.g., crop, brightness, resize, rotate).
- Built robustness pipeline with automated summary generation.

### Week 6:
- Integrated LPIPS perceptual metric.
- Analyzed relationship between LPIPS and watermark decode failures.
- Created plots and summary tables across methods and attack types.

### Week 7:
- Drafted poster and updated conceptual diagram.
- Added two new attack tests: **denoising** (NAFNet) and **rescaling** (image-super-resolution).
- Started integrating findings into final poster and paper.

## Future Work
- Evaluate traditional watermarking tool [OpenStego](https://github.com/syvaidya/openstego)
- Test advanced watermark attack [WatermarkAttacker](https://github.com/XuandongZhao/WatermarkAttacker)
- Consider hybrid attacks, deepfake models, and AI explainability integration

## Acknowledgments
This project is supported by the NSF REU Program at the University of Missouri–Kansas City. Special thanks to Dr. Fengjun Li and Dr. Yajin Duan for their mentorship.
