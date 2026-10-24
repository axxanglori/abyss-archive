# ABYSS — Kaynak Bütünlüğü Denetimi v0.2

**İlk denetim tarihi:** 23 Ekim 2026  
**Sürüm notu:** v0.2, v0.1 bulgularını K-001–K-013 kararları ve yeni senkronizasyon kontrolüyle eşitler; tam satır-satır/görsel kapsama denetimi henüz tamamlanmadı.  
**Kapsam:** Kaynak dosyalarının kimliği ve yapısı, GitHub eşleşmesi, PDF sayfalama/kapsam haritası ve önceki raporlarda taşınan kritik çelişki/atıf kayıtları.

> Bu rapor, kaynakları değiştirmez ve yeni kanon kararı üretmez. Kaynakta görülen ifadeler ile daha sonra kullanıcı tarafından kesinleştirilmiş kararlar ayrı tutulur. “Doğrulanmadı” ifadesi, bir bilginin yanlış olduğu değil, bu turda yeterli kanıtla yeniden kontrol edilmediği anlamına gelir.

## 1. İncelenen kaynaklar

| Kaynak | Bu turda doğrulanan durum | Kullanım |
|---|---|---|
| `Abyss_OCR.pdf` | 512 sayfa; 239,300,940 bayt; şifreli değil. SHA-256: `64ba19902904af14c13aa02b6f358575ef32da05f31f4741c75cbee5a02f4497`. Metin araması yapılabiliyor; seçilmiş sayfalar render edildi. | Ana konuşma/kampanya kaynağı; ihtiyaç olduğunda sayfa görüntüsüyle kontrol edilir. |
| `Abyss Evreni_ Tam Arşiv v1.2.docx` | 17 sayfa; 37,041 bayt. SHA-256: `5e27919c5aabb927713b0da5c2ebdc926a32ce940202a0afaa4fee366bd89921`. Yerel dosyanın GitHub'daki DOCX blob'uyla **birebir aynı** olduğu doğrulandı. | Öncelikli lore referansı; içindeki başlık, karakter fişi ve bölüm notları kendi kaynak statüleriyle okunur. |
| `md_output/Abyss_Arsiv_Envanteri_v0.8.md` | GitHub `main` ağacında mevcut; kaynak haritası ve mevcut açık konuları içeriyor. | Dizin/çalışma haritası; tek başına kanon kaynağı değil. |
| `md_output/Abyss_Karar_Kaydi_v0.4.md` | GitHub `main` ağacında mevcut; K-001–K-004 kararları var. | Doğrudan kullanıcı kararlarının takibi. |
| `md_output/Abyss_Tam_Arsiv_v1.2_Karsilastirma_Raporu_v0.4.md` | GitHub `main` ağacında mevcut; ilk çapraz-kaynak karşılaştırması. | Önceki bulgular; bu denetimde bulunan durum güncellemeleri uygulanmalı. |

### Kaynak kimliği / GitHub

- Depo: <https://github.com/axxanglori/abyss-archive>
- Denetimde görülen `main` ağacı SHA: `ef1de4033f1d05f4bd382a6a1f1f0a9a0c8cba05`
- Tam Arşiv DOCX Git blob SHA: `602da01e9d43b8f276925fe30d674faa4b073d68` — yerel DOCX için hesaplanan Git blob SHA ile eşleşiyor.
- Envanter v0.8 blob SHA: `3c4eb80dc6c0ff3b0237c3649c0efc01f579dccf`
- Karar kaydı v0.4 blob SHA: `5ff73f0f97f2e5c3e644944ad7ba57b252f723eb`
- Karşılaştırma raporu v0.4 blob SHA: `d7217732b959da5df9d12883dc8b7c12ebab4493`

Bu eşleşme, yüklenen DOCX'in depodaki ana DOCX ile aynı dosya olduğunu doğrular; DOCX'in içeriğinin konuşma arşivinin tamamını kapsadığını **kanıtlamaz**.

## 2. Bulgular

### A-01 — Ana DOCX GitHub kopyasıyla aynı

**Durum: DOĞRULANDI**

Yerel `Abyss Evreni_ Tam Arşiv v1.2.docx` için hesaplanan Git blob SHA, GitHub ağacında bu dosyaya ait SHA ile aynı. Bu turda iki farklı DOCX sürümünü karşılaştırma riski görülmedi.

