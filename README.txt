# Duygu Analizi Projesi

Bu proje, metin verileri üzerinde duygu analizi yapmayı hedeflemektedir. Kullanılan veri seti, incelemeler ve bu incelemelere ait pozitif veya negatif duygu etiketlerini içermektedir. Projede, metin işleme adımları, vektörleştirme teknikleri ve makine öğrenimi modelleri kullanılarak duygu sınıflandırması yapılmıştır.

## Proje İçeriği

1. **Veri Seti**: Projede kullanılan veri seti, inceleme metinleri (`review`) ve bu metinlere ait duygu etiketlerini (`sentiment`) içermektedir.
   - Veri seti iki sütundan oluşmaktadır: `review` ve `sentiment`.
   - `review`: Kullanıcı yorumları.
   - `sentiment`: Yorumların pozitif veya negatif olduğunu belirten etiketler.

2. **Veri Ön İşleme**:
   - Veriler temizlenmiş ve normalleştirilmiştir.
   - Metinler üzerinde gereksiz karakterler, sayılar ve noktalama işaretleri çıkarılarak düzenlenmiştir.

3. **TF-IDF Vektörleştirme**:
   - Metin verilerini sayısal verilere dönüştürmek için TF-IDF (Term Frequency-Inverse Document Frequency) kullanılmıştır.
   - Maksimum 5000 özelliğe sahip TF-IDF vektörleri oluşturulmuştur.

4. **Makine Öğrenimi Modelleri**:
   - Projede, duygu sınıflandırması için çeşitli makine öğrenimi algoritmaları kullanılmıştır:
     - Lojistik Regresyon
     - Support Vector Machine (SVM)
     - Random Forest
   - Bu modeller, `accuracy`, `precision`, `recall` ve `F1-score` gibi performans metrikleri ile değerlendirilmiştir.

5. **Kelime Bulutu**:
   - Metinlerdeki en sık kullanılan kelimeleri görselleştirmek için kelime bulutu (Word Cloud) oluşturulmuştur.

6. **Kelime Frekans Analizi**:
   - Kelimelerin hangi sıklıkta geçtiği ekrana yazdırılmıştır.

## Kullanılan Teknolojiler

- Python
- Pandas
- Scikit-learn
- WordCloud
- Matplotlib
