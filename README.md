# 🎭 Face Detection and Recognition System

Bu proje, dijital görüntüler üzerindeki insan yüzlerini tespit etmek ve sistemde kayıtlı olan kişilerle eşleştirmek amacıyla geliştirilmiş bir Görüntü İşleme (Image Processing) uygulamasıdır. 

Sistem, yüz tespiti (detection) için **OpenCV Haar Cascade** algoritmasını, yüz tanıma (recognition) ve kimliklendirme aşaması için ise derin öğrenme tabanlı **face_recognition** kütüphanesini kullanmaktadır.

## 🚀 Özellikler
* **Hızlı Yüz Tespiti:** `haarcascade_frontalface_default.xml` kullanılarak görüntülerdeki yüzler hızlıca tespit edilir.
* **Yüksek Doğruluklu Tanıma:** Klasik LBPH algoritmaları yerine, yüzleri 128 boyutlu özellik vektörlerine (encodings) çevirerek Öklid mesafesi ile karşılaştırma yapar.
* **Dinamik Görselleştirme:** Tanınan kişiler yeşil çerçeve ve isim/benzerlik skoruyla; sistemde olmayan kişiler ise kırmızı çerçeve ve "Kayıtlı Değil" uyarısıyla etiketlenir.
* **Önişleme Desteği:** Işık farklılıklarını tolere edebilmek için görüntüleri gri tonlamaya çevirir ve Histogram Eşitleme (Equalization) uygular.

## 🛠️ Kullanılan Teknolojiler
* **Python 3.x**
* **OpenCV** (Görüntü işleme ve Haar Cascade)
* **face_recognition** (Derin öğrenme tabanlı yüz eşleştirme)
* **NumPy** (Matris ve dizi işlemleri)
* **Matplotlib** (Çıktıların görselleştirilmesi)

## 📸 Ekran Görüntüleri
*(Buraya başarılı bir eşleşmenin ve "Kayıtlı Değil" uyarısının ekran görüntülerini ekleyebilirsin: `![Tanınan Yüz](gorsel_linki.jpg)` formatında)*

## ⚙️ Kurulum ve Kullanım
1. Repoyu bilgisayarınıza klonlayın:
   `git clone https://github.com/kullaniciadin/face-recognition-system.git`
2. Gerekli kütüphaneleri yükleyin:
   `pip install opencv-python numpy face_recognition matplotlib`
3. Kendi veri setinizi `oyuncu_yuzleri/` klasörüne, test edeceğiniz fotoğrafları ise `test_images/` klasörüne ekleyerek kodu çalıştırın.
