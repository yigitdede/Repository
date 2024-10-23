# Sınıflandırma Projesi

## İçindekiler
- [Veri Seti](#veri-seti)
- [Gereksinimler](#gereksinimler)
- [Model Yapısı](#model-yapısı)
- [Eğitim Süreci](#eğitim-süreci)
- [Sonuçlar](#sonuçlar)
- [Karmaşıklık Matrisi](#karmaşık-matris)
- [Nasıl Kullanılır](#nasıl-kullanılır)
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
Model, üç gizli katman ve bir çıkış katmanından oluşan bir yapıya sahiptir. 
- İlk gizli katman: 512 nöron
- İkinci gizli katman: 256 nöron
- Üçüncü gizli katman: 128 nöron

## Eğitim Süreci
Model, %80 eğitim ve %20 test verisi ile eğitilmiştir. Eğitim süreci sırasında, erken durdurma (early stopping) uygulanmıştır.

## Sonuçlar
Modelin test verisi üzerindeki doğruluğu hesaplanmış ve sonuçlar grafiklerle gösterilmiştir.

## Confusion(Karmaşıklık) Matrisi
Modelin başarısını daha iyi değerlendirmek için karmaşıklık matrisi oluşturulmuştur.

## Kaggle Proje Linki
Proje linki: [Kaggle Projesi](https://www.kaggle.com/code/yigitdede/classification-fish?scriptVersionId=202891630)
