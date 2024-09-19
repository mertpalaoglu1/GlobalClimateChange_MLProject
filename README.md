
Mini Final Project for Aygaz Machine Learning Bootcamp lead by Global AI Hub
# İklim Verileri Analizi ve Gelecek Tahminleri
https://www.kaggle.com/code/mertpalaolu/globalclimatechange-mlproject
## Proje Açıklaması

Bu proje, 1700'lü yıllardan itibaren belirli ülkeler için sağlanan sıcaklık verilerini inceleyerek zaman içinde yaşanan iklimsel değişiklikleri belirlemeyi ve gelecekteki sıcaklık değişimlerini tahmin etmeyi amaçlamaktadır. Veri analizi ve makine öğrenmesi teknikleriyle iklim trendlerini modellemeyi hedefler.

## Veri Seti

Proje, **Global Land Temperatures By Country** veri seti kullanılarak gerçekleştirilmiştir. Veri seti, dünya genelindeki farklı ülkelerde yıllara göre ortalama sıcaklık verilerini içermektedir.

### Veri Seti Özellikleri:

- **dt**: Tarih bilgisi (Yıl-ay-gün formatında)
- **AverageTemperature**: İlgili döneme ait ortalama sıcaklık (Celsius cinsinden)
- **AverageTemperatureUncertainty**: Ortalama sıcaklık ölçümündeki belirsizlik aralığı
- **Country**: Sıcaklık verisinin ait olduğu ülke

### Zaman Aralığı:

- 1700'lü yıllardan itibaren günümüze kadar olan dönemi kapsamaktadır.

## Kullanılan Algoritmalar

### 1. Gözetimli Öğrenme (Supervised Learning)

Lineer Regresyon kullanılarak yıllara göre ortalama sıcaklık tahmin edilmiştir.

- **Hedef Değişken**: Ortalama sıcaklık (`AverageTemperature`)
- **Model Performansı**:
  - **Mean Squared Error (MSE)**: 100.08491202660512
  - **Root Mean Squared Error (RMSE)**: 10.004244700456159

Lineer regresyon modeli, yıllara göre sıcaklık tahmininde makul bir başarı sağlamış olup, uzun dönem trendleri anlamak için uygun sonuçlar vermiştir.

### 2. Gözetimsiz Öğrenme (Unsupervised Learning)

K-means Kümeleme kullanılarak sıcaklık verileri kümelere ayrılmış ve benzer iklimsel dönemler tespit edilmiştir.

- **Silhouette Skoru**: 0.3959

Gözetimsiz öğrenme yöntemleri, zaman serisi verilerinde sınırlı performans göstermiş olsa da, belirli bölgeler ve dönemler arasında benzer sıcaklık trendlerini tespit etmiştir.

## Sonuçlar

Gözetimli öğrenme, zaman serisi verilerinde geleceği tahmin etme konusunda başarılı sonuçlar verirken, gözetimsiz öğrenme, veriyi gruplamak için kullanılabilir. Bu veri seti için **gözetimli öğrenme** **daha uygun sonuçlar vermiştir**, ancak belirli dönemler arasında benzerlik analizi yapmak için **gözetimsiz öğrenme** de faydalı olabilir.

---


