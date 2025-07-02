# 🚗 Lane Detection using Deep Learning (U-Net + OpenCV)

This project implements **lane detection** in road driving videos using a **U-Net convolutional neural network** for semantic segmentation, combined with **OpenCV** for video processing. The system takes a road video as input, detects lane lines in each frame, and outputs a video with the detected lanes overlaid.

---

## 🎯 Objective

- To develop an efficient deep learning model for real-time **lane detection** using semantic segmentation.
- To automate video processing using **OpenCV** and produce an annotated output video.
- To provide a reliable solution for use in **autonomous driving** and **advanced driver-assistance systems (ADAS)**.

---

## 📦 Features

- 🎥 **Video input and output** (supports `.mp4`, `.avi`, etc.)
- 🧠 **U-Net model** trained for semantic lane segmentation
- 🎯 Real-time frame-by-frame prediction and overlay
- 🔧 Easy customization for any road/lane dataset
- 🖥️ Built with Python, Keras/TensorFlow, and OpenCV

---

## 📁 Files Included

- `lane_detection_unet.py` – Script to load video, apply U-Net model, and save output
- `input_video.mp4` – Sample road driving video
- `README.md` – Documentation

---

## 🧠 Model Architecture

The project uses a **U-Net** architecture for semantic segmentation of road lanes.

- **Encoder**: Contracting path with convolution + max pooling
- **Decoder**: Expanding path with upsampling + skip connections
- **Output**: Binary mask (lane vs. background)

---

## 🧪 How It Works

1. Load pretrained U-Net model (`lane_segmentation_model.h5`)
2. Read input video frame-by-frame using OpenCV
3. Resize and normalize each frame
4. Predict segmentation mask using U-Net
5. Overlay mask on original frame
6. Save all processed frames as `output_video.mp4`

---

