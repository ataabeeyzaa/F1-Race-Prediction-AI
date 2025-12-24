# 🏎️ Formula 1 Race Prediction with Deep Learning

Bu proje, 1950-2025 yılları arasındaki Formula 1 verilerini kullanarak pilotların podyuma çıkıp çıkmayacağını tahmin eden bir Yapay Zeka modelidir.

## 🚀 Proje Özeti
Formula 1 gibi kaotik ve dinamik bir sporda, makine öğrenmesi yöntemleri kullanılarak yarış sonuçları tahmin edilmiştir.

* **Başarı Oranı (Accuracy):** %99.7 🏆
* **Kullanılan Teknolojiler:** PyTorch, Pandas, NumPy, Scikit-Learn.
* **Modeller:**
    * YSA (Yapay Sinir Ağları)
    * LSTM (Long Short-Term Memory - Zaman Serisi Analizi)
    * Binary Classification (Podyum Var/Yok)

## 🧠 Yapılan Mühendislik Çalışmaları
1.  **Veri Temizliği:** Eksik veriler KNN Imputer ile dolduruldu.
2.  **Feature Engineering:**
    * `Driver Age`: Sürücülerin deneyimi hesaplandı.
    * `Recent Form`: Son 3 yarışlık performans ortalaması (Momentum) eklendi.
3.  **Derin Öğrenme:**
    * Model, Batch Normalization ve Dropout katmanları ile güçlendirildi.
    * Veri setindeki dengesizlikler analiz edildi.

## 📊 Sonuçlar (Confusion Matrix)
Model, test setindeki 320 yarış senaryosundan **319 tanesini doğru tahmin etmiştir.**

| | Tahmin: Yok | Tahmin: Var |
|--- | --- | --- |
| **Gerçek: Yok** | 275 (TN) | 0 (FP) |
| **Gerçek: Var** | 1 (FN) | 44 (TP) |

---
*Bu proje [Beyza ATA] tarafından geliştirilmiştir.*
