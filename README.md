# Game-Customer-Persona-Segmentation
Bu proje, bir oyun şirketinin satış verilerini kullanarak kullanıcıları demografik özelliklerine göre segmentlere ayırmayı ve bu segmentlerin şirkete sağlayabileceği ortalama geliri tahmin etmeyi amaçlamaktadır.

## Proje Amacı

Veri bilimi bakış açısıyla kullanıcıları:

- Ülke (COUNTRY)
- Cihaz türü (SOURCE)
- Cinsiyet (SEX)
- Yaş aralığı (AGE_CAT)

kırılımlarına göre gruplayarak “seviye tabanlı müşteri tanımı” (persona) oluşturulmuştur. Her persona, PRICE (harcama) değişkenine göre segmentlere (A–D) ayrılarak analiz edilmiştir.

---

##  Kullanılan Adımlar

1. **Veri Keşfi:** Veri seti incelendi, eksik/aykırı değer kontrolleri yapıldı  
2. **AGE Kategorileştirme:** Yaşlar belirli aralıklara bölünerek `AGE_CAT` oluşturuldu  
3. **Persona Oluşturma:** COUNTRY, SOURCE, SEX ve AGE_CAT birleştirilerek `customers_level_based` üretildi  
4. **Tekilleştirme:** Aynı persona’ya sahip kayıtlar gruplandı, PRICE ortalamaları alındı  
5. **Segment Atama:** Persona’lar PRICE’a göre 4 segmente (A-B-C-D) ayrıldı  
6. **Yeni Müşteri Analizi:** Yeni gelen kullanıcıların hangi segmentte yer alacağı ve tahmini geliri hesaplandı

---

## 📁 Kullanılan Veri Seti

- **Dosya:** `persona.csv`  
- **Kaynak:** Miuul.com üzerinden sağlanan örnek oyun şirketi satış verisi  
- **Özellikler:** PRICE, SOURCE, SEX, COUNTRY, AGE

---

## Proje Çıktısı

Proje sonunda her persona'nın:

- Ortalama PRICE değeri
- Ait olduğu SEGMENT
- Segmentlerin ortalama, maksimum, toplam geliri

belirlenmiştir. Ayrıca yeni gelen kullanıcı profilleri (örneğin: `TUR_ANDROID_FEMALE_31_40`) için segment ve gelir tahmini yapılmıştır.

---

## 🔮 Gelecekte Neler Yapılabilir?

- Zaman serisi analizi ile dinamik kullanıcı davranışı izlenebilir  
- Makine öğrenmesi modelleriyle segment tahminlemesi yapılabilir  
- Kullanıcı etkileşimi, oturum süresi gibi değişkenlerle model zenginleştirilebilir  
- A/B testleriyle segment bazlı kampanya etkisi ölçülebilir  
- Yeni veriler geldikçe persona ve segment yapısı güncellenebilir

---

##  Teşekkürler

Bu proje [Miuul](https://www.miuul.com/) tarafından sunulan Python for Data Science eğitim kapsamında final projesi olarak gerçekleştirilmiştir.  
Veri bilimi öğrenme sürecime büyük katkı sağladı.


> Not: Bu proje Kaggle üzerinde de yayınlanmıştır.