### A-02 — PDF'nin üç fiziksel bölüm hâlindeki sayfa haritası genel olarak doğrulanıyor

**Durum: ÖRNEKLEM KONTROLÜNDE DOĞRULANDI; tüm sayfalar tek tek denetlenmedi**

Render edilen ve metinleri kontrol edilen sınır sayfaları şu yapıyla uyumlu:

- Fiziksel PDF s. 1, ilk konuşma parçasının iç sayfalamasında `1/204` olarak işaretli.
- Fiziksel PDF s. 205, sonraki “Abyss Main” parçasının iç sayfalamasında `1/209` olarak başlıyor.
- Fiziksel PDF s. 413, bu ikinci parçanın `209/209` sayfası.
- Fiziksel PDF s. 414, *When the Sun eclipsed above Tombstone* başlıklı başka bir sahne metnine geçiyor.

Bu örnekler envanterdeki `1–204`, `205–413`, `414–512` ana bölüm haritasını destekliyor. Bununla birlikte, her sayfadaki alt başlıkların ve bütün içerik kayıtlarının eksiksiz eşleştirildiği anlamına gelmez.

### A-02a — Temel lore özetinin seçili maddeleri v1.2 ile örtüşüyor

**Durum: HEDEF ODAKLI ÖRNEKLEM KONTROLÜNDE DOĞRULANDI**

Envanter/karşılaştırma raporundaki seçili temel bilgiler, Tam Arşiv v1.2'nin ilgili bölümleriyle örtüşüyor: insanların %33'ünde Origin bulunması, Anomali için %1 oranı, Origin kullanıcılarında Mana Çürümesi için %30 oranı; Outlander'ların 17 kişi olarak tanımlanması; F.O.R.A.'nın beş üyesi ve Rhodes'un bağımsız sayılması; dört mafya ailesi/Joker yapısı; Siyah Kan'ın kısa vadeli güç artışı ve sonrasında Mana Çürümesi riski. Bu sonuç seçilen maddeler içindir; bütün envanter satırlarının doğrulandığı anlamına gelmez.

### A-03 — Sayfa referansı hatalı: fiziksel s. 320'nin iç sayfa numarası `116/209`

**Durum: DÜZELTME GEREKİYOR**

Envanter v0.8 ve karşılaştırma raporu v0.4, kaynak önceliği talimatını `fiziksel PDF s. 320` ve iç sayfalama `23/209` olarak gösteriyor. Görüntülenen fiziksel s. 320'nin alt bilgisinde ise **`116/209`** yazıyor. `23/209` iç numarası PDF'nin başka bir noktasında, fiziksel s. 227 civarında görünüyor.

**Önerilen düzeltme:** Kaynak hiyerarşisi atfını `Abyss_OCR.pdf, fiziksel s. 320 (Abyss Main iç sayfalaması: 116/209)` biçiminde yaz. Fiziksel PDF sayfası ile içeride basılı sayfa numarasını ayrı alanlarda tut.

### A-04 — `GATE (brigade)` ifadesinin fiziksel görünümleri iki adet

**Durum: SAYIM/ENVANTER AÇIKLAMASI GÜNCELLENMELİ; K-003 KARARI DEĞİŞMİYOR**

PDF metin aramasında `GATE (brigade)` ifadesi iki fiziksel konumda bulundu: s. 5 ve s. 311. İki yerdeki metin, Sylan/Sylas günlüğündeki aynı olaya ilişkin aynı ya da çok yakın bir pasaj gibi görünüyor; dolayısıyla bu iki eşleşme iki bağımsız kanıt olarak sayılmamalı.

Kullanıcı karar kaydı K-003'teki **“GATE mevcut kanonda ayrı bir konsept değil”** kararıyla çelişki yok. Düzeltilmesi gereken nokta, ham PDF'de yalnızca bir metinsel eşleşme varmış gibi yazılmasıdır.

**Önerilen envanter notu:** “`GATE (brigade)` ifadesi PDF'de iki fiziksel konumda yer alır (s. 5 ve 311); içerik aynı günlük pasajının tekrarı gibi görünür. Bu, ayrı/kanonik bir GATE kurumu olduğunu kanıtlamaz.”

