# Abyss PDF Karşılaştırma Raporu v0.2

**Karşılaştırılan dosyalar**
- Özgün: `merged2pdf.pdf` — 512 sayfa, 92.942.222 bayt (~88,6 MiB).
- OCR'li: `Abyss_OCR.pdf` — 512 sayfa, 239.300.940 bayt (~228,3 MiB).

## Bulgular

1. Her iki PDF de 512 sayfa. Örnek sayfa kontrolleri ve metin yerleşimi ilk 204 sayfanın aynı sırada korunduğunu gösteriyor.
2. Özgün PDF'nin metin çıkarımında fiziksel s. 1–204 boş kalıyordu. Kullanıcının OCR PDF'sinden bu sayfalara ait toplam **95.158 kelime** çıkarıldı.
3. OCR'li PDF'den 512 sayfanın tamamında **328.231 kelime** çıkarıldı; özgün PDF'nin mevcut metin katmanından 233.073 kelime çıkarılıyordu. Bu fark ilk 204 sayfanın tamamının aranabilir hâle geldiğiyle tutarlı.
4. Fiziksel s. 205–512 için her iki PDF'den alınan içerik, boşluklar normalize edildikten sonra **birebir eşleşiyor**: 1.726.620 karakter ve 233.073 kelime. Metin katmanının mevcut bölümü değişmemiş.
5. Daha önce üretilmiş `Abyss_1-204_OCR.txt` ile karşılaştırıldığında, kullanıcı PDF'sinden çıkarılan ilk 204 sayfa metni sayfa bazında ortalama yaklaşık **%90,1 normalize benzerlik** gösteriyor. Bu oran bir doğruluk skoru değildir; OCR motorları arasındaki metin farkını ölçer. Örneklerde yeni PDF Türkçe diakritikleri daha iyi koruyor.

## Kullanım önerisi

- Aranabilir ana çalışma kopyası olarak `Abyss_OCR.pdf` kullan.
- Orijinal `merged2pdf.pdf` dosyasını değiştirilmemiş kaynak kopya olarak sakla.
- Metin araştırması için `Abyss_OCR_TumMetin.txt` dosyasını kullan; her sayfa açık bir fiziksel sayfa etiketiyle ayrılmıştır.
- Kişi adları, aliaslar, kurgusal terimler, sayı/oranlar ve güç kuralları kanon belgelerine aktarılmadan önce gerektiğinde PDF sayfa görüntüsünden doğrulanmalı.

## Açık kaynak eksikliği

OCR karşılaştırması, arşiv içindeki metin erişimi sorununu çözüyor. Ancak PDF'nin s. 22–26 bölümünde birincil kaynak olarak anılan **“Abyss Evreni: Tam Arşiv v1.2”** dosyası bu iki PDF'nin içinde bulunmuyor. Bu dosyanın içerik karşılaştırmasına katılması, daha önce belirlenmiş kaynak önceliğini doğrulamak için ayrıca gerekli olabilir.
