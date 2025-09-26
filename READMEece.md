# Türkiye Trafik İşaretleri Sınıflandırma (CNN)

## Amaç
Bu proje, Türkiye trafik işaretlerini görüntüden sınıflandırmak için basit bir CNN modeli geliştirmeyi amaçlamaktadır.  
Proje, Akbank Derin Öğrenme Bootcamp kapsamında yapılmıştır.

## Veri Seti
- Kaynak: Kaggle (Türkiye Trafik İşaretleri)  
- Eğitim ve doğrulama verileri `traffic_data/train` ve `traffic_data/val` klasörlerinden alınmıştır.  
- Görseller 64x64 boyutuna getirilip tensör formatına dönüştürülmüştür.

## Kullanılan Teknolojiler
- Python  
- PyTorch  
- Torchvision  
- scikit-learn  
- Matplotlib  

## Yöntem
- Basit CNN mimarisi:  
  - Conv → ReLU → MaxPool  
  - Fully Connected katman  
- Loss: CrossEntropyLoss  
- Optimizer: Adam (lr=0.001)  
- Eğitim süresi: 20 epoch  

## Sonuçlar
- Eğitim ve doğrulama kayıplarının (Loss) ve doğruluklarının (Accuracy) grafikleri çizildi.  
- Confusion Matrix ve Classification Report elde edildi.  
- Ortalama doğruluk, modelin trafik işaretlerini ayırt etmede yeterli bir performans gösterdi.  

### Görseller ve Çıktılar
- Eğitim grafikleri: `artifacts/history.png`  
- Confusion matrix: `artifacts/confusion_matrix.png`  
- Classification raporu: `artifacts/classification_report.txt`  

## Hyperparametre Denemesi
- **Batch size denemesi:**  
  - Batch size 32 kullanıldığında eğitim daha hızlı oldu.  
  - Batch size 16 kullanıldığında eğitim daha yavaş ama doğrulama sonuçları daha stabil hale geldi.  

## Çalıştırma
1. Kaggle veya Google Colab ortamında notebook’u açın.  
2. Dataset’i yükleyin (`traffic_data/train`, `traffic_data/val`).  
3. Notebook hücrelerini sırasıyla çalıştırın.  
4. Çıktılar `artifacts/` klasöründe oluşacaktır.  

## Linkler
- [Kaggle Notebook](KAGGLE_LINKİNİ BURAYA EKLE)  
- [GitHub Repository](GITHUB REPO LİNKİNİ BURAYA EKLE)  