### A-05 — Horizon Day kaydının “açık çelişki” durumu güncel karar kaydıyla senkron değil

**Durum: RAPOR DURUMU GÜNCELLENMELİ; K-001 ESAS ALINMALI**

Kaynak DOCX'te:

- Bölüm 5, Horizon'un Deneb tarafından öldürüldüğünü yazar.
- Aynı bölümdeki Sylas fişi, March/Arcturus'u Exis'in babasının “gerçek katili” olarak tanımlar.
- Bölüm 14.6'daki Horizon fişi yine Deneb'in öldürdüğünü yazar.

Karar kaydı K-001, bu ayrımı açıkça çözüyor: **gerçek katil March/Arcturus; kamuya yansıyan/Day ailesinin inandığı anlatı Deneb/September'ın katil olduğu.** Dolayısıyla kaynak dosyadaki iki kısa ifade tarihsel kaynak izi olarak kalmalı; güncel envanter ve rapor bu konuyu kullanıcı kararıyla çözülmüş kabul etmeli.

Buna rağmen karşılaştırma raporu v0.4'ün Bölüm 4'ü Horizon'u iki önemli açık çelişki adayından biri sayıyor; Bölüm 13 de kaynak tek başına ayrımı çözemiyormuş gibi yazıyor. Envanter v0.8'in Bölüm 13'ünde de benzer bir eski durum notu kalmış.

**Önerilen düzeltme:** Bu konu “açık çelişki” listesinden çıkarılsın; “kaynakta kamuya açık anlatı / gizli gerçek ayrımı kullanıcı kararı K-001 ile netleşti” biçiminde iz bıraksın.

### A-06 — Kintoki'nin ölümü ile bedeninin akıbeti birbirinden ayrılmalı

**Durum: ÖLÜM ÇÖZÜLDÜ; BEDENİN NİHAİ AKIBETİ AÇIK**

Tam Arşiv v1.2'nin Bölüm 7.4'ü Kintoki'nin Bowling Faciası'nda öldüğünü anlatırken, Bölüm 14.2 karakter fişinde “Yakında Ölecek” yazıyor. Karar kaydı K-002 bunu doğru biçimde ayırıyor: Kintoki öldü; bedeni ailesine teslim edilmedi; F.O.R.A. araştırmayı sürdürdü ve aile boş tabut gömdü. F.O.R.A.'nın bedenle en sonunda ne yaptığı ise hâlâ açık.

Karşılaştırma raporu v0.4'ün Bölüm 4'ü Kintoki konusunu hâlâ ikinci “önemli çelişki adayı” olarak topluyor. Bu, K-002 ile senkronize edilmeli.

**Önerilen düzeltme:** “Kintoki'nin ölüm durumu çözüldü; eski ‘Yakında Ölecek’ etiketi kaynak geçmişinde korunur. Açık soru yalnızca bedenin nihai akıbeti ve araştırmanın sonucudur.”

### A-07 — Tam Arşiv v1.2'nin kendi bölüm yapısında iki yapısal not var

**Durum: KAYNAK YAPISI DOĞRULANDI; İÇERİK EKSİĞİ OLDUĞU KANITLANMADI**

DOCX'in bölüm başlıklarında Bölüm 12'den Bölüm 14'e geçiliyor; **Bölüm 13 başlığı yok**. E.Y.Ö. ölçeği, Bölüm 10'un ardından bağımsız bir blok olarak geliyor ve Bölüm 12'de yeniden anlatılıyor. Bunlar içerik düzeni/numaralandırma özellikleridir. Bölüm 13'ün hangi içeriğe sahip olması gerektiği tahmin edilmemeli; tekrarlanan E.Y.Ö. blokları da sürüm geçmişi anlaşılmadan silinmemeli.

### A-08 — Caspian “Siren” Locke için kaynak/karar farkı korunmalı

**Durum: KARAR KAYDI KAYNAK ETİKETİNİ AÇIKÇA DÜZELTİYOR**

Tam Arşiv v1.2 Bölüm 14.4'te Caspian “İnhibitör” olarak etiketli. Karar kaydı K-004, bunun kullanıcı tarafından karıştırılarak yazıldığını ve doğru sınıfın **Katalizör** olduğunu kaydediyor.

