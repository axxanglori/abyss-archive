# ABYSS — Kaynak Konum Eşleştirme İndeksi v0.5

**Bu sürüm:** Olay/kronoloji aşaması (27 kayıt) için ilk kaynak denetimi eklendi. v0.4 korunmuştur.

**Yeni ekler:** [Olay ve Kronoloji Kaynak Denetimi v0.1](Abyss_Olay_Kronoloji_Kaynak_Denetimi_v0.1.md)

**Bu aşamadaki temel sonuçlar:**
- Bowling Faciası, Kintoki’nin ölümü ve karantina/örtbas, v1.2 Bölüm 7.4–7.5’te oturum günlüğü olayı olarak anlatılıyor.
- Horizon Day’in gerçek katili için K-001 kararı uygulanıyor: March/Arcturus; halka yansıyan anlatı Deneb/September.
- “T9 darbesi” iki zaman katmanına ayrıldı: geçmiş yargılanma/tasfiye ve PDF s.190’da plan olarak yazılan F.O.R.A.–Mafya ittifakının T9’a karşı hamlesi.
- Görev panosu, Fate Core ev kuralları, şehir kodeksi, Prime/Fringe/Rogue tercihi ve Indigo boss tasarımı olay olarak kanonlaştırılmadı.

---

# Önceki sürüm gövdesi: Kaynak Konum Eşleştirme İndeksi v0.4

**Hazırlanma tarihi:** 24 Ekim 2026  
**Eşleştirilen envanter:** `Abyss_Arsiv_Envanteri_v0.8.md`  
**Sürüm notu:** v0.4, 302 kayıtlık eşleştirme listesini korur; ilk 10 Origin/Mana kaydına, 37 kurum/coğrafya kaydına ek olarak 100 karakter kaydı için kaynak pasajı, kaynak türü ve açık nokta eklendi.  
**Öncelikli lore kaynağı:** `Abyss Evreni_ Tam Arşiv v1.2.docx` (17 sayfa)  
**Tamamlayıcı konuşma arşivi:** `Abyss_OCR.pdf` (512 fiziksel sayfa; bu çalışma için `merged2pdf.pdf` ile aynı içerik kabul edildi.)

## Dosyalar nasıl okunmalı?

Bu indeks, envanterdeki kayıtları **iki ayrı fiziksel sayfalama sistemi** üzerinden eşleştirir: DOCX sayfaları ve konuşma PDF’sinin fiziksel sayfaları. CSV, satır düzeyindeki ayrıntılı defterdir; her satırda kayıt türü, envanter bağlantısı, ana kaynak konumu, metinde bulunan sayfalar ve durum notu vardır.

- **Ana konum**: kaydın en açıklayıcı veya karar açısından öncelikli bağlamı. Bu, tüm görünen kelime eşleşmelerinin listesi değildir.
- **Metin eşleşme sayfaları**: ad/terim, OCR’dan çıkarılan metinde aynı sayfada en az bir kez bulundu. Bunlar bulunabilirlik işaretleridir; her eşleşmenin bağlam bakımından doğru kişi/olay olduğunun garantisi değildir.
- **DOCX ana kaynak**: v1.2’nin metinsel tanımı varsa öncelik ondadır. DOCX’te karşılığı bulunmayan ekler, sohbet PDF’sinden tamamlayıcı kayıt olarak tutulur.
- **Olay / FRP kayıtları**: öneri, oyun yöneticisi taslağı, oyuncu günlüğü, kurum içi rapor ve gerçekleşmiş masa olayı tek statüde birleştirilmez.
- Bazı kısa/ortak terimler (ör. `Eli`, `Asa`, `March`, `Mana`, `T9`) çok sayıda eşleşme üretir; özellikle bu terimlerin sayfa listeleri bağlam kontrolü için gezinme yardımıdır.

## Kapsam özeti

| Kayıt türü | Satır sayısı |
|---|---:|
| Karakter | 100 |
| Origin / güç sistemi | 109 |
| Kurum / örgüt | 21 |
| Coğrafya / yer | 16 |
| Olay / kronoloji | 27 |
| FRP / oyun mekaniği | 29 |
| **Toplam** | **302** |

## Kaynak haritası: ana çıpalar

