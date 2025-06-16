# REU: Speech Copyright Detection and Deepfake Robustness via Adversarial Attacks on Watermarked Images
**Project Title:** Speech Copyright Detection and Deepfake Robustness via Adversarial Attacks on Watermarked Images

**Student Name:** Cat Lewin

**Mentor Name:** Dr. Rui Duan

**Problem Statements:** 

**Speech Copyright Detection**
This project examines the limitations of automated copyright detection systems by evaluating whether pure speech content can evade detection, thereby revealing potential vulnerabilities in existing enforcement mechanisms.

**Watermark Robustness in Deepfake Detection**
This project aims to examine the resilience and robustness of invisible image watermarks to adversarial manipulation, and their reliability in support of proactive deepfake detection.

# REU Week 3 – Cat Lewin

## 🔍 Project Overview
This repository documents two connected research explorations:
1. **Speech Copyright Detection** using YouTube’s Content ID system
2. **Adversarial Robustness of Invisible Watermarks** for deepfake detection

## 🧪 Experiments
- **Content ID Tests:** 10 audio-only video uploads tested for copyright claims
- **Watermarking:** Preparing to implement the Invisible Watermark framework (Zhang et al., 2019)

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