**Öneri:** Kaynak DOCX'i geriye dönük değiştirme. Güncel karakter fişinde Katalizör kullan; eski kaynak etiketini kaynak geçmişi/not olarak koru.

### A-09 — Host'un Origin olmadan yaşayabileceği ifadesi, öncelikli DOCX'te açıkça yazmıyor

**Durum: KAYNAK DESTEĞİ EKSİK; KESİN KURAL OLARAK SUNULMAMALI**

Envanter v0.8'in 3.1 bölümünde “İnsan (host) Origin olmadan yaşayabilir” ifadesi yer alıyor. Tam Arşiv v1.2 Bölüm 1.1 ise Origin'in host olmadan yaşayamadığını ve Origin ile insanın birlikte doğup öldüğünü söylüyor; fakat bir Origin'in alınması/ölmesi durumunda insan host'un hayatta kalacağını açıkça belirtmiyor. Bu çıkarım doğru olabilir, ancak mevcut birincil metin tek başına yeterli kanıt sağlamıyor.

**Önerilen düzeltme:** Şimdilik asimetrik bağımlılık kuralını yalnızca kaynakta açıkça yazıldığı biçimde kaydet: “Origin host olmadan yaşayamaz; host ile birlikte doğup ölür.” Host'un Origin kaybından sonra yaşayıp yaşayamayacağı ayrı bir `[AÇIK SORU]` olsun veya konuşma arşivinde bunu açıkça belirleyen kullanıcı cümlesine bağlansın.

### A-10 — GitHub deposundaki OCR metinlerinin adları ve kökenleri net değil

**Durum: TAKİP GEREKİYOR**

GitHub `main` ağacında birden fazla OCR/metin kopyası bulunuyor:

| Dosya yolu | Boyut (bayt) | Bu turdaki not |
|---|---:|---|
| `Abyss_OCR.txt` | 2,668,906 | Depo kökünde; envanterde ayrı bir kaynak olarak açıklanmıyor. |
| `md_output/Abyss_1-204_OCR.txt` | 721,078 | İlk 204 sayfanın eski/ayrı OCR metni. Örnek satırlarda belirgin OCR bozulmaları var. |
| `md_output/Abyss_OCR_TumMetin.txt` | 2,810,474 | Envanterin arama/inceleme kopyası olarak tanımladığı tam metin. |
| `Abyss_OCR.pdf` | Depoda görünmüyor | Bu sohbetin yüklemesi olarak mevcut; GitHub ağacında yok. |
| `merged2pdf.pdf` | Depoda görünmüyor | Envanterde özgün kaynak olarak anılıyor; bu turda dosya olarak karşılaştırılamadı. |

Bu metin dosyalarının birbirinin aynısı, farklı OCR sürümleri veya farklı kapsamlar olduğu bu turda tam olarak doğrulanmadı. Özellikle iki ana metin dosyasının kökeni ve hangisinin hangi PDF sürümünden üretildiği bir manifestte yazılmalı. Büyük kaynak PDF'lerin GitHub ağacında olmaması, depoyu **tek başına tam bir kaynak yedeği** olarak görmememiz gerektiği anlamına geliyor.

### A-11 — Önceki OCR karşılaştırma istatistikleri bu turda bağımsız yeniden hesaplanmadı

**Durum: DOĞRULANMADI; YANLIŞ OLDUĞU SÖYLENMİYOR**

Envanter v0.8'deki 95.158 kelime farkı, 1.726.620 karakterlik eşleşme ve yaklaşık %90,1 OCR benzerliği gibi ölçümler önceki çalışmanın bulguları olarak yazılı. Ancak özgün `merged2pdf.pdf` bu oturumda yüklenmemiş ve GitHub dosya ağacında bulunmuyor. Dolayısıyla bu turda iki PDF'yi baştan karşılaştırarak sayıları doğrulamak mümkün olmadı. Raporlarda bunlar “önceki karşılaştırma sonucu; bu turda yeniden hesaplanmadı” olarak belirtilmeli.

## 3. Durum özeti