| Konu kümesi | Tam Arşiv v1.2 | Konuşma arşivi PDF | Eşleştirme notu |
|---|---|---|---|
| Origin, mana, Nebula, Mana Çürümesi, Origin Felaketi | s. 1–2, Bölüm 1 | fiziksel s. 205–208; ek konuşmalar için CSV sayfa eşleşmeleri | DOCX ana tanım; sohbet açıklaması tamamlayıcıdır. |
| Perde, Outlander’lar, Euruyn/Morygnn, Ambrossa | s. 2, Bölüm 2 | fiziksel s. 62–66 ve 205–208; sonraki Outlander sahneleri | Mit/köken ve sahne kaynakları ayrılmalı. |
| Devletler, kurumlar, mafya aileleri, Siyah Kan | s. 2–3, Bölüm 3–4 | fiziksel s. 24–30; 35–46; 151–160; 247–250 | F.O.R.A. beş devlet; Rhodes bağımsız. T9 ayrı güç odağı. |
| Ana karakter geçmişleri | s. 3, Bölüm 5 | erken kampanya s. 1–204; ana dünya inşa s. 205–413 | V1.2 üstün; sohbet günlükleri ve öneriler kendi statülerinde kalır. |
| FRP oturum günlükleri | s. 4–6, Bölüm 7 | ilgili fiziksel sayfalar CSV’de aranmış terim/olay bazında listelenir | Oturum özeti ile kurum içi gizli rapor aynı perspektif değildir. |
| 5 Renkli Indigo, Kod: 0, E.Y.Ö., The Progenitors | s. 6–10, Bölüm 8–12 | fiziksel s. 247–271 ve terim eşleşmeleri | Tasarım/mekanik içeriğinin oynanmış olduğu varsayılmamalı. |
| Birleştirilmiş karakter fihristi | s. 11–17, Bölüm 14.1–14.8 | karakter adı/Origin sayfaları CSV’de tüm 512 fiziksel PDF sayfasına göre taranır | Güncel fişin sayfa konumu ana referanstır; eski metin eşleşmeleri ek konumlardır. |
| Bağımsız düzyazı / evren içi medya | DOCX’te her zaman karşılığı olmayabilir | fiziksel s. 414–512 | Sahne ve forum/haber metinleri nesnel/oynanmış olay olarak otomatik kabul edilmez. |

## Önemli eşleştirme kararları ve açık noktalar

1. **Horizon Day:** DOCX s. 3 ve s. 16’ta Deneb’in öldürdüğünü söyleyen kayıtlar var; March/Arcturus’un gerçek fail oluşu kullanıcı kararı K-001 ile ayrılmıştır. PDF’de ilgili hedefli arama eşleşmeleri CSV satırında listelidir.
2. **Kintoki Sentaro:** DOCX Bölüm 7.4 s. 5’te ölüm; Bölüm 14.2 s. 11’de eskimiş “Yakında Ölecek” fişi. K-002 uyarınca ölüm kesin, bedenin nihai akıbeti açık.
3. **Caspian “Siren” Locke:** DOCX s. 14’te “İnhibitör” yazsa da K-004 ile güncel sınıf **Katalizör**; eski kaynak etiketi kaybolmamalı.
4. **Sylas/Sylan:** güncel ad Sylas; erken günlüklerde Sylan varyantı bulunur. Ayrı karakter kabulü için yeterli kanıt yok.
5. **GATE:** PDF fiziksel s. 5 ve 311’de “GATE (brigade)” ifadesi aranabilir; K-003 gereği mevcut kanonda bağımsız konsept değildir.
6. **T9:** DOCX s. 16’daki 14.6 başlığı, dokuz kişilik eksiksiz resmî roster olarak yorumlanmamalı; T9, F.O.R.A. ve mafya ayrı güç odaklarıdır.
7. **Origin kaydı ile karakter kaydı:** Aynı güç birden fazla karakter/kurum bağlamında görünüyorsa Origin satırı güç adını; karakter satırı karakter fişini izler. Bunlar bilinçli olarak tek satırda eritilmedi.
8. **PDF sayfaları:** bütün 512 fiziksel sayfa OCR metin katmanından tarandı; sayfa görüntülerinin tümü bu ad-indeks çalışmasında tek tek görsel olarak yeniden incelenmedi. OCR yazım hataları ve kısa terim eşleşmeleri ayrıca bağlam doğrulaması gerektirebilir.

## CSV alanları

- `Kategori`: Karakter, Origin/güç sistemi, kurum, coğrafya, olay veya FRP.
- `Kayıt`: okunabilir ana kayıt adı.
- `Diğer adlar / aranacak biçimler`: taramada kullanılan varyantlar.
- `Envanter bağlantısı`: v0.8 envanter bölümü/çelişki/karar ID’si.
- `Tam Arşiv v1.2 ana konumu`: öncelikli DOCX konumu.
- `Tam Arşiv v1.2 metin eşleşme sayfaları`: OCR değil, DOCX’ten oluşturulmuş 17 sayfalık kontrol PDF’sindeki fiziksel sayfalar.
- `Konuşma arşivi PDF ana konumu`: bilinen/başlangıçta yararlı sayfa çıpaları.
- `Konuşma arşivi PDF metin eşleşme sayfaları (fiziksel)`: `Abyss_OCR.pdf` içinde tüm 512 sayfada eşleşen fiziksel sayfalar.
- `PDF eşleşen sayfa adedi`: eşleşme sayısı; kararın doğruluk derecesi değildir.
- `İlişkili Origin / kayıt`: karakter-Origin ilişkileri veya ek bağlantı.
- `Statü / denetim notu`: çelişki, kullanıcı kararı, kapsam veya kaynak türü uyarısı.

