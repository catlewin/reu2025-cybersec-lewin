# REU: Deepfake Robustness via Adversarial Attacks on Watermarked Images
**Project Title:** Speech Copyright Detection and Deepfake Robustness via Adversarial Attacks on Watermarked Images

**Student Name:** Cat Lewin

**Mentor Name:** Dr. Rui Duan

**Problem Statement:** 

**Watermark Robustness in Deepfake Detection**
This project aims to examine the resilience and robustness of invisible image watermarks to adversarial manipulation, and their reliability in support of proactive deepfake detection.

# REU Week 5–6 - Cat Lewin

**Project Summary** During Weeks 5 and 6 of the REU program, the project focused on evaluating the robustness of invisible watermarking methods against a variety of adversarial image attacks. Three watermarking techniques were tested: DWT-DCT, DWT-DCT-SVD, and RivaGAN. A threshold-based evaluation framework was implemented to determine the attack severity at which each method fails to decode embedded watermarks.

In Week 6, the pipeline was extended with perceptual similarity analysis using the LPIPS metric (AlexNet backbone) to assess how visually imperceptible attacks can still disrupt watermark integrity. The combined evaluation—decode success plus LPIPS score—helps identify particularly dangerous transformations that evade human detection but break watermarking.

In parallel, the functional codebase and full set of results were maintained on a public repository:

🔗 [invisible-watermark-cat GitHub Repository](https://github.com/catlewin/invisible-watermark-cat)

The project is now positioned to test robustness against generative model–based attacks and to explore extensions using diffusion models and transformers.


# REU Week 4 – Cat Lewin

**Project Summary** Three watermarking approaches were implemented and evaluated:

- DWT-DCT
- DWT-DCT-SVD
- RivaGAN


## Key Contributions

Reproduced baseline (ShieldMnt) neural watermarking model

Implemented classical frequency-based watermarking approaches

Evaluated against JPEG, crop, rotate, noise, and more

## Baseline Reproduction: Invisible Watermark (ShieldMnt)

This project includes a partial reproduction of the Invisible Watermark framework, which provides a CNN-based encoder-decoder architecture for embedding and decoding imperceptible watermarks in images.

[ShieldMnt GitHub repository](https://github.com/ShieldMnt/invisible-watermark)

The reproduction focuses on:

- Running the provided model on a clean test image
- Applying adversarial attacks (e.g., JPEG, resize, crop, noise)
- Measuring bitwise decode accuracy and perceptual similarity

_Note: All code and models for this reproduction were adapted from the original ShieldMnt GitHub repository, accessed in June 2025._

# REU Week 3 – Cat Lewin

## 🔍 Project Overview
This repository documents two connected research explorations:
1. **Speech Copyright Detection** using YouTube’s Content ID system
2. **Adversarial Robustness of Invisible Watermarks** for deepfake detection

## 🧪 Experiments
- **Content ID Tests:** 10 audio-only video uploads tested for copyright claims
- **Watermarking:** Preparing to implement the Invisible Watermark framework (Zhang et al., 2019)

## Outputs

This folder contains experimental visuals and screenshots for both phases of the research.

## Speech Copyright Detection
- Screenshots of YouTube’s Content ID results for MLK and Joker speech tests
- Summary results table of 10 uploaded clips and corresponding claims
- Flowchart diagram of the audio-only testing methodology

## Watermark Robustness
- Visual pipeline for the proposed adversarial attack setup using Invisible Watermark


## 📁 Folder Structure
- `reports/`: Final PDF report
- `slides/`: Week 3 presentation
- `notebooks/`: Experimental logs and setup plans
- `outputs/`: Screenshots and tables from experiments

## 📎 Reproduced Work
- Attempted implementation of [LampMark](https://github.com/wangty1/LampMark) (paused)
- Baseline moving forward: [Invisible Watermark](https://github.com/ShieldMnt/invisible-watermark)

## ⚙️ Setup Instructions
_Note: Watermarking experiments pending setup_
```bash
git clone https://github.com/ShieldMnt/invisible-watermark
cd invisible-watermark
pip install -r requirements.txt
# Training instructions to follow
