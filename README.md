# Sınıflandırma Projesi

## İçindekiler
- [Veri Seti](#veri-seti)
- [Gereksinimler](#gereksinimler)
- [Model Yapısı](#model-yapısı)
- [Eğitim Süreci](#eğitim-süreci)
- [Sonuçlar](#sonuçlar)
- [Karmaşıklık Matrisi](#Karmaşıklık-Matrisi)
- [Kaggle Proje Linki](#kaggle-proje-linki)

## Veri Seti
Proje, A Large Scale Fish Dataset isimli veri setini kullanmaktadır. Veri seti, farklı türde balıkların görüntülerini içermektedir.

## Gereksinimler
- Python 3.x
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn

## Model Yapısı
Model, aşağıdaki katmanlardan oluşmaktadır:
- Giriş katmanı: 512 nöron, ReLU aktivasyon fonksiyonu
- Gizli katman 1: 512 nöron, ReLU aktivasyon fonksiyonu
- Gizli katman 2: 256 nöron, ReLU aktivasyon fonksiyonu
- Gizli katman 3: 128 nöron, ReLU aktivasyon fonksiyonu
- Çıkış katmanı: 9 nöron, softmax aktivasyon fonksiyonu

## Eğitim Süreci
Model, %80 eğitim ve %20 test verisi ile eğitilmiştir. Eğitim süreci sırasında, erken durdurma (early stopping) uygulanmıştır.

## Sonuçlar
Modelin test verisi üzerindeki doğruluğu hesaplanmış ve sonuçlar grafiklerle gösterilmiştir.

## Karmaşıklık Matrisi
Modelin başarısını daha iyi değerlendirmek için karmaşıklık matrisi oluşturulmuştur.

## Kaggle Proje Linki
Proje linki: [Kaggle Projesi](https://www.kaggle.com/code/yigitdede/classification-fish?scriptVersionId=202891630)
