# viton-hd-custom-inference-pipeline
An end-to-end virtual try-on pipeline using the VITON-HD framework, integrated with U-2-Net for cloth mask generation, SCHP for human image parsing, and OpenPose for pose estimation. This notebook-driven project supports custom image inputs and outlines a step-by-step process to test VITON-HD on your own data.

# Link:-
Checkpoints - https://drive.google.com/drive/folders/0B8kXrnobEVh9fnJHX3lCZzEtd20yUVAtTk5HdWk2OVV0RGl6YXc0NWhMOTlvb1FKX3Z1OUk?resourcekey=0-OIXHrDwCX8ChjypUbJo4fQ
SCHP - https://drive.google.com/file/d/1k4dllHpu0bdx38J7H28rVVLpU-kOHmnH/view
U2NET - https://drive.google.com/file/d/1rbSTGKAE-MTxBYHd-51l2hMOQPT_7EPy/view

# 👕 VITON-HD Custom Inference Pipeline

An end-to-end virtual try-on pipeline built using the **VITON-HD** model, integrated with:

- 🧥 **U-2-Net** for cloth mask generation  
- 👤 **SCHP** (Self-Correction Human Parsing) for human segmentation  
- 🕺 **OpenPose** for pose estimation (skeleton + keypoints)  
- 📸 Custom image and clothing support for high-resolution virtual try-on

---

## 🚀 How to Run

1) Upload checkpoints data and test dataset  
2) Upload image and cloth in `datasets/test/image` and `datasets/test/cloth` directories in **768x1024** format with **white background**  
3) After cloning U-2-Net repo, make a directory `u2net` in `saved_models` directory and upload U-2-Net model in it  
4) Before running `simple_extractor.py`, upload LIP model in `models` directory  
5) Rest go with the flow, everything is mentioned in the `.ipynb`

---

## ✅ Notes

- Tested on Python 3.11.3 (for VITON-HD compatibility) , also created virtual environment and used Python 3.8 for SCHP
- Requires pretrained models:
  - VITON-HD checkpoints
  - U-2-Net model (`u2net.pth`)
  - LIP model for SCHP (`exp-schp-201908261155-lip.pth`)
  - OpenPose output (pose JSON and image)
- All image inputs must be **768x1024** and have **white backgrounds** for best results.

---

## 💡 Credits

- [VITON-HD](https://github.com/ShuyaCheng/VITON-HD)
- [U-2-Net](https://github.com/xuebinqin/U-2-Net)
- [SCHP (LIP Parsing)](https://github.com/PeikeLi/Self-Correction-Human-Parsing)
- [OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose)

---
