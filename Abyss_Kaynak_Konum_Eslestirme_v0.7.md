# ABYSS — Kaynak Konum Eşleştirme İndeksi v0.7

**Bu sürüm:** Envanterden bağımsız ters taramanın ilk turu kaydedildi. Ana 302 kayıtlık eşleştirme tablosu değiştirilmedi; kaynaklarda görünen fakat ana indekste eksik veya yalnızca geniş olay kaydına gömülü öğeler ayrı aday defterinde tutuluyor.

## Yeni dosyalar

- [Envanter Açık/Kayıp Kayıtlar Raporu v0.1](Abyss_Envanter_Acik_Kayip_Kayitlar_v0.1.md)
- [Kayıp Kayıt Adayları v0.1 — CSV](Abyss_Kayip_Kayit_Adaylari_v0.1.csv)

## Ters taramanın kapsamı

- `Abyss_OCR.pdf` metin katmanı: 512 fiziksel sayfa.
- Öncelikli kaynak: `Abyss Evreni_ Tam Arşiv v1.2.docx`, 17 sayfa.
- Karşılaştırılan kayıt defteri: v0.6 CSV’deki 302 kayıt.
- Kullanıcı beyanı gereği `merged2pdf.pdf` ve `Abyss_OCR.pdf` aynı içerik sayıldı; OCR yeniden karşılaştırılmadı.

## İlk bulgular

- Beş kullanıcı-tanımlı A-sınıfı öğrenci (**Nari Velden, Tobias Krell, Elin Marr, Darian Solvek, Lilly Wisp**) ana indekste yok.
- **Poloz Will** kaynakta bir karakter ve güç taslağı olarak var; aynı bağlamda “Kael” yazımı da bulunduğundan birleştirme kararı bekliyor.
- **Leyra** ile **Commander Wooly**, kullanıcı kaynaklı konuşma/sahne öncüllerinde belirgin ama bağımsız karakter fişleri yok. Wooly suikastı isteği PDF s. 29’da ve metnin yinelenen sürümünde s. 323’te görünür.
- **Gridlock** adı ve beş kişilik ekip varlığı oyuncu metninde geçiyor; bireysel üye adları ve dramatik çatışma ayrıntıları asistan tarafından yazıldığı için doğrulanmış kabul edilmiyor.
- **Atum Abargil** anlatı sahnelerinde PDF s. 426 ve 494’te ve haber isteğinde s. 511–512’de geçiyor; mevcut tabloda yalnızca haber/olay satırına bağlanmış, bağımsız kişi kaydı yok.
- **Radian Exis Day**, **Pithou/Pithuo** ve **General Accel** mevcut karakterler için alias güncellemesi adayları.
- **Kasa-7/Vault-7, Null-Core, Sun-Wire, Thermal Leech** ana tabloda görev kaydına gömülü; bağımsız tesis/nesne fişleri açılması değerlendirilebilir.
- **Luda Oksana** gibi adlarda kimlik uyuşmazlığı ve **Selene/Sage Baez/Gridlock üyeleri** gibi asistan üretimi detaylar, ana indekse onaysız eklenmedi.

## Statü ve sınır

Bu yeni adaylar ana 302 kayıtlık CSV’ye otomatik işlenmemiştir. Aday defteri; kullanıcı kaynaklı eksik kayıtları, mevcut satırlara eklenebilecek alias’ları, geniş bir olay kaydı içinde kalan alt kayıtları ve yalnızca asistan metninde beliren taslakları ayırır. PDF’nin metin katmanı tüm 512 sayfada arandı; her sayfanın bütün görsel ayrıntıları baştan sona tek tek incelenmediğinden bu ilk tur nihai eksiksizlik garantisi değildir.

**Önceki ana eşleştirme tablosu:** `Abyss_Kaynak_Konum_Eslestirme_v0.6.csv` (302 kayıt; değişmeden korunur).
