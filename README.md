# Face Mask Detection using TinyML, Edge Impulse, and OpenMV

This project demonstrates the use of **TinyML**, **Edge Impulse**, and **OpenMV** to build a **real-time face mask detection system**. The system can detect whether a person is wearing a face mask or not and is designed to run efficiently on embedded devices like OpenMV Cam.

---

## 🚀 Overview

By leveraging the Edge Impulse platform, a Convolutional Neural Network (CNN) model was trained on labeled images of people with and without masks. The model was then deployed onto an edge device to perform live inference using a connected camera module.

---

## 📁 Dataset Acquisition

- The dataset was sourced from the **COVID-19 PIS** dataset hosted on **Roboflow**.
- It includes images categorized into two classes:
  - **Mask**
  - **No Mask**

---

## 📤 Data Upload to Edge Impulse

- Images were uploaded to the [Edge Impulse](https://www.edgeimpulse.com/) platform.
- The platform's intuitive UI was used to label and manage the dataset.
- Edge Impulse automatically:
  - Normalizes and augments data
  - Prepares it for efficient model training and deployment

---

## 🧠 Model Training

- The model was trained using a **Convolutional Neural Network (CNN)** optimized for image classification tasks.
- We handled:
  - Feature extraction
  - Model configuration
  - Training and validation pipeline

---

## 📊 Model Evaluation

- Performance metrics like **accuracy**, **precision**, and **recall** were monitored.
- Evaluation was performed using a reserved test dataset.
- Results and confusion matrix were accessible on the Edge Impulse dashboard.

---

## 💻 Code Explanation

This repository contains the complete code and scripts used to integrate the trained model with **OpenMV Cam**. It includes:
- MicroPython scripts for loading and running the `.tflite` model
- Real-time camera input processing
- Displaying mask/no mask detection results on the OpenMV device

Refer to the code files and comments within the repository for detailed understanding.

---

## 📸 Real-Time Inference

- The model was integrated with a live webcam or camera feed.
- Real-time image processing was done using Python scripts or firmware on the OpenMV Cam.
- The system could:
  - Capture a frame
  - Run inference
  - Output mask/no mask detection in milliseconds

---


## 📸 Demo

🎥 **Watch the project in action!**  
[![Face Mask Detection Demo](https://img.youtube.com/vi/YOUR_VIDEO_ID/0.jpg)](https://www.loom.com/share/bd40cdbb3b38406e85c57beb72f269fe?sid=7a2bfc8d-a0ca-472e-9be3-cd6883bad0e8)


---

## 🧰 Tools & Technologies

- [Edge Impulse](https://www.edgeimpulse.com/)
- [Roboflow](https://roboflow.com/)
- TensorFlow Lite
- OpenMV IDE
- OpenMV Cam
- Python
- TinyML