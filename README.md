# 🧵 Fabric Defect Detection using Image Subtraction

This Python project compares a **reference (perfect)** fabric image with a **test (possibly defective)** fabric image to automatically detect and highlight defects using OpenCV.

---

## 📌 Overview

The algorithm uses **image subtraction** to find the differences between two aligned images and highlights the regions of defects using bounding boxes.

---

## 🧠 How It Works

1. **Load & Resize**: Both reference and test images are resized to the same dimensions.
2. **Convert to Grayscale**: Simplifies the image comparison by reducing complexity.
3. **Image Subtraction**: Calculates the absolute difference between the two grayscale images.
4. **Thresholding**: Highlights areas with significant differences (potential defects).
5. **Noise Removal**: Uses morphological operations to clean up noise.
6. **Contour Detection**: Identifies and draws bounding boxes around real defect regions.
7. **Display Results**: The final image is shown with all detected defects labeled.

---

## 🛠️ Requirements

Install required Python libraries:

```bash
pip install opencv-python numpy matplotlib