| Başlık | Sonuç |
|---|---|
| Ana DOCX'in GitHub eşleşmesi | **Doğrulandı** |
| PDF sayfa sayısı ve ana segment sınırları | **Örneklem kontrolünde doğrulandı** |
| PDF s. 320 iç sayfa numarası | **23/209 değil, 116/209 — düzelt** |
| GATE metinsel görünümü | **İki fiziksel konum; muhtemel tekrar; K-003 kararı değişmiyor** |
| Horizon Day | **K-001 ile çözüldü; rapordaki eski “açık çelişki” işareti güncellenmeli** |
| Kintoki Sentaro | **Ölüm çözüldü; bedenin nihai akıbeti açık** |
| Caspian | **Güncel sınıf Katalizör; DOCX'teki İnhibitör etiketi tarihsel kaynak izi** |
| OCR TXT kopyalarının kökeni | **Açık** |
| 512 sayfanın her satırının envanterde bulunup bulunmadığı | **Henüz tam kapsam denetimi yapılmadı** |

## 4. Kaynak önceliği ve işlem kuralları

1. `Abyss Evreni_ Tam Arşiv v1.2.docx` öncelikli lore kaynağıdır; ancak bu, onun tüm sohbet arşivini kelimesi kelimesine kapsadığı anlamına gelmez.
2. `Abyss_OCR.pdf` tamamlayıcı konuşma/kampanya kaynağıdır. Oyuncu günlükleri, kullanıcı kararları, Gemini/ChatGPT önerileri, sahne taslakları, kurgu içi haberler ve oynanmış olaylar ayrı statülerle tutulmalıdır.
3. Kullanıcı karar kaydındaki K-001–K-004 hükümleri güncel kararlardır. Kaynakların eski/yanlış ifadeleri silinmez; güncel bilgiye giden bir notla işaretlenir.
4. OCR metni arama yardımcısıdır; ad, sayı, güç kuralı veya kritik olay gerektiğinde PDF sayfası ve/veya öncelikli DOCX kontrol edilir.
5. Kaynakta bulunmayan ayrıntılar tamamlanmış gibi yazılmaz. “Bulunamadı”, “bu turda yeniden doğrulanmadı” ve “çelişiyor” farklı statülerdir.

## 5. Bu turda yapılmayanlar

- 512 fiziksel sayfanın tamamını envanter maddeleriyle satır satır karşılaştırmak.
- Özgün `merged2pdf.pdf` ile OCR PDF arasındaki eski istatistikleri yeniden hesaplamak.
- `Abyss_OCR.txt`, `Abyss_OCR_TumMetin.txt` ve `Abyss_1-204_OCR.txt` dosyalarını bütün satırlarda karşılaştırmak.
- Bütün karakter, Origin, kurum, yer ve olay kayıtlarını tek tek kaynak sayfasına bağlamak.
- Açık kanon kararlarını kullanıcı adına çözmek.

Bu nedenle bu dosya, kaynak bütünlüğü denetiminin **ilk tur raporudur**; arşivin eksiksizliğine dair garanti değildir.

## 6. Kaynak bağlantıları

