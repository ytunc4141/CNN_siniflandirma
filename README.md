# 🧠 CNN ile Trafik Levhası Sınıflandırma

Bu projede, **trafik levhalarının (Dur – Yaya Geçidi)** görüntüler üzerinden sınıflandırılması amacıyla farklı CNN mimarileri denenmiştir.  
Aynı veri seti kullanılarak **üç farklı model** oluşturulmuş ve sonuçları karşılaştırılmıştır.

---

## 📂 Proje İçeriği

- **Model 1:** Transfer Learning (VGG16)
- **Model 2:** Temel CNN (Sıfırdan)
- **Model 3:** Geliştirilmiş CNN
- Eğitim / doğrulama grafikleri
- Tek görüntü üzerinde tahmin örnekleri

---

## 🗂️ Veri Seti

- **Sınıflar:**
  - `dur`
  - `yaya_gecidi`

- **Görseller:**
  - Kendi çektiğim gerçek trafik levhası görüntüleri  
  - Farklı açı, mesafe ve ışık koşulları

- **Veri bölünmesi:**
  - Eğitim (%80)
  - Doğrulama (%20)

> Model performansını artırmak için görseller **elle kırpılarak** levhaya odaklanılmıştır.

---

## 🧪 Model 1 – Transfer Learning (VGG16)

- Önceden eğitilmiş **VGG16** modeli kullanılmıştır.
- Özellik çıkarımı hazır ağ üzerinden yapılmıştır.
- Sadece üst katmanlar eğitilmiştir.
- Küçük veri setlerinde hızlı ve stabil sonuçlar vermektedir.

**Kullanım amacı:**  
Transfer learning yaklaşımının etkisini görmek.

---

## 🧪 Model 2 – Temel CNN (Sıfırdan)

- CNN mimarisi tamamen sıfırdan oluşturulmuştur.
- Convolution ve MaxPooling katmanları kullanılmıştır.
- Transfer learning **kullanılmamıştır**.
- Daha basit ve anlaşılır bir yapı tercih edilmiştir.

**Kullanım amacı:**  
Temel CNN yapısının performansını gözlemlemek.

---

## 🧪 Model 3 – Geliştirilmiş CNN

Model 2 üzerine bazı geliştirmeler yapılmıştır.

**Model 2’den farklı olarak:**
- Konvolüsyon katmanlarındaki **filtre sayıları artırılmıştır**.
- Daha derin bir ağ yapısı oluşturulmuştur.
- **Dropout (0.4)** katmanı eklenmiştir.
- Eğitim sırasında **online veri artırımı (data augmentation)** uygulanmıştır.

Bu değişiklikler sayesinde modelin genelleme yeteneği artırılmıştır.

---

## 📊 Eğitim ve Değerlendirme

Eğitim süreci boyunca:

- Accuracy
- Loss

değerleri takip edilmiştir.

- Eğitim ve doğrulama grafikleri notebook içerisinde gösterilmiştir.
- Her model doğrulama verisi üzerinde değerlendirilmiştir.

---

## 🖼️ Tek Görüntü Üzerinde Tahmin

Her model için:

- Tek bir trafik levhası görüntüsü modele verilmiştir.
- Tahmin edilen sınıf:
  - Görsel üzerinde
  - Sınıf adı ve güven oranı ile gösterilmiştir.

Bu sayede modellerin gerçek görüntüler üzerindeki davranışı gözlemlenmiştir.

---

## 🛠️ Kullanılan Teknolojiler

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab

---

## 📌 Notlar

- Tüm kodlar açıklamalı markdown hücreleri ile desteklenmiştir.
- Notebook adım adım ilerleyecek şekilde düzenlenmiştir.
- Okunabilirlik ve anlaşılabilirlik ön planda tutulmuştur.

---

## 👤 Öğrenci Bilgileri

- **Ad:** Yusuf  
- **Soyad:** Tunç  
- **Okul No:** 2012721024  

---