## Sınır ve sonraki denetim

Bu dosya **kaynak konumu eşleştirme indeksi**dir; henüz her sayfadaki her cümlenin içerik denetimi ve tüm karakter fişlerinin karar/kanon onayı değildir. İlk sürüm, envanterdeki ana kayıt kümelerini ve v1.2’nin ayrıntılı karakter/Origin fihristini aranabilir fiziksel sayfa konumlarına bağlar. Bir sonraki turda CSV’de “Eşleşme bulunamadı” görünen kaynak adları ve alias ilişkileri, OCR sayfa görüntüsüyle bağlam bazında elle doğrulanabilir.


## v0.2 — İlk kaynak doğrulama turu

Bu sürümde `Origin sistemi`, `Katalizör`, `Aktivatör`, `İnhibitör`, `Anomali`, `Origin Felaketi`, `Mana`, `Nebula`, `Mana Çürümesi` ve `Evrim Sancısı` olmak üzere 10 kayıt pasaj düzeyinde incelenmiştir. Bu 10 kayıt için DOCX kanıtı, tamamlayıcı PDF kanıtı, kaynak türü ve açık noktalar CSV’ye yeni sütunlar olarak eklenmiştir. Diğer 292 kaydın v0.1 konum eşleşmeleri korunur ama pasaj düzeyinde henüz doğrulanmamıştır.

**Yeni ayrıntılı rapor:** `Abyss_Origin_Mana_Kaynak_Denetimi_v0.1.md`

**Sayfa numarası kuralı:** `PDF fiziksel s. 205 (iç sayfa 1/209)` ifadesinde fiziksel PDF sayfası ve konuşma içi sayfalama ayrı ayrı gösterilir. Kullanıcının açıklamasına göre `merged2pdf.pdf` ve `Abyss_OCR.pdf` aynı içerik kabul edilmiştir; tekrar OCR karşılaştırması yapılmamıştır.

### İlk turda korunan önemli ayrımlar

- Hostun Origin olmadan yaşayabilmesi, eski kullanıcı mesajında açıkça yazılıdır fakat v1.2 temel bölümünde tekrar edilmez; tamamlayıcı kullanıcı bilgisi olarak tutulur.
- Anomali’nin %1 oranı ve her kullanıcının bir noktada Anomali’ye evrilebilmesi aynı öncelikli paragrafta geçer; payda/zaman ölçeği açıklanmadığından yeni uzlaştırma üretilmemiştir.
- Origin Felaketi’nin v1.2’deki tetikleyicisi fiziksel/psikolojik çöküştür; daha eski kullanıcı notundaki iyileşme bağlantısı açık nokta olarak bırakılmıştır.
- “Evrim Sancısı” için ayrı mekanik bulunmadığından Mana Çürümesi’nin başlık/açıklaması olarak tutulmuştur.


## v0.3 — Kurumlar ve coğrafya kaynak denetimi

Bu sürümde kurum/örgüt kategorisindeki 21 kayıt ve coğrafya/yer kategorisindeki 16 kayıt olmak üzere 37 satırın kaynak bağlamı denetlendi. Öncelikli DOCX pasajları ile PDF’nin ilgili fiziksel sayfaları eşleştirildi; öneri metinleri, kullanıcı kararları, evren içi medya ve kanon dışı kaynak izleri birbirinden ayrıldı.

**Ayrıntılı rapor:** `Abyss_Kurum_Cografya_Kaynak_Denetimi_v0.1.md`

**Öne çıkan açık nokta:** DOCX s. 2’de Demir Şapel Rhodes’taki Dünya Ağacı köklerine yerleştirilirken PDF fiziksel s. 26’daki bir pasaj aynı adlı büyük şapeli din merkezine bağlayan bir bağlamda geçirebilir. Öncelikli kayıt Rhodes olarak kalır; ikinci bağlantı çözülmüş kabul edilmez. `F.M.S.`, `Praxis Bio-Catalyst`, `Vesper Industries` ve `Apex Dome` ise yalnızca asistan taslağı/öneri olarak kanon dışı statüde tutulur.


## v0.4 — Karakter kaynak denetimi

Envanterdeki 100 karakter kaydına DOCX ve konuşma PDF’sinden temsilî pasajlar, fiziksel sayfa konumları ve kaynak türü ayrımları eklendi. Bu tur, her karakterin bütün 512 sayfadaki her geçişinin veya bütün olaylarının görsel olarak denetlenmesi değil; her kayıt için kaynak bağlamı doğrulama turudur.

**Ayrıntılı rapor:** `Abyss_Karakter_Kaynak_Denetimi_v0.1.md`

**Önemli notlar:** Horizon/K-001, Kintoki/K-002 ve Caspian/K-004 kararları korundu; Sylas/Sylan yazımı, Vega/Tempest ayrımı ve Koç Yamino Kuni/Kael Vesper kimlik çakışması açıkça işaretlendi.
