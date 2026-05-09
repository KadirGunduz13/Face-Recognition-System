# 🎭 Face Detection and Recognition System (Yüz Algılama ve Tanıma Sistemi)

[![English](https://img.shields.io/badge/Language-English-blue)](#english-version)
[![Türkçe](https://img.shields.io/badge/Dil-Türkçe-red)](#türkçe-sürüm)

---

<h2 id="english-version">🇬🇧 English Version</h2>

This project is a Computer Vision application developed to detect human faces in digital images and match them with registered individuals in the system.

The system uses the **OpenCV Haar Cascade** algorithm for face detection and the deep learning-based **face_recognition** library for the facial recognition and identity matching stages.

### 🚀 Features
* **Fast Face Detection:** Rapidly detects faces in images using `haarcascade_frontalface_default.xml`.
* **High-Accuracy Recognition:** Instead of classic LBPH algorithms, it converts faces into 128-dimensional feature vectors (encodings) and compares them using Euclidean distance.
* **Dynamic Visualization:** Recognized individuals are labeled with a green bounding box, their name, and a similarity score. Unregistered faces are labeled with a red box and a "Not Registered" (Kayıtlı Değil) warning.
* **Image Preprocessing:** Converts images to grayscale and applies Histogram Equalization to tolerate lighting differences and improve accuracy.

### 🛠️ Technologies Used
* **Python 3.x**
* **OpenCV** (Image processing and Haar Cascades)
* **face_recognition** (Deep learning-based facial embeddings)
* **NumPy** (Matrix and array operations)
* **Matplotlib** (Output visualization)

### 📸 Screenshots
*(Insert your screenshots here)*
* `![Successful Match](link_to_image_1)`
* `![Unknown Face](link_to_image_2)`

### ⚙️ Setup and Usage
1. Clone the repository to your local machine:
   ```bash
   git clone [https://github.com/yourusername/face-recognition-system.git](https://github.com/yourusername/face-recognition-system.git)
