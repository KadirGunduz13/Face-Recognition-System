# 🎭 Face Detection and Recognition System (Yüz Algılama ve Tanıma Sistemi)

[![English](https://img.shields.io/badge/Language-English-blue)](#english-version)


[![Türkçe](https://img.shields.io/badge/Dil-Türkçe-red)](#türkçe-sürüm)

---

<h2 id="english-version">ᴇɴ</h2>

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

*Successful Match*
 <img width="712" height="687" alt="test9" src="https://github.com/user-attachments/assets/5e49d343-de41-43f8-8bdc-e954dd38962e" />

*Unknown Face*
<img width="597" height="675" alt="test11" src="https://github.com/user-attachments/assets/0e40719f-a4e3-4afc-8e31-b32b81f04e27" />


### ⚙️ Setup and Usage
1. Clone the repository to your local machine:
   ```bash
   git clone [https://github.com/yourusername/face-recognition-system.git](https://github.com/yourusername/face-recognition-system.git)

2. Install the required dependencies:
   ```bash
   pip install opencv-python numpy face_recognition matplotlib

3. Add your training dataset to the `oyuncu_yuzleri/` directory and your test images to the `test_images/` directory, then run the notebook/script.

---

<h2 id="türkçe-sürüm">ᴛʀ</h2>

Bu proje, dijital görüntüler üzerindeki insan yüzlerini tespit etmek ve sistemde kayıtlı olan kişilerle eşleştirmek amacıyla geliştirilmiş bir Görüntü İşleme (Computer Vision) uygulamasıdır.

Sistem, yüz tespiti (detection) için **OpenCV Haar Cascade** algoritmasını, yüz tanıma (recognition) ve kimliklendirme aşaması için ise derin öğrenme tabanlı **face_recognition** kütüphanesini kullanmaktadır.

### 🚀 Özellikler
* **Hızlı Yüz Tespiti:** `haarcascade_frontalface_default.xml` kullanılarak görüntülerdeki yüzler hızlıca tespit edilir.
* **Yüksek Doğruluklu Tanıma:** Klasik LBPH algoritmaları yerine, yüzleri 128 boyutlu özellik vektörlerine (encodings) çevirerek Öklid mesafesi ile karşılaştırma yapar.
* **Dinamik Görselleştirme:** Tanınan kişiler yeşil çerçeve ve isim/benzerlik skoruyla; sistemde olmayan kişiler ise kırmızı çerçeve ve "Kayıtlı Değil" uyarısıyla etiketlenir.
* **Önişleme Desteği:** Işık farklılıklarını tolere edebilmek için görüntüleri gri tonlamaya çevirir ve Histogram Eşitleme (Equalization) uygular.

### 🛠️ Kullanılan Teknolojiler
* **Python 3.x**
* **OpenCV** (Görüntü işleme ve Haar Cascade)
* **face_recognition** (Derin öğrenme tabanlı yüz eşleştirme)
* **NumPy** (Matris ve dizi işlemleri)
* **Matplotlib** (Çıktıların görselleştirilmesi)

### 📸 Ekran Görüntüleri

*Başarılı Eşleşme*
 <img width="712" height="687" alt="test9" src="https://github.com/user-attachments/assets/5e49d343-de41-43f8-8bdc-e954dd38962e" />

*Kayıtlı Olmayan Yüz*
<img width="597" height="675" alt="test11" src="https://github.com/user-attachments/assets/0e40719f-a4e3-4afc-8e31-b32b81f04e27" />

### ⚙️ Kurulum ve Kullanım
1. Repoyu bilgisayarınıza klonlayın:
   ```bash
   git clone [https://github.com/kullaniciadin/face-recognition-system.git](https://github.com/kullaniciadin/face-recognition-system.git)

2. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install opencv-python numpy face_recognition matplotlib

3. Kendi veri setinizi `oyuncu_yuzleri/` klasörüne, test edeceğiniz fotoğrafları ise `test_images/` klasörüne ekleyerek kod dosyasını çalıştırın.
