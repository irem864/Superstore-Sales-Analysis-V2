### Superstore Stratejik Satış & Bütçe Analizi (V2.0)


![Dashboard Görünümü](store2.png)


 ## Gelişim ve İnovasyon (Neler Yeni?)
Bu versiyon, mevcut altyapının üzerine sektör profesyonellerinden alınan geri bildirimler doğrultusunda karar verdirici katmanlar eklenerek geliştirilmiştir:

Bütçe ve Hedef Takibi (Yeni): Satış performansını hedefle kıyaslayan dinamik Gauge yapısı.

İnteraktif Coğrafi Harita (Yeni): Bölgesel analiz için bar grafiklerinden harita tabanlı derinleşme (drill-down) yapısına geçiş.

Operasyonel Detay Tablosu (Yeni): En değerli 3 müşteri ve birim maliyet analizlerini içeren aksiyonel tablo.

Görsel Modernizasyon (Yeni): Gölge efektleri, yuvarlatılmış köşeler ve modern renk paleti ile profesyonel UI/UX.

##  Korunan ve Geliştirilen Fonksiyonlar (Core Infrastructure)
Projenin temelini oluşturan ve işlevselliği korunan mevcut yapılar:

Trend Analizi: Aylara göre satış dağılımını gösteren çizgi grafikler.

Kategorik Analiz: Ürün ve kategori bazlı performans bar grafikleri.

Gelişmiş Filtreleme (Slicers): Bölge, kategori, segment ve tarih bazlı çok boyutlu dilimleyiciler.


## Teknik Mimari & DAX
Tools: Power BI, Power Query, DAX.

Key Measures: Toplam Satış, Kâr Marjı, Toplam Kar,Sipariş sayısı

## Gelişmiş DAX Ölçüleri (Calculated Measures)
Kar Marjı = DIVIDE(SUM('Sample - Superstore'[Profit]), SUM('Sample - Superstore'[Sales]))

Sipariş Sayısı = COUNT('Sample - Superstore'[Order ID])

Toplam Kar = SUM('Sample - Superstore'[Profit])

Toplam Satış = SUM('Sample - Superstore'[Sales])

## Veriseti Yapısı (Dataset Schema)
Analizde kullanılan Sample - Superstore veriseti aşağıdaki ana boyutları içermektedir:

Müşteri Bilgileri: Customer Name, Segment, City, State.

Sipariş Detayları: Order ID, Order Date, Ship Mode.

Ürün ve Finans: Category, Sub-Category, Sales, Quantity, Profit, Discount.