- [GitHub deposu](https://github.com/axxanglori/abyss-archive)
- [Envanter v0.8](https://github.com/axxanglori/abyss-archive/blob/main/md_output/Abyss_Arsiv_Envanteri_v0.8.md)
- [Karar kaydı v0.4](https://github.com/axxanglori/abyss-archive/blob/main/md_output/Abyss_Karar_Kaydi_v0.4.md)
- [Karşılaştırma raporu v0.4](https://github.com/axxanglori/abyss-archive/blob/main/md_output/Abyss_Tam_Arsiv_v1.2_Karsilastirma_Raporu_v0.4.md)
- [Tam Arşiv v1.2 DOCX (GitHub)](https://github.com/axxanglori/abyss-archive/blob/main/Abyss%20Evreni_%20Tam%20Ar%C5%9Fiv%20v1.2.docx)
- `Abyss_OCR.pdf`: fiziksel s. 320; sayfa alt bilgisinde `116/209`. Bu PDF bu sohbetin eki olarak mevcut; GitHub ağacında bulunmuyor.


## v0.2 durum güncellemesi — güncel kararlarla çapraz kontrol

Bu bölüm, v0.1’deki denetim bulgularının yerine geçmez; hangi bulguların yeni sürümlerde işlendiğini, hangilerinin hâlâ açık kaldığını belirtir.

### Güncel dosyalarla eşleştirilenler

- **A-05 / Horizon Day:** K-001 güncel karardır: gerçek katil March/Arcturus; kamuya yansıyan anlatı Deneb/September’dır; gerçeği yalnızca Deneb ile Arcturus bilir. Güncel kaynak konum eşleştirme indeksi v2.8 bunu doğru statüde taşır. Horizon’u yalnızca “açık çelişki” diye işaretleyen eski rapor sürümleri yine de ayrıca güncellenmelidir.
- **A-06 / Kintoki Sentaro:** K-002’ye göre ölüm çözülmüştür; bedeni ailesine verilmemiş, F.O.R.A. araştırması sürmüş ve aile boş tabut gömmüştür. Bedenin nihai akıbeti ile araştırmanın sonucu hâlâ açıktır. Güncel kaynak indeksi bu ayrımı taşır; eski “yakında ölecek” roster metni tarihsel kaynak izi olarak korunur.
- **A-08 / Caspian “Siren” Locke:** Güncel sınıf Katalizör; DOCX’teki İnhibitör etiketi tarihsel/eski yanlış etiket olarak korunur.
- **K-013 / The Progenitors:** Aile adları ile ata Origin adları farklı katmanlardır. Yedi eşleşmenin temel işlevleri kullanıcı kararıyla netleşmiştir; Day ailesi Animus uzantısıdır ve sekizinci aile değildir. Kaynak eşleştirme indeksi v2.8 bu güncellemeyi içerir.
- **99 kayıtlık güç denetimi:** `Abyss_Origin_Guc_Denetimi_99_Kayit_Takip_v1.9.csv` tam 99 veri satırına sahiptir. Her satırda DOCX/PDF kanıt alanları doludur. Bu, tüm satırların her sayfa görünümünün görsel olarak doğrulandığı veya bütün mekaniklerin çözüldüğü anlamına gelmez.

### Yeni bulunan ve düzeltilen kapsam tutarsızlığı

- **Kategori toplamı:** Ana indeks `Abyss_Kaynak_Konum_Eslestirme_v2.8.csv` 319 satır ve sekiz kategori içerir. Önceki kapsam matrisi v0.3 yedi normal kategori toplamıyla 318’e ulaşıyor, indeksteki 1 adet `Tarihsel taslak / Origin denemesi` kategorisini toplamda göstermiyordu. Bu satır `Abyss_Kaynak_Kapsam_Matrisi_v0.4.csv` sürümüne eklendi; sekiz kategori toplamı 319 olarak eşitlendi.
- **Literal PDF eşleşmesi / Kael ve koç:** K-006 kimlik ayrımını çözmüştür: öğrenci Kael “Sonar” Vesper ile Koç Yamino “Furiko” Kuni ayrı kişilerdir. PDF’de yalnızca eski “Koç Kael Vesper” ifadesinin bulunması, kimlik ilişkisinin hâlâ belirsiz olduğu şeklinde yazılmamalıdır. Nihai çalışma adları ise kullanıcının notuna göre açık kalır.
- **Ouroboros:** K-008 ile güncel Origin olmadığı, Isolde Vance (çalışma adı) için önceki deney/taslak olduğu kesinleşmiştir. DOCX s.14’teki kaynak izi korunur; PDF’de literal terim eşleşmesi bulunmaması kayıt silinmesini gerektirmez.

### Hâlâ açık kalan bulgular

- Host’un Origin olmadan yaşayabileceği iddiası, öncelikli DOCX’te açık bir kural olarak desteklenmiyor; yeni kullanıcı kararı veya açık kaynak pasajı olmadan kesin kanon kabul edilmemelidir.
- OCR dosyalarının GitHub’daki ad/köken ilişkisi ve önceki OCR karşılaştırma istatistikleri bağımsız olarak yeniden doğrulanmış değildir.
- PDF 512 fiziksel sayfadır; görsel kontrol örneklem bazlı kalır. 512/512 sayfanın görsel olarak satır satır denetlendiği ileri sürülmez.
- Bu v0.2, yerel `/mnt/data` çalışma dosyalarını senkronize eder. Burada yerel kopyası bulunmayan eski GitHub raporlarının uzaktan değiştirilmiş olduğu iddia edilmez.
