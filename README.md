# Fish Classification Project

## Proje Hakkında
Bu proje, farklı türdeki balıkları sınıflandırmak için derin öğrenme yöntemleri kullanarak bir model geliştirmeyi amaçlamaktadır. Proje, büyük ölçekli bir balık veri kümesi kullanarak gerçekleştirildi ve TensorFlow ve Keras kütüphaneleriyle bir yapay sinir ağı (ANN) modeli oluşturuldu.

## İçindekiler
- [Veri Seti](#veri-seti)
- [Gereksinimler](#gereksinimler)
- [Model Yapısı](#model-yapısı)
- [Eğitim Süreci](#eğitim-süreci)
- [Sonuçlar](#sonuçlar)
- [Karmaşıklık Matrisi](#karmaşıklık-matrisi)
- [Nasıl Kullanılır](#nasıl-kullanılır)

## Veri Seti
Proje, `A Large Scale Fish Dataset` adlı bir veri setini kullanmaktadır. Veri setinde balık türlerine ait resimler bulunmaktadır. Her resim, ilgili balık türü etiketiyle birlikte yüklenmiştir.

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
Model, 100 epoch boyunca, 64'lü batch boyutlarıyla eğitilmiştir. Eğitim sırasında erken durdurma (EarlyStopping) kullanılarak overfitting önlenmiştir.

```python
from keras.callbacks import EarlyStopping

# EarlyStopping tanımı
early_stopping = EarlyStopping(monitor='val_loss', patience=10, restore_best_weights=True)

# Model eğitimi
results = model.fit(X_train_flattened, y_train_one_hot, epochs=100, batch_size=64, validation_data=(X_test_flattened, y_test_one_hot), callbacks=[early_stopping])


##Sonuçlar
Modelin test doğruluğu hesaplandı ve sonuçlar ekrana yazdırıldı. Ayrıca, modelin eğitim sürecindeki kayıp (loss) ve doğruluk (accuracy) grafikleri çizildi.

## Kaggle Proje Linki
Projeye [buradan][(https://www.kaggle.com/your-kaggle-link)](https://www.kaggle.com/code/yigitdede/classification-fish?scriptVersionId=202891630) ulaşabilirsiniz.
