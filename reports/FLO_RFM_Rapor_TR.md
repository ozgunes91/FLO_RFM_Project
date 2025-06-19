
# FLO RFM Analizi - Proje Raporu

## 1. Proje Amacı
Bu projede, FLO firmasının omni-channel (hem online hem offline) alışveriş yapan müşterilerini, geçmiş davranışlarına göre segmentlere ayırmak hedeflenmiştir. Amaç, bu segmentlere uygun pazarlama stratejileri belirlemektir.

## 2. Veri Seti
Veri seti, FLO'ya ait son iki yıl içinde gerçekleşen online ve offline satış hareketlerini içeren, her bir müşteri için alışveriş kanalları, sipariş sayıları, harcamaları ve tarih bilgilerini barındıran özelliklere sahiptir.

> Not: Veri seti lisans ve gizlilik nedeniyle GitHub projesine dahil edilmemiştir.

## 3. Yöntem: RFM Analizi
RFM (Recency, Frequency, Monetary) analizi uygulanarak müşteriler şu şekilde değerlendirilmiştir:

- **Recency**: Müşterinin en son alışveriş tarihinden itibaren geçen gün sayısı
- **Frequency**: Toplam alışveriş sayısı
- **Monetary**: Toplam harcama tutarı

Bu metrikler 1-5 arası skorlanarak "RF_SCORE" değerleri elde edilmiştir.

## 4. Segment Tanımları
RFM skorları regex tabanlı şu kurallarla segmentlere dönüştürülmüştür:

- `champions`, `loyal_customers`, `at_Risk`, `hibernating`, `new_customers`, `cant_loose`, vb.
- Her segment farklı bir davranış örüntüsü gösterir (sadakat, riskli, yeni, uykuda vs.)

## 5. Pazarlama Önerileri (Case Çözümleri)

### Case A:
Yüksek fiyatlı yeni kadın ayakkabı markasını tanıtmak için:

- `champions` ve `loyal_customers` segmentlerindeki,
- Son 12 ayda kadın kategorisinden alışveriş yapan müşteriler hedeflenmelidir.

### Case B:
Çocuk ve erkek ürünlerinde indirim kampanyası için:

- `cant_loose`, `hibernating`, `new_customers` segmentlerindeki,
- Erkek/çocuk ürünleriyle ilgilenen müşteriler hedeflenmelidir.

## 6. Sonuç
Bu çalışma ile müşteriler davranış temelli segmentlere ayrılmış ve bu segmentlere özel pazarlama eylemleri planlanabilir hale gelmiştir.

RFM analizi, sadakat, kayıp riski, potansiyel gibi temel unsurları belirlemede etkin bir araçtır.

---

**Not**: Bu rapor, kodlama çalışmasından öğrenilenler temelinde oluşturulmuştur ve kişisel bilgi veya ticari veri içermez.
