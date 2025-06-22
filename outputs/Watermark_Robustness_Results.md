# 🔬 Watermark Robustness Test Summary

This table summarizes the decoding results for each attack across the three watermarking methods: `dwtDct`, `dwtDctSvd`, and `rivaGan`.

| **Attack**              | **Image**                                                                                                         | **dwtDct**               | **dwtDctSvd**            | **rivaGan**        |
|-------------------------|--------------------------------------------------------------------------------------------------------------------|---------------------------|---------------------------|--------------------|
| No Attack               | ![No_Attack](https://github.com/user-attachments/assets/73edfef0-dee4-4620-a327-f533f6dd8d19)                     | ✅ `qingquan`             | ✅ `qingquan`             | ✅ `qing`          |
| JPEG Compression (Q=40) | ![JPEG_Compression_Q_40](https://github.com/user-attachments/assets/f46f92cc-84b2-4d3a-87f2-534263abd6fb)          | ❌ `\x00\x00\x00\x00@\x00` | ❌ `P\x00\x00\x03 0 $`     | ✅ `qing`          |
| Resize (50%)            | ![Resize_50_](https://github.com/user-attachments/assets/3c777ab0-6a53-4028-a491-23303c248a14)                    | ✅ `qingquan`             | ✅ `qingquan`             | ✅ `qing`          |
| Gaussian Noise (std=5)  | ![Gaussian_Noise_std_5](https://github.com/user-attachments/assets/fbf38aac-af41-4a26-bcaa-863829d5ef73)          | ✅ `qingquan`             | ✅ `qingquan`             | ✅ `qing`          |
| Crop (7x5%)             | ![Crop_7x5_](https://github.com/user-attachments/assets/2558cb1f-eb8a-4501-abf8-22ce7b16779f)                     | ❌ `[UTF-8 Error]`        | ❌ `[UTF-8 Error]`        | ✅ `qing`          |
| Brightness ×1.2         | ![Brightness_x1_2](https://github.com/user-attachments/assets/35f0d23f-f284-4593-a127-d681248ea263)               | ✅ `qingquan`             | ❌ `[UTF-8 Error]`        | ✅ `qing`          |
| Overlay (Smiley)        | ![Overlay_Smiley](https://github.com/user-attachments/assets/132ef030-9cb5-4375-b4e4-73530a4c90a3)                | ✅ `qingquan`             | ✅ `qingquan`             | ✅ `qing`          |
| Mask (20%)              | ![Mask_20_](https://github.com/user-attachments/assets/916188af-5911-4140-b1a8-e5b1bd4f8178)                      | ✅ `qingquan`             | ✅ `qingquan`             | ✅ `qing`          |
| Rotate (30°)            | ![Rotate_30](https://github.com/user-attachments/assets/fd813fd6-79c7-4082-94ac-5dccb7ba43c8)                     | ❌ `[UTF-8 Error]`        | ❌ `\x00\x00\x00\x00\x00\x02` | ❌ `[UTF-8 Error]` |


Legend:

* ✅: Exact match with expected watermark.
* ❌: Failure or decoding error.
* UTF-8 Error indicates corrupted or malformed decoding.

> Note: `rivaGan` only supports 32-bit watermarks, which is why its decoded string is shorter (`qing` instead of `qingquan`).
