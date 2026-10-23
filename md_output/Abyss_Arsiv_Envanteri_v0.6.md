# ABYSS — Arşiv Envanteri v0.6

**Durum:** OCR karşılaştırması tamamlandı; Tam Arşiv v1.2 birincil kaynak; kullanıcı kararları K-001, K-002 ve K-003 işlendi. Kintoki’nin ölümü kesin; bedeninin F.O.R.A. tarafından sonrasında ne yapıldığı açık karar olarak duruyor. GATE mevcut kanonda ayrı bir konsept değil; konuşma arşivindeki tekil ifade kaynak notu olarak tutuluyor ve ancak gelecekte geliştirilecek fikir statüsünde.  
**Kaynak dosyaları:** `Abyss Evreni_ Tam Arşiv v1.2.docx` (17 sayfa; öncelikli referans), `merged2pdf.pdf` (özgün konuşma arşivi, 512 sayfa, 88,6 MiB) ve `Abyss_OCR.pdf` (aranabilir OCR sürümü, 512 sayfa, 228,3 MiB). `Abyss_OCR_TumMetin.txt` arama/inceleme kolaylığı sağlayan türetilmiş metin kopyasıdır.  
**Amaç:** Arşivde nelerin bulunduğunu belirlemek, kaynak türlerini ayırmak ve sonraki kanon belgelerine güvenilir bir yol haritası sağlamak.

> **Önemli uyarı:** Bu dosya bir kanon özeti değildir. Burada geçen hiçbir madde yalnızca bu envantere girdiği için kesinleşmiş kanon sayılmaz. Kullanıcı notları, Gemini önerileri, oyuncu günlükleri ve sahne taslakları farklı türde kaynaklardır. Aralarındaki ayrımlar sonraki aşamada tek tek kaydedilecektir.

## Kaynak önceliği — kullanıcı tarafından belirlenmiş kural

512 sayfalık konuşma arşivinin fiziksel s. 320 bölümünde (Gemini konuşmasının kendi sayfalamasında 23/209) kullanıcı, “Abyss Evreni: Tam Arşiv v1.2” dosyasını açıkça birinci öncelikli kaynak olarak tanımlıyor; dosya ile sohbet arasında çelişki varsa dosyanın doğru kabul edilmesini, dosyada bulunmayan sohbet bilgisinin ise ek kaynak olarak korunmasını istiyor. Bu dosya artık yüklendiği için bu kural uygulanabilir.

1. **Öncelikli referans:** `Abyss Evreni: Tam Arşiv v1.2.docx`. Çelişen sohbet kaydı, kendi başına v1.2'yi değiştirmez.
2. **Tamamlayıcı arşiv:** `merged2pdf.pdf` / `Abyss_OCR.pdf`. v1.2'de bulunmayan sohbet ayrıntıları korunur; fakat kaynak türü ve durumu (kullanıcı kararı, oyuncu günlüğü, oynanmış olay, plan, Gemini önerisi, ChatGPT önerisi vb.) kaybolmaz.
3. **v1.2 içindeki çelişkiler:** Belge kendi içinde çelişiyorsa bu öncelik kuralı tek başına yeterli değildir. İlgili iki ifade de saklanır ve `[ÇELİŞKİ—AYNI KAYNAK]` olarak işaretlenir; kullanıcı onayı olmadan biri seçilmez.
4. **Türetilmiş OCR metni:** `Abyss_OCR_TumMetin.txt` arama ve sayfa bulma içindir; bağımsız ya da daha üstün bir kaynak değildir. Özel ad ve kural doğrulaması gerektiğinde sayfa görüntüsü ve asıl DOCX/PDF kontrol edilir.

## 1. Teknik durum ve kapsama

- Özgün PDF `merged2pdf.pdf`: 512 sayfa, 92.942.222 bayt (yaklaşık 88,6 MiB), şifresiz.
- Kullanıcının OCR sürümü `Abyss_OCR.pdf`: 512 sayfa, 239.300.940 bayt (yaklaşık 228,3 MiB), şifresiz ve ilk 204 sayfada artık aranabilir metin katmanına sahip.
- Sayfa sayısı ve sırası korunmuş görünüyor. Fiziksel sayfa 1–204'te OCR metni eklenmiş; özgün PDF'de bu sayfalar için normal metin çıkarımı boştu.
- Özgün PDF'den çıkarılabilen metin toplam 233.073 kelimeydi (esas olarak fiziksel s. 205–512). OCR PDF'den 328.231 kelime çıkarılıyor. Fark olan **95.158 kelime**, OCR PDF'nin ilk 204 sayfasından alınan metne karşılık geliyor.
- Fiziksel s. 205–512 için iki PDF'den alınan metin, boşluklar normalize edildikten sonra birebir eşleşti: 1.726.620 karakter ve 233.073 kelime. Bu, OCR sürümünün önceki metin katmanını değiştirmediğini gösteren güçlü bir metin karşılaştırmasıdır.
- İlk 204 sayfa için önceki ayrı OCR çıktım (`Abyss_1-204_OCR.txt`) 96.470 kelime içeriyordu. Kullanıcının PDF'sinden alınan metinle sayfa bazında ortalama normalize benzerlik yaklaşık %90,1; kelime sayıları aynı ölçek aralığında. Bu oran doğruluk puanı değildir, yalnızca iki OCR metninin örtüşmesini ölçer. Örnek kontrollerde kullanıcının PDF'si Türkçe karakterleri ve noktalama işaretlerini daha okunaklı koruyor; yine de özel adlar ve kurgu terimleri manuel doğrulama gerektirebilir.
- Tam metin çıkarımı, her fiziksel PDF sayfasını ayıran bir dosya olarak da saklandı: `Abyss_OCR_TumMetin.txt`.

**Sonuç:** İlk 204 sayfa artık aranabilir ve envantere alınabilir. Bu, her OCR kelimesinin hatasız olduğu anlamına gelmez; özellikle özel adlar, kurgusal terimler, İngilizce/Türkçe geçişleri ve diyalog içindeki hitaplar gerektiğinde özgün sayfa görüntüsüyle kontrol edilmeli.


### Yeni eklenen öncelikli kaynak: Tam Arşiv v1.2

- Dosya: `Abyss Evreni_ Tam Arşiv v1.2.docx`; 17 sayfa, yaklaşık 37 KB. Belge metin tabanlıdır ve okunabilir.
- Bu, 512 sayfalık sohbet arşivinin bir parçası değil; ayrı bir “ana kaynak / güncellenmiş lore kitabı”dır. Kullanıcının arşivde açıkça verdiği kaynak hiyerarşisine göre çelişki çözümünde öncelik v1.2'dir.
- Bölüm düzeni: 1–5 temel evren ve tarihçe; 6 güncellenmiş karakter fihristinin 14. bölüme taşındığına dair tarihsel not; 7 oturum günlükleri; müdüriyet içi gizli rapor; 8 beş renkli Indigo boss tasarımı; 9 Kod: 0; 10 De Paul/Mitsuki geçmişi; E.Y.Ö. ölçeği; 11 The Progenitors; 12 E.Y.Ö.'nün ikinci sunumu; 14 birleşik NPC/karakter arşivi. Belge numaralamasında 13. bölüm görünmüyor; bu, eksik/çıkarılmış bölüm olasılığı olarak kaydedildi, içeriği uydurulmadı.
- İçerik statüsü tek tip değil: kurallar, kampanya günlüğü, kurum içi rapor, boss mekaniği ve geniş karakter fihristi aynı belgede. Başlığın “Tam Arşiv” olması, içindeki her paragrafın aynı anlatı statüsünde olduğu anlamına gelmez.

## 2. Belgenin kaynak katmanları

### A. Fiziksel sayfalar 1–204 — Kampanya günlüğü, sezon değerlendirmeleri ve GM hazırlıkları

Kullanıcının OCR PDF'si sayesinde bu bölümün tamamında aranabilir metin mevcut. Aşağıdaki harita sayfa gruplarındaki ana konuları gösterir; bir aralıkta farklı sahneler veya öneriler iç içe geçebilir.

| Fiziksel PDF sayfaları | İçerik haritası | Statü açısından dikkat |
|---|---|---|
| 1–8 | Birinci yıl/sezon değerlendirmesi; ikinci yıl için öneriler; Eli'nin günlük devamı; Sylan/Sylas'ın 25.09.2041–08.10.2041 günlüğü. Lapis-7, oyuncu günlüğünde bir kez geçen “GATE (brigade)” ifadesi, Anastasia ile karşılaşma, March'la yeraltı işi, PvP ve parti içi güven kaybı. | Günlükler oyuncu perspektifidir; Gemini değerlendirmeleri ayrı yorum katmanıdır. GATE ifadesi tek başına ayrı bir kurum/konseptin kanıtı değildir; kullanıcı K-003'te GATE'in mevcut kanon olmadığını belirtti. “Sezon 2 / birinci yıl” gibi etiketler kronolojiyle çapraz kontrol edilmeli. |
| 9–18 | Sakamoto Akademisi'ne mafya saldırısı için offscreen dövüş taslağı: Spor öğretmeni Kuro Falls'ın Spades Joker'i olması, Ryuichi'yi ve Creation Origin'i hedefleyen operasyon; September/Deneb ile çatışma; Eos'un cenaze/offscreen anlatısı ve rekabet eden haber bültenleri. | İlk dövüş taslağında September'a yanlış biçimde vektör manipülasyonu verilmiş; kullanıcı bunu açıkça düzeltiyor. Düzeltilmiş sürüm esas alınmalı. |
| 19–23 | Yeni sezon görev panosu, F/E/S benzeri görev seviyeleri, seviye ve görev tasarlama kuralları; Google Drive'daki “Abyss Evreni: Tam Arşiv v1.2” belgesine başvurma ve ana kaynak önceliği talimatı. | Görev taslakları oynanmış işlerle aynı şey değil. Atıf yapılan Tam Arşiv v1.2 bu 512 sayfalık dosyaya ekli değil. |
| 24–30 | Şehirler ve bölgeler kodeksi; F.O.R.A.'nın beş üyesi (T.O.W.E.R., Tokyo, Verdun, Peru, Helenaport) ve bağımsız Rhodes; T.O.W.E.R. katmanları, aileler ve şehir kültürleri; T.O.W.E.R. ve alternatif medya/haber akışları; Ryuichi ve komutanlar hakkında propaganda metinleri. | Kurgu içi haberleri nesnel anlatı olarak değil, belirli kurumların veya yayınların bakışı olarak etiketle. |
| 30–35 | Gideon–Kaelen yıl sonu maçı; Kaelen'in “Sütür” ve Kara Kan bağlantılı antagonist motivasyonu; Elara'nın olası uyanışı; 3. ve 4. sınıfa uzanan kampanya kancaları; görev/operasyon geliştirme. | Birçok unsur gelecek sezon fikri olarak önerilmiş; oynandığı teyit edilmeden [PLAN] veya [ÖNERİ] statüsünde kalmalı. |
| 35–42 | Mafyanın akademi saldırısı için GM sahnesi; Anastasia Day ve özel timi; Ryuichi'nin kaçırılması ve Creation Origin'i host ölümü şartıyla çıkarabilen cihaz; F.O.R.A./Brigade, yeraltı mafyası ve T9 arasındaki güç üçgeni. | Sayfa 40'ta kullanıcı, **T9'un F.O.R.A.'nın altında olmadığını; T9, mafya ve F.O.R.A.'nın üç ayrı güç odağı olduğunu** açıkça düzeltiyor. |
| 42–46 | Dünya inşası yaklaşımı: kelebek etkisi, gündelik dehşet, sistem içindeki yanlış insanların etkisi; Fate Core uyarlaması; High Concept, Relationship, Trouble, World Aspects ve Invoke/Compel kullanım örnekleri. | Bunlar FRP masa kuralları ve GM ilkeleri; evrenin diegetik kanonundan ayrı belgelenmeli. |
| 46–62 | Exis–Anastasia mesajlaşmaları ve uzun anne-oğul sahneleri; Anastasia'nın eğitim tarzı, geçmişi ve askeri otoritesi; Exis'in Sora Amamiya ile randevu/romantik sahneleri; September'ın Exis'e sorumluluk, hedef ve irade üzerine dersleri. | Bir kısmı oyuncu kararından sonra üretilen devam sahneleri, bir kısmı önerilen diyalogdur; masa kayıtlarıyla doğrulanmalı. |
| 62–75 | Outlander'ların kökeni ve “Kutsal 17” hakkındaki alternatif açıklamalar; Perde'nin amacı; Kara Kan'ın kimyası ve Fate Core Consequence'larıyla ilişkisi; ateş/ışık Originlerinin silinmesi teorisi; Boy King, mafya ve F.O.R.A. üçgeni; Asa'nın mektupları/hafızası ve Exis'in hedef olması gibi kancalar. | Kullanıcı, yalnızca çığlık atma/nefretle yetinmeyen bir Outlander motivasyonu arıyor; Kara Kan tarifi de ilk taslak/karar ayrımıyla kaydedilmeli. |
| 76–84 | Kaelen'in antagonist felsefesi; Gideon, Elara ve Sütür; Kara Kan ihtiyacı ve “Kusursuz Kesik” travması; 3. sezon/3. sınıf olasılıkları. | Olay zincirlerinin önemli kısmı GM tarafından tasarlanan olasılık ve foreshadowing'dir, kesinleşmiş olay değildir. |
| 85–100 | Exis ve Anastasia'nın aile/askeri eğitim sahneleri; sınıf ve dünya tarihi dersleri için “Kutsal 17”, ateş/ışık Originleri ve Mana Çürümesi anlatısı; Exis'in güç ve etik sınırlarını sınayan antrenman. | Bazı içerikler ders önerisi ya da offscreen rol yapma metnidir. |
| 101–105 | C-seviyesi iş/job tasarımları; bürokratik, teknik/çevresel ve psikolojik görev örnekleri; Apex Dome, seçkinlerin katılımı ve kan/mana yemini töreni. | Görev ve tören konseptlerini kampanya panosu, gerçekleşmiş sahne ve fikir havuzu olarak ayrı kayıtlarla tut. |
| 106–120 | Sylas'ın Gage ve Vanya ile ilişkili yüksek riskli sızma/soygun senaryosu; Kasa-7/Vault-7, Null-Core, Sun-Wire, Thermal Leech, kütle/cep boyutu ve zamanlayıcı tabanlı kaçış; sahne içinde oyuncuya verilen karar anları. | Bir kısmı “oyun yöneticisi olarak oyuncuya verilecek metin” ve taktik sahne taslağıdır. Her satırı gerçekleşmiş kampanya olayı sayma. |
| 121–138 | Kara Kan'ın zehriyle ilişkili kampüs/parti sonrası olayları; Asa, Eli, Exis, Sylas, Fleur ve Agatha'nın durumları; yaralanma, hastane ve gizli ajanda sahneleri; September'ın uyarıları ve karakterler arası sorgulamalar. | Bazı neden-sonuç ilişkileri, özellikle kimin neyi bildiği, ayrı bir olay çizelgesinde izlenmeli. |
| 139–150 | Sylas ile March/Arcturus arasında karanlık geçmiş, koruma, T9 ve Outlander tehlikesi üzerine uzun bir sahne; March'ın hem koruyucu hem geçmişte şiddet işlemiş biri olarak sunulması. | Kimlik/alias bağları ve hangi açıklamanın Sylas'a ne zaman verildiği gizli bilgi olarak işaretlenmeli. |
| 151–160 | Ay isimli T9 karakterlerinin anlamı; mevsim temaları ve T9 Dokuzlu yapısı; Ambrossa ve September'ın dersleri; anomaliler, dışlanmışlar, rezonans ve mana pilleri; F.M.S., Praxis Bio-Catalyst, Vesper Industries; yeni job tasarımları. | Kullanıcı 12 kişilik öneriyi reddedip T9'un dokuzlu oluşunu ve mevsim temasını koruyor. Job taslaklarında “öncekilere çok benzer” eleştirisi var; beğenilmeyen teklifler kanon değildir. |
| 161–171 | Exis'in iyileşme/yaralanma süreci etrafındaki diyaloglar; Sylas ile Fleur gibi ilişkiler; kurumun öğrenci/ajanları sınıflandırması için Prime, Fringe ve üçüncü kategori adı üzerine iterasyon. | Üçüncü kategori için “Blackbox” yerine kullanıcının seçtiği **Rogue** güncellemesi takip edilmeli. |
| 172–190 | İkinci sınıfın ikinci dönemine geçiş; sezon finalinin ölçeği ve uzun soluklu altı yıllık akademi yapısı; F.O.R.A.–mafya ittifakı, T9'un nüfuz ağı, September'ın devre dışı bırakılması, Creation, Kara Kan, Mitsuki ve Indigo projesi çevresindeki planlar; March'ın olası ileriki ölümü. | Kullanıcı T9'u oyuncu grubunun düşmanı olarak konumlandırmıyor ve September'ın kötü biri olmadığını özellikle düzeltiyor. March'ın ölüm zamanlaması olasılık olarak geçiyor. |
| 191–204 | “Reality but Unreal” başlıklı sezon/arc planı; Verdun zirvesi, Ruru'nun ortadan kaybolması, Kara Kan/mafya cephesi, Sylas için oyuncu seçimi ve bekleme süresi; rüya/uyanış çizgisi, Babylon Ekspresi, sezon finali ve Anastasia–Deneb yüzleşmesi için Discord lore-drop sahnesi. | Haftalık bölüm taslağı ile oynanmış sahneler ayrılmalı. 204. sayfadaki Anastasia–September yüzleşmesi sahne metni, tek başına olayın masada gerçekleştiğini kanıtlamaz. |

Bu bölümün yalnızca evren ansiklopedisi olmadığı netleşti: oyuncu günlükleri, DM değerlendirmeleri, iş listeleri, Fate Core ev kuralları, sahne yazımı, kurgu içi haberler ve sezon planları aynı akışta bulunuyor. Bunlar farklı koleksiyonlarda tutulmalı.

### B. Fiziksel sayfalar 205–413 — “Abyss Main” konuşma arşivi ve ana dünya kurma notları

Bu bölüm, evrenin temel kavramlarının ilk açık anlatımlarını ve uzun Gemini konuşma dizisini içeriyor. İçinde hem kullanıcı tarafından yazılmış dünya notları hem de Gemini'nin fikirleri, yorumları ve sahne taslakları var.

Öne çıkan içerikler:

- Deneb, Horizon ve Anastasia'nın çocukluk/geçmiş anlatıları.
- Origin, mana, Origin türleri, Mana Çürümesi ve Origin Felaketi.
- Perde, Outlander'lar ve İkiz Tanrıçalar Euruyn/Morygnn.
- T9, F.O.R.A., T.O.W.E.R., Verdun, Rhodes ve diğer devletler.
- Karakter aileleri, hükümdar kökenleri ve güç aileleri için birden çok isimlendirme/versiyon.
- Sakamoto Koleji, sınıf hiyerarşileri, eğitmenler ve NPC veri tabanları.
- FRP kampanyası için görev tasarımları, silah ruhsatı testi, turnuva eşikleri, sınıf olayları ve sezon finalleri.
- Kara Kan, Indigo Çocuk Projesi, F.O.R.A. yayın/istihdam indeksleri ve T9'un mevsimsel doktrini.

Bu bölümde 261 adet `User prompt:` ve 261 adet `Response:` işaretçisi metin çıkarımında bulundu. Bu sayı, evrende 261 ayrı karar bulunduğu anlamına gelmez; yalnızca arşivdeki konuşma işaretçilerinin yaklaşık sayısıdır.

### C. Fiziksel sayfalar 414–512 — Hikâye sahneleri, gizli kayıtlar ve evren içi medya

Bu bölümde konuşma notlarından daha doğrudan sahne/metin biçimine geçen materyal bulunuyor:

- *When the Sun eclipsed above Tombstone* başlıklı, gizli arşiv/kamera kaydı biçiminde bir sahne.
- September/Deneb, Anastasia ve T.O.W.E.R. çevresindeki karakter odaklı düzyazı ve diyaloglar.
- F.O.R.A., mafya, Indigo çocukları ve Kara Kan çevresindeki komplo/olay örgüsü parçaları.
- **Abyss-Net** günlük akışı ve yeraltı forumu biçimindeki evren içi yayınlar.
- Atum Abargil'e yapılan saldırıyla ilgili son dakika haber taslağı.

Bu bölüm için “ana olay örgüsü”, “sahne taslağı”, “gizli belge” ve “evren içi medya” etiketleri ayrı tutulmalı. Kurgu içi bir haber, nesnel anlatıcı tarafından doğrulanmış bir olayla aynı kaynak türü değildir.


### D. Atıf yapılan fakat bu paket içinde bulunmayan ana kaynak

Fiziksel s. 22–26 arasında kullanıcı, “Abyss Evreni: Tam Arşiv v1.2” belgesine dayanarak şehir/lokasyon kodeksini geliştirmeyi ister; bu fiziksel sayfalarda ana dosyanın kendisi yer almaz. Kaynak önceliği talimatı daha sonra PDF fiziksel s. 320’de (Gemini konuşmasının iç sayfalamasında 23/209) daha açık biçimde ifade edilmiştir. v1.2 DOCX’i artık ayrıca yüklendi ve bu envanter sürümünde karşılaştırmaya katıldı; eski kaynak eksikliği giderilmiştir.

## 3. Evrenin temel kavram haritası

Aşağıdaki maddeler arşivde doğrudan anlatılan notların tasnifidir; henüz nihai kanon kararı değildir.

### 3.1 Origin ve mana

- **Origin:** İnsanların içinde bulunan ve olağan dışı yetenekler sağlayan mana küresi/yaşam formu olarak tarif ediliyor. Notlarda insan nüfusunun yaklaşık %33'ünün Origin kullanıcısı olduğu söyleniyor.
- **Host–Origin ilişkisi:** İnsan (host) Origin olmadan yaşayabilir; Origin ise host olmadan yaşayamaz ve onunla doğup ölme eğilimindedir. Originlerin hayatta kalma içgüdüsü kuralların merkezinde yer alıyor.
- **Origin türleri:**
  - **Katalizör:** Kullanıcının dışındaki varlıkları/şeyleri etkileme veya manipüle etme.
  - **Aktivatör:** Kendi bedenine etki etme/manipüle etme.
  - **İnhibitör:** Canlılar üzerinde enzim restorasyonu/iyileştirme.
  - **Anomali:** İlk üç gruptan birine sığmayan veya birkaçını farklı oranlarda barındıran durum.
- **Anomali oranı ve gelişimi:** Notlarda kullanıcıların yaklaşık %1'inin anomali olduğu söylenirken, her Origin kullanıcısının psikolojik/kişisel gelişim veya gerileme sonucunda anomali eşiğine gelebileceği de belirtiliyor. Bu iki ifadenin aynı anda tam olarak nasıl işleyeceği netleştirilmeli.
- **Mana ve nebulalar:** Mana, dünyanın/varoluşun özü olarak anlatılıyor; fiziksel olarak nebulalarda bulunuyor. Kullanıcılar dinlenerek mana yenileyebiliyor, nebulalar anlık destek sunabiliyor. Başka bir notta mananın geceleri daha yoğun olduğu belirtiliyor.

**Kaynak başlangıcı:** Fiziksel PDF s. 205–207.

### 3.2 Mana Çürümesi ve Origin Felaketi

- **Mana Çürümesi:** Kullanıcı, kapasitesinin çok üzerine çıkmak zorunda kaldığı fiziksel/psikolojik kırılma anında bu hastalığa yakalanabiliyor. Yenileme haznesi zamanla işlev kaybediyor; kullanıcı günden güne zayıflıyor. İleri aşamada beden ya da Origin manayı absorbe edemez duruma gelebiliyor ve ölüm/kullanamama riski doğuyor.
- **Görünür belirti:** Saçların, kaşların ve kirpiklerin beyazlaması; notlarda diğer yüz kılları da belirtiliyor.
- **Sıklık:** İlk notta Origin kullanıcılarının yaklaşık %30'u ile ilişkilendiriliyor. Bu yüksek oran bilinçli bir dünya kuralı mı, taslak oran mı teyit edilmeli.
- **Origin Felaketi:** Originin kendi varlığını sürdürme içgüdüsüyle hostun fiziksel/psikolojik durumuna sert tepki vermesiyle ilgili yıkıcı olay. Her Origin Felaketinin Mana Çürümesiyle aynı şey olduğu varsayılmamalı.
- **Toplumsal sonuçlar:** Devlet hastaneleri/araştırmaları, bağımsız dernekler ve çürümenin çaresini arayan gizli/karanlık bir organizasyon fikri geçiyor; bu fikirlerin hangilerinin mevcut kanon olduğu ayrılmalı.

**Kaynak başlangıcı:** Fiziksel PDF s. 206–207; konu daha sonraki sayfalarda tekrar ele alınıyor.

### 3.3 Deneb ve Origin manipülasyonu

- Deneb'in yeteneği salt Origin çalma değil, doğrudan **Origin manipülasyonu** olarak açıklanıyor; bu, bir Origin'i çalabilmesi ve belirli koşullarda aktarabilmesi için temel gerekçe.
- Çaldığı Origin'in asıl hostu hayatta kalırsa yaklaşık **7 dakika** sonra Origin'in asıl hosta dönmesi gerektiği not edilmiş.
- Asıl host ölürse Origin'in Deneb'de kalabildiği söyleniyor.
- Deneb'in aktarım yapabildiğini kendisinin baştan bilmediği, bu beceriyi Horizon'un ölümü ve sonrasındaki trajik olaylarda keşfettiği anlatılıyor.
- İkiz Tanrıçaların soy/ritüel yoluyla aktarımı ile Deneb'in anomaliden kaynaklanan manipülasyon/aktarım olasılığı aynı mekanik kabul edilmemeli.
- Felix'in Deneb'e bıraktığı “yedek” Origin ve bunun gerçek potansiyelinin ne kadarının bilindiği ayrıca izlenmeli.

**Kaynak başlangıcı:** Fiziksel PDF s. 205–207; ilgili karakter veritabanı ve sonraki hikâye parçalarıyla birlikte okunmalı.

### 3.4 Perde ve Outlander'lar

- Outlander'lar Rhodes çevresindeki **Perde'nin** ardındaki küre/boyutla ilişkili varlıklar olarak anlatılıyor.
- İlk notlarda eskiden insan oldukları; çoğunun Mana Çürümesiyle ilişkili olduğu; Perde'nin ardında dönüşüm geçirseler de zekâ ve bilinçlerini korudukları yazıyor.
- Perde arkasında mana yerine Perde'den akan sınırsız bir enerji kullanabildikleri belirtiliyor.
- Sayılarının başlangıçta 17 olduğu ve artıp azalabileceği not edilmiş.
- Liderlerinin amaçlarından biri çürümenin çaresini aramak olarak anlatılırken, sonraki bölümlerde Abyss'i kendi kurallarıyla yönetme/dönüştürme yönünde farklı öneriler de var. Bunların tek bir motivasyona birleştirilmesi için karar gerekiyor.
- İnsanların çoğu Outlander'ların varlığını bilmiyor; bilen azınlığın da ne olduklarını tam kavramadığı belirtiliyor.

**Kaynak başlangıcı:** Fiziksel PDF s. 206–207; başka açıklamalar ilerleyen dünya kurma bölümünde.

### 3.5 İkiz Tanrıçalar, Ambrossa, Rigel ve Blackthorn

- **Euruyn:** Doğa/mevsimler temalı Origin; kendi soyuna Origin aktarımı ve pembe saçlı soy işaretiyle ilişkilendiriliyor.
- **Morygnn:** Kozmos, yıldızlar ve muhtemel gelecekleri görme ile ilişkilendiriliyor; kendi gücünü seçtiği varise aktarma ritüeli olduğu anlatılıyor.
- **Ambrossa:** Yalanları gerçeğe dönüştürme/gerçekliği bükme temalı Origin. Morygnn'ın seçilmiş varisi olarak yetiştiriliyor ancak gizlice bir Origine sahip olduğu için ritüel sırasında Morygnn'ı öldürüyor; ardından Outlander lideriyle anlaşması ve mührün gelecekte kırılması anlatılıyor.
- **Rigel / Altın Leydi:** Rhodes yöneticisi; Euruyn'un soy/Origin mirasıyla ilişkili. Dünya Ağacı ve Rhodes Kilisesi onun hikâyesinin merkezinde.
- **Vega / December:** Rigel'ın kız kardeşi, T9 ile bağlantılı. Sonraki karakter veritabanında “Tempest” adı geçiyor; farklı notlardaki güç terminolojisi karşılaştırılmalı.
- **Lord Blackthorn:** Perde/Ağaç/şapel çevresinde mühürlü Outlander. Rigel ile aralarında kapının/mührün durumuna bağlanan simbiyotik bir ilişki olduğu belirtiliyor.
- **Dünya Ağacı:** Rhodes'un güneyindeki dev ağaç; Perde mührüyle ve bölgenin kavurucu güneşinden gölgelik sağlamasıyla ilişkilendiriliyor.

**Açık düğüm:** Rigel'ın mühürlenmesi, Blackthorn'un serbest kalması ve Perde'nin açılması arasındaki koşulların tam mantığı bazı notlarda tersine dönmüş/karmaşık görünüyor. Sonraki kaynaklar karşılaştırılmadan bu ilişkiyi tek cümlelik kesin kurala dönüştürmeyelim.

**Kaynak başlangıcı:** Fiziksel PDF s. 207–208.

### 3.6 Siyasi harita ve kurumlar

- **F.O.R.A.:** Beş devletli ittifak olarak tarif ediliyor: T.O.W.E.R., Verdun, Peru, Tokyo ve Helenaport. Avrupa Birliği/NATO benzeri işlev benzetmesi yapılıyor.
- **Rhodes:** İttifak dışında kalıyor. T.O.W.E.R., Verdun ve Rhodes aynı kıtada; Tokyo ve Helenaport merkez kıtadaki Wastelands çölüyle; Peru ise daha seyrek yerleşimli başka bir kıtayla ilişkilendiriliyor.
- **T.O.W.E.R.:** Üç katmanlı şehir/düzen; Fildişi Kulesi katmanları bağlıyor. En üst kat gelişmiş ve ayrıcalıklı; ikinci kat rekabetçi ve sert; en alt kat yoksulluk ve kargo/sahil işlevleriyle tarif ediliyor.
- **Sakamoto Koleji:** T.O.W.E.R.'ın üst katındaki ünlü Origin koleji; Mitsuki Sakamoto ile ilişkili. Farklı sınıf yılları ve 1-S/1-A gibi gruplar kampanya materyallerinde önemli.
- **Verdun:** Gece hayatı, kaçakçılık/gizli laboratuvar/askerî araştırma ve dağlık tarımsal bölgelerle tarif ediliyor; lideri Boy King olarak veriliyor.
- **Rhodes:** Yunan mimarisi etkisi, siyah kumlu sahiller, doğayla iç içe ama teknolojik yaşam, Dünya Ağacı ve kilise/şapel merkezleriyle anlatılıyor.
- **T9:** Darbe girişimi, gizli operasyonlar, kimlik gizleme ve güç aileleriyle bağlantılı eski elit örgüt. Mitsuki'nin liderliği bazı karakter veritabanı kayıtlarında açıkça yazıyor.
- **GATE:** Tam Arşiv v1.2 içinde ayrı bir konsept olarak yer almıyor. 512 sayfalık konuşma arşivinin başındaki bir oyuncu günlüğünde yalnızca bir kez “GATE (brigade)” ifadesi geçiyor. Kullanıcı kararı K-003 uyarınca GATE, mevcut kanonda ayrı bir kurum/konsept değildir; ileride değerlendirilebilecek fikir olarak kaydedilir. Bu tekil günlük ifadesinden kurumsal yapı veya Brigade ile kesin ilişki çıkarılmayacak.

**Kaynak başlangıcı:** Fiziksel PDF s. 206–208 ve 247–250; ilgili kurum tasarımları ilerleyen sayfalarda da geçiyor.

## 4. Kampanya ve anlatı haritası

### Oyuncu karakterleri ve ilişkiler

Arşivde öne çıkan PC/NPC başlıkları: **Exis Day, Eli, Asa, Seth, Sylas, Fleur, Adriana, Agatha, Yuri, Radius, Elohim, Orelia, Corvus, Gideon, Kintoki, Kaelen, Elara, Ryuichi** ve diğer öğrenciler/üst sınıflar.

Önemli yetişkin/arka plan karakterleri: **Deneb/September, Horizon Day, Anastasia Day, Mitsuki Sakamoto, Felix Dux, Eos, March/Arcturus, Ruru Wagna, Rigel/Altın Leydi, Vega/December, Ambrossa, Lord Blackthorn, Lord Pestilence, Boy King** ve F.O.R.A./T9/mafya liderleri.

Bu isim listesi tam roster değildir; karakter veritabanında daha geniş sınıf, akademi, yetişkin, mafya ve Outlander kayıtları bulunuyor.

### Kampanya omurgası olarak görünen unsurlar

- Birinci yıl sonu değerlendirmesi ile daha sonraki ikinci sınıf/ikinci dönem planlaması aynı arşivde. Fiziksel s. 188'de kullanıcı, artık 1. sınıfta olmadıklarını ve 2. sınıfın ikinci döneminde olduklarını özellikle hatırlatıyor; daha eski yanıtların “1. sınıf” dilini ileriye taşımamak gerekir.

1. Sakamoto Koleji'nde 1-S sınıfının oluşumu; her oyuncunun birbirinden farklı geçmişi ve gizli motivasyonu.
2. A/S sınıfı rekabeti, disiplin cezaları, sınavlar, turnuvalar ve okul görevleri.
3. F.O.R.A. düzeni ve kurumların öğrenci/Origin kullanıcılarını sınıflandırması.
4. Seth–Ambrossa anlaşması; güven kaybı ve parti içi çatışma.
5. Eos'un ölümünden sonra devlet propagandası ve gerçeğin örtülmesi.
6. Indigo Çocuk Projesi ve Origin kopyalama/karıştırma araştırmaları.
7. Deneb'in September kimliğiyle öğrencilerden gizlenmesi; Horizon, Anastasia ve Exis'le bağlantılı ana trajedi.
8. Kara Kan, mafya ağları ve T.O.W.E.R. katmanları arasında kurulacak olay örgüsü.
9. T9, F.O.R.A., Outlander'lar ve iktidar dengelerinin sezonlar boyunca çatışması.

### Açık kullanıcı düzeltmeleri ve tercihleri (ilk 204 sayfada)

Bu maddeler, Gemini'nin daha önceki bir taslağını düzeltmek veya bir tercihi netleştirmek amacıyla kullanıcı tarafından açıkça yazılmıştır. Bunlar öneri gibi ele alınmamalı; ilgili konu işlenirken sonraki bağlamı belirleyen güçlü kaynaklardır:

1. **September/Deneb'in gücü:** İlk dövüş taslağındaki vektör manipülasyonu yanlıştır. Kullanıcı, September'ın Origin'inin “zaman çarkı” içinde geriye gitme/backup, saldırıyı durdurma ve tekrar etme ile ilgili olduğunu belirtiyor (s. 12–17). Düzeltilmiş sahne bu kurala göre yazılmalı.
2. **T9'un kurumsal konumu:** T9, F.O.R.A.'nın alt kuruluşu değildir; F.O.R.A., mafya ve T9 üç ayrı güç odağıdır (s. 40–42).
3. **T9'un sayısı ve teması:** Kullanıcı 12 kişilik taslağı reddedip dokuzlu (T9) sayısını ve mevsim temasını koruyor (s. 153–155); üye dağılımı yine de nihai roster karşılaştırması ister.
4. **T9'un oyuncularla ilişkisi:** Kullanıcı, T9'un oyuncu grubuna düşman olmadığını açıkça söylüyor (s. 178).
5. **September'ın ahlaki konumu:** Kullanıcı, September'ın kötü biri olmadığını ve Deneb'in geçmişinin dikkate alınması gerektiğini belirtiyor (s. 187). Onu düz bir kötü karakter olarak yazan öneriler bu düzeltmeye aykırıdır.
6. **Indigo Çocuk Projesi:** Kullanıcı, projenin Origin kopyalama ve çaprazlama projesi olduğunu netleştiriyor (s. 184); başka genel “genetik çocuk” tanımları tek başına yeterli değil.
7. **F.O.R.A. ajan kategorileri:** A/Prime, B/Fringe sonrası C kategorisi için “Blackbox” yerine “Rogue” seçiliyor (s. 167–171). “Blackbox” önceki taslak etiketi olarak arşivde tutulmalı.
8. **Outlander motivasyonu ve Kara Kan:** Kullanıcı Outlander'ların yalnızca bağıran/nefret eden kurbanlar değil, kendi düzenleriyle Abyss'i yönetmek veya dönüştürmek isteyen bir aktör olması fikrini tartışıyor; Kara Kan ise Perde faunasından yaratık cesetlerinden damıtılan maddenin Origin kullanıcısı kanıyla füzyonu olarak tarif ediliyor ve Consequence'lara iyi gelip iyileşmeyi hızlandırması fikri yazılıyor (s. 63–66). Ayrıntılar nihai mekanik olarak ayrı ayrı denetlenmeli.

### Görev / oturum tasarımı türleri

- Sessiz Arşiv, Star Killer teslimatı, biyolojik atık temizliği, kayıp kan/medikal lojistik gibi görevler.
- Silah ruhsatı ve psikolojik/sadakat testi.
- Zihin labirenti, dikey kuşatma, hükümdar arenası gibi turnuva aşamaları.
- T.O.W.E.R. kör nokta/silah simülasyonu ve sınıf içi Origin testleri.
- Okul dersleri aracılığıyla verilen dünya tarihi, ikiz tanrıçaların anlatısı, Mana Çürümesi ve Originlerin evrimi.

**Önemli ayrım:** Bu başlıkların bir bölümü oynanmış oturum özeti, bir bölümü Gemini'nin gelecek oturum önerisi. Ayrıştırma yapılmadan hepsini “gerçekleşmiş olay” olarak kullanmamalıyız.

## 5. Karakter veritabanları ve sürüm riski

Arşivde hem **“Abyss Evreni — Karakter Veritabanı (Sürüm 1.0)”** hem **“Tam Karakter Veritabanı (Sürüm 2.0)”** başlıkları bulunuyor (fiziksel PDF s. 247–250 civarı). Sürüm 2.0 daha geniş bir taksonomi içeriyor:

- Oyuncu karakterleri — Sakamoto 1-S.
- Sakamoto Koleji 1. sınıflar ve üst sınıf elitleri.
- Twin Tides Akademisi (rakip okul).
- Eğitmenler ve okul yönetimi.
- T9, F.O.R.A. ve sistem liderleri.
- Mafya liderleri/Jokerler.
- Outlander'lar.

**Kural:** Sürüm 2.0 otomatik olarak 1.0'ın yerini almış sayılmayacak. Silinen, eklenen, isim değişikliği yapılan veya gücü değişen karakterler için sürüm fark tablosu açılmalı.

## 6. İlk çelişki / belirsizlik adayları

Bunlar şu aşamada “hata” değil; yan yana tutulması ve kaynakların karşılaştırılması gereken düğümlerdir.

| ID | Konu | Neden takip edilmeli? | Sonraki işlem |
|---|---|---|---|
| C-001 | Sezon/yıl adlandırması | İlk bölümün ilk sayfasında “ikinci sezon” denirken Gemini yanıtında “Sezon 1 / ikinci yıl” ifadesi kullanılıyor. | Gerçek zaman çizelgesini ve masa sezonu/yıl ayrımını netleştir. |
| C-002 | Origin türleri ve “Sovereign Origins” | Katalizör/Aktivatör/İnhibitör/Anomali sınıflaması ile aile/hanedan temelli “Sovereign Origins” listeleri aynı taksonomi mi, farklı eksenler mi belli değil. | “Kullanım tipi” ile “soy/çekirdek Origin” ayrımı önerisini test et. |
| C-003 | Yedi/sekiz hükümdar Origin listeleri | Sakamoto, Simo, Dux, Frenze, Minamoto, Sterling, Quinn ve Day farklı listelerde farklı isimlerle geçiyor; bazı adlar alternatif veya eski sürüm olabilir. | Ad, aile, Origin adı, işlev ve kaynak sütunları olan karşılaştırma tablosu üret. |
| C-004 | Mana Çürümesi oranı | Yaklaşık %30 ifadesi var; bunun tüm Origin kullanıcılarını mı, belirli koşullardaki kullanıcıları mı kapsadığı belirsiz. | Payda ve hastalığın yaygınlık/ilerleme oranını doğrula. |
| C-005 | Anomali oranı | Yaklaşık %1 denirken herkesin belirli koşullarda anomali eşiğine gelebileceği de anlatılıyor. | “Doğuştan anomali” ile “sonradan anomalileşme”yi ayır. |
| C-006 | Origin aktarım koşulları | Tanrıçaların soy/ritüel aktarımı, Deneb'in manipülasyonu ve Felix'in yedek Origin'i ayrı mekanizmalar olabilir. | Üç mekanizmayı ayrı kural olarak yaz ve ortak sınırlarını belirle. |
| C-007 | Rigel–Blackthorn–Perde mührü | Kapalı kapı, Rigel'ın mühürlenmesi ve Blackthorn'un serbest kalması arasındaki koşulların bazı notlarda anlaşılması zor. | Olayı ön koşul → sonuç diyagramıyla yeniden kur; kararı kullanıcı verir. |
| C-008 | Outlander motivasyonu ve “17” | Çürümenin çaresini arama, dünyayı yönetme/dönüştürme ve mühürlenmiş 17 kişinin tarihi aynı dosyada farklı ağırlıklarla ele alınıyor. | Liderin amacı, diğer Outlanderların amaçları ve halk efsanesini ayır. |
| C-009 | Black Blood'ın kapsamı | Hem madde/ilaç/iyileşme hızlandırıcı hem de mafya ticareti ve kampanya olayı olarak kullanılıyor. | Üretim, etki, risk, dağıtım ve olay kronolojisini tek sayfada birleştir. |
| C-010 | Ad/alias ve Origin adları | Exis/Radius, Sylas/Sylan OCR, March/Arcturus, Deneb/September, Vega/December gibi çift adlar geçiyor. | Her çift için “gerçek ad / takma ad / dönüşüm / OCR hatası / henüz belirsiz” alanı aç. |
| C-011 | GATE ifadesinin statüsü | Tam Arşiv v1.2’de GATE yoktur; konuşma arşivindeki bir oyuncu günlüğünde “GATE (brigade)” ifadesi bir kez geçer. | Çözüm: GATE mevcut kanonda ayrı bir konsept değildir. Tekil günlük ifadesi kanon kurmaz; kullanıcı isterse gelecekteki fikir olarak geliştirilebilir (K-003). |
| C-012 | Oynanmış olay ile öneri | Gemini yanıtları gerçekleşmiş olayları yorumluyor ve hemen ardından gelecek olaylar öneriyor. | Her olay kaydına [OYNANDI], [PLAN], [ÖNERİ] statüsü ekle. |
| C-013 | September'ın güç tanımı | İlk Kuro sahnesi vektör manipülasyonu yazar; kullanıcı bunu açıkça reddedip zaman çarkı/backup ve saldırıyı durdurma-tekrarlama mekaniklerini açıklıyor. | Kullanıcı düzeltmesini esas al; yalnızca hangi sınırların kesin olduğu belirsizse soru listesine taşı. |
| C-014 | T9–F.O.R.A. hiyerarşisi | Bazı sahne önerileri T9'u devlet/askeri yapı ile iç içe anlatabilir; kullanıcı T9'un F.O.R.A.'nın altında olmadığını özellikle belirtiyor. | Ayrı güç odağı ve bağlantı/ittifak ilişkilerini ayır. |
| C-015 | Kampanyanın hangi sınıfta/yılda olduğu | Erken sayfalar sezon 1/2 ve birinci yıl dilini kullanırken s. 188 kullanıcı 2. sınıfın ikinci döneminde olduklarını söylüyor. | Her kayıt için kaynak tarihi ve masa içi zaman noktası ekle; geç dönem kullanıcı düzeltmesini zaman çizelgesine yerleştir. |
| C-016 | T9'un dokuzlu ve mevsim kodları | Kullanıcı 12 kişilik öneriyi reddediyor; dokuzlu ve mevsim temasını tutuyor. Her ay/mevsim kodunun hangi üyeye bağlandığı tüm kayıtlarla karşılaştırılmalı. | T9 roster'ında sayı, alias, mevsim/birim, görev ve kaynak sütunları aç. |
| C-017 | Üçüncü ajan kategorisi | “Blackbox” önceki seçenek, “Rogue” ise kullanıcının tercih ettiği ad. | Güncel dokümanlarda Rogue kullan; Blackbox'ı eski adlandırma olarak işaretle. |
| C-018 | Indigo Çocuk Projesi'nin tanımı | Kullanıcı s. 184'te amaç kopyalama ve Origin çaprazlamasıdır diye düzeltiyor. | Proje tanımında bu formülasyonu kaynak notuyla kullan; ayrıntıları sonraki kaynaklarla eşleştir. |
| C-019 | “Abyss Evreni: Tam Arşiv v1.2” ana kaynağı | 512 sayfalık PDF bu dosyanın öncelikli olduğunu söylüyordu; dosya artık yüklendi ve ilk çapraz-kaynak denetimine alındı. | **Kaynak eksikliği giderildi.** Kullanıcı kuralını uygula; v1.2 ile çelişen sohbet ayrıntısını değişiklik olarak değil, kaynak farkı olarak kaydet. |
| C-020 | Sylas/Sylan yazımları | İlk günlüklerde “Sylan”, diğer bölümlerde “Sylas” geçiyor. Bu, OCR veya eski karakter adı olabilir. | Oyuncu/karakterin tercih edilen yazımını bir kez onayla; kaynak yazımını tarihsel kayıtta sakla. |
| C-021 | Kuro/September sahnesinin statüsü | Kuro'nun akademiye sızması ve Deneb ile dövüşü ayrıntılı biçimde yazılmış ama sahne offscreen taslağıdır. | GM notu olarak tut; oynandı kaydı gelmedikçe [PLAN]/[SAHNE TASLAĞI] statüsünde bırak. |

## 7. Önerilen ana bilgi tabanı

Sonraki aşamada bu envanterden şu ana belgeler türetilebilir:

1. **00 — Abyss Ana İndeks ve Karar Kaydı:** kaynak önceliği, kanon statüleri, açık sorular ve değişiklik günlüğü.
2. **01 — Kozmoloji ve Origin Sistemleri:** mana, Origin sınıfları, Anomali, Mana Çürümesi, Origin Felaketi, aktarım kuralları.
3. **02 — Coğrafya, Devletler ve Kurumlar:** kıtalar, ülkeler, F.O.R.A., T.O.W.E.R., Rhodes, Verdun, T9 ve kaynaklarda geçen Brigade kayıtları. GATE ayrı kurum olarak eklenmez; yalnızca kanon dışı gelecek fikri olarak izlenir.
4. **03 — Karakterler, Soylar ve Kronoloji:** karakter fişleri, aileler, aliaslar, ilişkiler, olay tarihi ve sürüm geçmişi.
5. **04 — Kampanya ve Oturum Arşivi:** 1-S/1-A, günlükler, görevler, oyuncu kararları, NPC olayları, sezon değerlendirmeleri ve GM hazırlıkları.

Büyük özgün PDF ayrı ve değiştirilmeyen **kaynak arşiv** olarak saklanmalı. Bu beş belge, PDF'nin yerine geçmez; hızlı erişim için hazırlanmış, kaynak sayfalarına geri dönen çalışma belgeleri olur.

## 8. Kaynak statüsü ve yazım standardı

Her kayıt şu alanlarla tutulmalı:

- **ID:** ör. `ORIGIN-001`, `CHAR-DENEB-001`, `EVENT-EOS-001`.
- **İfade:** bilginin kısa ve net tanımı.
- **Kaynak:** PDF fiziksel sayfa numarası; mümkünse iç konuşma tarihi/başlığı.
- **Kaynak türü:** kullanıcı notu / oyuncu günlüğü / oynanmış olay özeti / Gemini önerisi / ChatGPT önerisi / hikâye taslağı / evren içi belge.
- **Durum:** `[KANON-ONAYLI]`, `[KULLANICI NOTU—ONAY BEKLİYOR]`, `[ÖNERİ—GEMINI]`, `[ÖNERİ—CHATGPT]`, `[OYNANDI]`, `[PLAN]`, `[ÇELİŞKİ]`, `[ESKİ SÜRÜM]`, `[AÇIK SORU]`.
- **Bağlantılar:** ilişkili karakter, Origin, kurum, olay ve diğer kayıt ID'leri.
- **Değişiklik geçmişi:** önceki ifade, yeni ifade, karar tarihi ve gerekçe.

### Kanon koruma kuralı

Kullanıcıya ait notların içinde de taslak, soru ve ihtimaller bulunabilir. Bu nedenle “kullanıcı yazdı” tek başına “kanon onayı var” demek değildir. Açık bir kesinleştirme yoksa, ilgili madde `[KULLANICI NOTU—ONAY BEKLİYOR]` olarak kalmalıdır.

## 9. Bu aşamanın sonucu ve kalan iş

Bu güncellemede kullanıcı tarafından OCR yapılmış ikinci PDF, özgün PDF ve daha önce oluşturduğum ilk 204 sayfa OCR metni karşılaştırıldı. İlk 204 sayfa için aranabilir metin artık mevcut ve ana konu haritası envantere işlendi. 205–512 aralığındaki çıkarılabilir metin OCR PDF'de özgün PDF ile birebir aynı normalize metni veriyor.

Henüz yapılmamış olanlar: ilk 204 sayfadaki her özel adın ve her sahne ayrıntısının özgün sayfa görüntüsüne göre satır satır doğrulanması; bütün 512 sayfadan tam karakter/Origin/kurum/yer/olay veri tabanının çıkarılması; karakter veritabanı 1.0 ile 2.0 farklarının tek tek karşılaştırılması; ve kaynak içindeki önerilerin oynanmış olaylardan ayrılması. Bu envanter ayrıntılı bir dizin ve işlem haritasıdır, nihai kanon ansiklopedisi değildir.

**Güncellenmiş işlem sırası:**

1. OCR PDF'den alınan tam metni arama/kaynak metni olarak kullan; belirsiz özel adlarda özgün PDF görüntüsüne dön.
2. Bütün kaynaklardan kişi, Origin, kurum, yer ve olay adlarını ID'li envantere çıkar.
3. 1.0/2.0 karakter veritabanlarını karşılaştır; eski ad ve aliasları koru.
4. Origin/kozmoloji kurallarını ve kurum/coğrafya tanımlarını kaynak sayfalarıyla düzenle.
5. Her kural ve olay için [KANON-ONAYLI], [KULLANICI NOTU—ONAY BEKLİYOR], [ÖNERİ—GEMINI], [ÖNERİ—CHATGPT], [OYNANDI], [PLAN], [ÇELİŞKİ] veya [ESKİ SÜRÜM] statüsü belirle.
6. Öncelikli Tam Arşiv v1.2 artık mevcut; ilk fark tablosu hazırlandı. Sonraki adım, iç çelişkileri kullanıcının kararıyla çözmek ve bütün karakter/Origin kayıtlarını v1.2 + sohbet arşivi kaynaklarıyla ayrıntılı biçimde eşlemek.

## 10. OCR karşılaştırması — v0.2 (önceki teknik rapor korunmuştur)

| Ölçüt | Özgün PDF | Kullanıcının OCR PDF'si | Sonuç |
|---|---:|---:|---|
| Sayfa sayısı | 512 | 512 | Eşit |
| Dosya boyutu | 88,6 MiB | 228,3 MiB | OCR sürümü yaklaşık 2,58 kat büyük |
| Metin çıkarımı | 233.073 kelime | 328.231 kelime | Aradaki 95.158 kelime ilk 204 sayfanın metninden geliyor |
| Fiziksel s. 205–512 | 233.073 kelime | 233.073 kelime | Boşluklar normalize edilince tüm çıkarılmış metin birebir eşleşiyor |
| Fiziksel s. 1–204 | Aranabilir metin yok | 95.158 kelime | Kullanıcının OCR'si eksik metin erişimini gideriyor |

Önceki OCR metniyle yapılan karşılaştırma yaklaşık %90,1 ortalama normalize sayfa benzerliği gösterdi; bu, birbirinden farklı iki OCR çıktısının ne ölçüde örtüştüğünü gösterir ve bağımsız OCR doğruluk ölçümü değildir. Yeni OCR PDF'si, örnek kontrollerde daha okunaklı Türkçe karakterlerle tam metin araması için tercih edilmelidir. Ham OCR metni, OCR hatalarının izlenebilmesi ve gerektiğinde kaynak sayfaya dönülebilmesi için korunmalı.


## 11. Tam Arşiv v1.2 — öncelikli kaynak içerik haritası

### 11.1. Temel mekanikler ve kozmoloji (DOCX s. 1–2)

- **Origin:** İnsanların %33'ünde bulunan, mana küresi/başka yaşam formu olarak tanımlanır; host olmadan yaşayamaz. Sınıflar Katalizör, İnhibitör, Aktivatör ve %1 olarak belirtilen Anomaliler/Jokerlerdir. Her kullanıcının psikolojik durumuyla bir noktada Anomali'ye evrilebileceği de yazılıdır.
- **Origin Felaketi:** Hostun fiziksel/psikolojik çöküşünde Origin'in hayatta kalma içgüdüsünün büyük krize yol açmasıdır.
- **Mana ve Mana Çürümesi:** Mana dünyanın varoluş özü olarak ve geceleri yoğunlaşan Nebula formlarıyla tanımlanır. Origin kullanıcılarının %30'unda görülebileceği yazılıdır; aşırı güç kullanımının yenileme haznelerini bozması, yüz kıllarının tamamen beyazlaması ve sonuçta ölüm ya da güç kaybı anlatılır.
- **Perde / Outlander:** Perde Rhodes bölgesindedir. Outlander'lar uzaylı olarak değil, geçmişte Mana Çürümesine uğramış ve Perde'nin çarpık enerjisi sayesinde mutasyona uğrayarak hayatta kalmış 17 insan olarak tanımlanır. Kendi manaları yerine Perde'nin enerjisini kullanırlar. Lord of the Mists, insanlık adına ajanlık yapan tek Outlander olarak tarif edilir.
- **İkiz Tanrıçalar:** v1.2 yazımı “Euruyn ve Morygnn”dir. Ambrossa, Yalanlar Origini sahibi ve Perde'nin gelecekteki kilidini açacak anahtar olarak; Felix'in Deneb'e yalan söyleyip kendi Origin'ini yedeklemesi de ayrı bir gizli tarih olarak özetlenir.

### 11.2. Politik coğrafya, mafya ve Siyah Kan (DOCX s. 2–3)

- **F.O.R.A.:** T.O.W.E.R., Verdun, Peru, Tokyo ve Helenaport'un oluşturduğu beş-devlet paktıdır; Rhodes bağımsızdır.
- **T.O.W.E.R.:** Üç katlı Fildişi Kule; üstte elitler/Sakamoto Koleji, ortada sert rekabet ve Verdun'a bağlantı, altta sefalet ve kargo gemileri vardır.
- **Rhodes / Helenaport / Verdun:** Rhodes'ta Rigel/Altın Leydi, Dünya Ağacı ve mühürlü Lord Blackthorn; Helenaport'ta Lady Purplecarrot/Jailer ve tasma dini; Verdun'da gizli laboratuvarlar, gece hayatı ve Boy King belirtilir.
- **Mafya aileleri:** 70 yıllık anlaşma gereği her ailede yalnızca bir Anomali/Joker bulunması kuralı verilir. Hearts/Simo, Diamonds/Lewis, Spades/Minamoto, Clubs/Frenze ve Jokerleri listelenir.
- **Siyah Kan:** v1.2'de Frenze/Clubs laboratuvarlarında sentetik üretilen, Diamonds ağı üzerinden okula/sokaklara dağıtılan illegal Verdun iksiri olarak tanımlanır. Gücü kısa süreli zirveye taşır; sonra Mana Çürümesi krizi ve yıkım riskine sürükler.

### 11.3. Karakter geçmişi, kampanya kaydı ve kurum içi rapor (DOCX s. 3–6)

- Deneb/September ve Anastasia'nın yetimhane geçmişi; Horizon Day'in ölümü; Exis, Eli, Asa, Seth ve Sylas geçmişleri Bölüm 5'te kısa özetlerle anlatılır.
- Bölüm 7, Seans 0, Agatha'nın tasmalanması, sınıf başkanlığı/sınıf savaşları, Bowling Faciası, Kintoki'nin ölümü, karantina ve resmi örtbası kapsar.
- Gizli rapor, September'ın 1-S sınıfına dair kurum içi değerlendirmesidir; bu rapordaki yargılar diegetik/kurumsal bakış açısıdır ve otomatik olarak objektif gerçek kabul edilmemelidir.
- “5 Renkli Indigo” (DOCX s. 6–7), beş Origin fazı, göz/damar rengiyle güç değişiminin telegraph edilmesi, hızlı geçişte bedenin iflası ve oyuncuların boss'u aşırı kullanıma zorlayarak Origin Felaketi yaşatması mekaniklerini içerir.
- Kod: 0 / Code: Zero (DOCX s. 7–8), De Paul'un mana emme Origin'inden üretilmiş, hedefi öldürmek yerine manasını bayılana kadar emip geçici komaya sokan hançerdir.

### 11.4. E.Y.Ö., The Progenitors ve karakter fihristi (DOCX s. 8–17)

- E.Y.Ö. beş eşik olarak sıralanır: Taktiksel, Kentsel, Ulusal, Küresel, Varoluşsal. Tanımları ve örnekleri DOCX s. 8–10 ve yeniden s. 10'da bulunur.
- **The Progenitors (7 Hükümdar Origin):** Sakamoto/Demiurge, Simo/Animus, Dux/Aion, Frenze/Sanguis Sanctum, Minamoto/Eidolon, Sterling/Gravitas, Quinn/Logos. Bu listenin Day ailesini içermediği, Minamoto ve Quinn'i içerdiği kaydedildi.
- **Birleşik karakter arşivi:** Sakamoto 1-S ve 1-A; Sakamoto üst sınıfları; Twin Tides öğrencileri; eğitmenler; T9/F.O.R.A./düzen liderleri; mafya liderleri/Jokerleri; Outlander listesi. Ayrıntılı Origin işlevleri, bedeller, dış görünüşler ve hikâye kancaları için doğrudan DOCX Bölüm 14 referans alınmalıdır.
- v1.2, daha önceki sürümlerdeki bazı bilgileri bir araya topluyor; ancak tüm kayıtların oturum günlüğünde gerçekten oynandığı varsayılmamalı. Özellikle “Senaryo Kancası”, “Hikâye ve Dinamik”, “Durum: çizildi” gibi işaretler kendi anlamlarıyla korunmalı.

## 12. Tam Arşiv v1.2 ile konuşma arşivi arasındaki ilk fark tablosu

Bu, tam satır-satır denetim değil; v1.2'nin yüklenmesinden sonra kaynaklardaki önemli kavram ve uyuşmazlıkların ilk çapraz kontrolüdür. “v1.2 önceliklidir” kuralı uygulanır. v1.2 kendi içinde çelişiyorsa seçim yapılmaz.

| ID | Konu | Tam Arşiv v1.2 | 512 sayfalık sohbet arşivi | Şu anki kayıt yöntemi |
|---|---|---|---|---|
| X-001 | Kaynak önceliği | Ayrı belge olarak öncelikli başvuru kaynağıdır; sohbet arşivi içindeki kullanıcı talimatı açıkça bunu söyler (PDF fiziksel s. 320; Gemini konuşmasının iç sayfalamasında 23/209). | v1.2 ile çelişen bilgi için dosyanın doğru; dosyada olmayan sohbet verisinin tamamlayıcı olduğunu belirten talimat içerir. | Kaynak hiyerarşisi **kesin olarak kaydedildi**. |
| X-002 | Tanrıça adının yazımı | **Euruyn ve Morygnn** (DOCX s. 2). | Birçok eski/alternatif yazımda “Morriggan” vb. görünüyor. | Güncel referans adı Morygnn; eski yazımlar tarihsel varyant olarak korunur. |
| X-003 | Horizon Day'in ölümü | Bölüm 5 ve 14.6, Horizon'u Deneb'in öldürdüğünü yazar; Sylas'ın fişi March/Arcturus'u “Exis'in babasının gerçek katili” olarak tanımlar (DOCX s. 3, 16). | Kullanıcı doğrudan açıkladı: gerçek katil March/Arcturus'tur. Dünya, Anastasia ve Exis dahil, Deneb/September'ın öldürdüğüne inanır. Gerçeği yalnızca Deneb ile Arcturus bilir. | **Kullanıcı açıklamasıyla çözüldü (K-001).** “Deneb öldürdü” kamuoyuna yansıyan/örtbas edilmiş anlatıdır; “March gerçek katil” gizli gerçektir. v1.2'deki kısa fişler buna göre yorumlanır, ancak kaynak metni değiştirilmiş gibi gösterilmez. |
| X-004 | Kintoki’nin ölümü ve bedeni | Bölüm 7.4 Bowling Faciası’nda Kintoki’nin öldüğü yazılır; Bölüm 14.2 karakter fişinde “Yakında Ölecek” etiketi kalmıştır (DOCX s. 5 ve 12). | Kullanıcı kesinleştirdi: Kintoki, Outlander’ların geçtiği portaldaki sızıntı sırasında o akşam öldü. Bedeni teslim edilmedi; F.O.R.A. beden üzerinde araştırmayı sürdürdü ve ailesi boş tabut gömdü. | **Ölüm durumu çözüldü (K-002).** “Yakında Ölecek” eski/eskimiş roster etiketi olarak korunur, güncel gerçek diye kullanılmaz. Bedenin F.O.R.A. tarafından nihayetinde ne yapıldığı/şimdi nerede olduğu kullanıcı kararı bekleyen açık sorudur. |
| X-005 | T9 ve F.O.R.A. ilişkisi | v1.2, T9'un F.O.R.A.'nın bir alt birimi olduğunu söylemez. Bölüm 14.6 liderleri bir arada ve karma başlık altında listeler. | Kullanıcı açıkça T9, mafya ve F.O.R.A.'yı üç ayrı güç odağı olarak tanımlar (PDF fiziksel s. 40 civarı); birbirlerine Outlander tehdidini durdurma hedefiyle bağlı olduklarını söyler. | Çatışma yok. Üçlü güç odağı ayrı tutulmalı; 14.6 başlığındaki karışık liste T9'un dokuz kişilik kadrosu diye okunmamalı. |
| X-006 | The Progenitors / Sovereign Origins | Güncel başlık “The Progenitors (7 Hükümdar Origini)” ve yedi aile Sakamoto, Simo, Dux, Frenze, Minamoto, Sterling, Quinn'dir (DOCX s. 9–10). | Sohbetin eski aşamalarında “Sovereign Origins” gibi adlandırma taslakları var; ilerleyen kullanıcı mesajı “The Progenitors” adını beğeniyor (PDF s. 271 civarı). | Güncel terim The Progenitors. Eski isimler karar geçmişinde kalır, eş anlamlı kanon terimi olarak kullanılmaz. |
| X-007 | Siyah Kan tarifi/etkisi | Sentetik Verdun iksiri; Frenze/Clubs laboratuvarında üretilir, Diamonds ağı dağıtır; kısa süreli güç artışını Mana Çürümesi ve yıkım riski izler (DOCX s. 3). | Sohbetin bir kısmında Perde faunası cesetlerinden damıtma, Origin kullanıcısı kanıyla füzyon ve Consequence'ları iyileştirme/hızlandırma fikri var (PDF s. 63–66 civarı). | V1.2'nin üretim ve uzun vadeli riske ilişkin tanımı önceliklidir. Fauna/kan bileşeni sentezin ayrıntısı olarak uyumlu olabilir; iyileştirici kısa vadeli etki ayrı/koşullu ek mekanik olarak saklanır, otomatik biçimde v1.2'nin yerine geçmez. |
| X-008 | September/Deneb'in savaş gücü | Deneb'in Origin çalma/aktarma yeteneği ve Felix'in Zero O'clock gücünü kullanması v1.2'de var (DOCX s. 16–17). | İlk offscreen dövüş taslağında vektör manipülasyonu gibi yanlış bir güç yazılır; kullanıcı daha sonra açıkça reddeder ve kendi zaman çarkı içinde geri alma/yedeğe alma, saldırıyı durdurma/tekrarlama anlatımını verir (PDF s. 9–12 civarı). | Vektör manipülasyonlu taslak **eski/yanlış öneri** olarak işaretlenir; kullanıcı düzeltmesiyle uyumlu zaman gücü açıklaması tamamlayıcı mekanik olarak tutulur. |
| X-009 | Origin oranları | İnsanların %33'ünde Origin; %1 Anomali; kullanıcıların %30'unda Mana Çürümesi anlatılır (DOCX s. 1). | Sohbet arşivinde de aynı temel oranlar yer alır; ayrıca “herkes psikolojik duruma göre Anomali'ye evrilebilir” düşüncesi bulunur. | Oran ile potansiyel ayrımı korunur: %1 mevcut/ölçülen Anomali oranı olabilir, evrilme ise olasılık. Paydalar ve ölçüm zamanı ileride netleştirilebilir. |
| X-010 | GATE’in kanon statüsü | Kullanıcının kontrolüne göre Tam Arşiv v1.2 içinde “GATE” aramasında sonuç yok; mevcut dosyada GATE ayrı bir konsept olarak tanımlanmıyor. | 512 sayfalık konuşma arşivinin başındaki bir oyuncu günlüğünde tekil “GATE (brigade)” ifadesi görülüyor. | **Mevcut statü netleşti (K-003):** GATE kanonda ayrı bir konsept değil. Tekil günlük ifadesi ayrı kurum kurmaya yetmez. Kullanıcı bunu ileride geliştirilebilecek bir fikir olarak görüyor; şimdilik [GELECEK FİKRİ — KANON DEĞİL]. |
| X-011 | Ajan kategorileri | v1.2 bu sınıflandırmayı belirtmez. | Sohbet arşivinde kullanıcı “Prime / Fringe / Rogue” dizisini seçer; “Blackbox” önceki seçenek olarak kalır (PDF s. 171 civarı). | Sohbet v1.2'deki boşluğu tamamlar: Rogue seçilmiş addır; Blackbox eski taslak. Statü tasarım kararı/kullanıcı onayı olarak kaynaklanır. |
| X-012 | Fate Core ev kuralları | v1.2 ayrıntılı Fate Core +11 puan dağılımı ve Trouble/Flaw kurallarını içermez. | Sohbet arşivinde bu mekanikler ve oyun içi kullanım örnekleri ayrıntılı olarak geliştirilmiştir (PDF s. 42–46 civarı ve diğer iş/job sayfaları). | Kullanıcı kaynak hiyerarşisine göre bu bilgiler tamamlayıcı veridir; v1.2'ye eklenen mekanikler olarak değil, ayrı “04 — FRP/Kampanya Kuralları” dokümanında korunur. |
| X-013 | Sylas/Sylan yazımı | Birleşik kadroda güncel yazım **Sylas** (DOCX s. 11). | Erken oyuncu günlüğünde “Sylan” biçimi görülür; diğer kısımlarda Sylas kullanılır. | Ana kayıtta Sylas kullan; “Sylan” OCR/yazım veya eski ad varyantı olarak kaynak bağlantısıyla sakla, otomatik olarak başka karakter sayma. |
| X-014 | T9 kadro ve mevsim kodları | Bölüm 14.6, T9 ve devlet/lider karakterlerini aynı başlık altında toplar; tam dokuzlu T9 roster'ı ayrı ve eksiksiz görünmez (DOCX s. 16). | Sohbet arşivinde T9'un dokuzlu yapısı, ay/mevsim kodları ve bazı üye aliasları üzerine kararlar yer alır (PDF s. 151–160 civarı). | Dokuzlu kadro tamamlayıcı sohbet kaydıyla ayrı tabloya alınır; v1.2 Bölüm 14.6 doğrudan ve bütünüyle T9 üye listesi kabul edilmez. |
| X-015 | Outlander listesi | Bölüm 14.8'de seçili Outlander'lar listelenir; dosya 17 kişinin hepsini ayrı ayrı ayrıntılandırmıyor olabilir (DOCX s. 17). | Sohbet arşivinde “Kutsal 17”, tarihsel yalan ve farklı motivasyon teorileri tartışılır (PDF s. 62–66 civarı). | v1.2'nin “17 eşsiz insan” ifadesi temel alınır. Katalogda görünmeyen isimler yok sayılmaz; ayrı “adlandırılmamış/fişi eksik” kapsam açığı oluşturulur. |
| X-016 | Bölüm numaralaması ve E.Y.Ö. | Belge Bölüm 12'den Bölüm 14'e geçer; 13 görünmüyor. E.Y.Ö. tanımı hem 10. bölüm sonrası hem Bölüm 12'de tekrarlanır (DOCX s. 8–10). | Sohbet arşivi E.Y.Ö.'yü güç ölçeği olarak kullanır. | Yapısal durum kaydı; Bölüm 13'ün ne olduğu tahmin edilmez. E.Y.Ö. kopyaları sürüm karşılaştırması yapılana kadar korunur. |

## 13. Tam Arşiv v1.2 içindeki çözülmesi gereken noktalar

Bu noktalar sohbetle çatıştıkları için değil, öncelikli DOCX'in kendi içinde iki ifade taşıdığı veya kaydın güncellenmiş olabileceği için açık bırakıldı:

1. **Horizon Day'in ölümü:** Bölüm 5'te Deneb'in öldürdüğü; Bölüm 14.6'da March/Arcturus'un gerçek katil olduğu yazıyor. Bunlar “fiilî saldırıyı yapan” ve “arka plandaki gerçek fail” şeklinde uzlaştırılabilir; fakat kaynak tek başına kesin ayrımı tanımlamıyor.
2. **Kintoki Sentaro — bedenin akıbeti (ölüm çelişkisi çözüldü, kalan soru açık):** Kintoki’nin o akşam Outlander portalındaki sızıntıda öldüğü kesin. Bedeni geri verilmedi; F.O.R.A. araştırmasını sürdürdü ve ailesi boş tabut gömdü. F.O.R.A.’nın bedenle nihayetinde ne yaptığına henüz karar verilmedi. Karakter fişindeki “Yakında Ölecek” kaydı tarihsel/eski etiket olarak korunur.
3. **T9 / düzen liderleri başlığı:** Bölüm 14.6 tek başına dokuz kişilik resmi T9 listesi değil; devlet liderleri, ölü üyeler, T9 üyeleri ve başka önemli kişiler bir başlık altında toplanmış. Ayrı T9 roster'ı oluşturulmalı.
4. **Bölüm 13:** Numara atlanmış. İçeriği çıkarılmış, unutulmuş veya başka yerde olması mümkün; elimizdeki DOCX'te bulunmuyor.
5. **Outlander kadrosu:** Bölüm 14.8'de seçili önemli isimler var, ancak 17 kişinin tümü aynı ayrıntı düzeyinde listelenmiyor. Eksik isimler uydurulmayacak.
6. **Origin yüzdelerinin paydası:** %33 insan, %1 Anomali ve %30 Mana Çürümesi oranları farklı paydaları anlatıyor olabilir; v1.2 bunu matematiksel olarak netleştirmiyor. Rakamları değiştirmeden, açıklamayı açık soru olarak tut.

## 14. Sonraki çalışma için kaynaklı işlem planı

1. **00 — Ana İndeks ve Karar Kaydı:** Bu envanterin güncel sürümünü başlangıç indeksi yap; kaynak önceliği kuralını ilk maddeye koy.
2. **01 — Kozmoloji ve Origin Sistemleri:** v1.2 s. 1–2'yi ana referans; sohbet arşivindeki kullanıcı onaylı ek ayrıntıları alt kayıt olarak kullan.
3. **02 — Coğrafya, Devletler ve Kurumlar:** v1.2 s. 2–3'ü referans al; T9, F.O.R.A., mafya ve Brigade kayıtlarını kaynaklarına göre düzenle. GATE, kullanıcı yeniden gündeme getirip geliştirmedikçe ayrı kurum olarak şemaya eklenmeyecek.
4. **03 — Karakterler, Soylar ve Kronoloji:** v1.2 s. 3 ve s. 11–17'deki kadro fişlerini temel al; iç çelişkileri ayrı sütunda tut.
5. **04 — Kampanya ve FRP:** v1.2 s. 4–6'daki oturum kaydını, 512 sayfalık PDF'deki devam eden günlükler ve Fate Core ev kurallarıyla eşleştir; plan/taslak/oynandı ayrımını koru.
6. Sonraki ürünler “kaynağa bağlı madde listesi” olarak hazırlanmalı; nihai kanon ansiklopedisi ancak çelişkiler ve açık sorular etiketlendikten sonra birleştirilmeli.


## 14. Kullanıcı karar kaydı — K-001: Horizon Day'in öldürülmesi

**Durum:** Kullanıcı açıklamasıyla çözüldü; gizli gerçek ile kamuya kabul ettirilen anlatı birbirinden ayrıldı.

### Kesinleştirilen bilgiler

- **Gerçek katil:** March / Arcturus, Horizon Day'i fiilen öldüren kişidir.
- **Kamuya açık anlatı:** Dünya, Anastasia Day ve Exis Day dahil, Horizon'u Deneb / September'ın öldürdüğünü bilir veya buna inanır.
- **Sırrı bilenler:** Gerçeği yalnızca Deneb ve Arcturus bilir.
- **Ambrossa'nın amacı:** Deneb'de psikolojik yıkım yaratıp onu Anomali Felaketi ve Mana Çürümesi yönünde itmek ister; Horizon'un Deneb'in gözleri önünde ölmesi bu planın parçasıdır.
- **Önceden mevcut durum:** Deneb, T9 darbesinden önce De Paul ile yaptığı çatışmada zaten Mana Çürümesi'ne yakalanmıştır. Deneb bunun farkında değildir; Ambrossa da bunu bilmez.
- **Zaman Origin'i fikri:** Deneb'in taşıdığı Felix/Dux bağlantılı zaman gücü, zaman bükülse bile kayıpların sonuçlarını ortadan kaldıramama ve kimi anlarda yalan/illüzyon çatlaklarını algılama fikriyle ilişkilendiriliyor. Bu, kullanıcının anlattığı yaratıcı yönelim olarak kaydedilir; aşağıdaki mekanik ayrıntılar henüz ayrı ayrı doğrulanmamıştır.

### Arcturus'un motivasyonu — statü ayrımı

Kullanıcı, Arcturus'un Horizon'u neden öldürdüğüne dair daha önce kurulmuş mantığın tüm ayrıntılarını hatırlamadığını söyledi. Gemini'nin önerileri olası açıklamalar olarak aşağıda korunur; otomatik biçimde kesin kanon sayılmaz:

1. Ambrossa'nın, Horizon'un hayatta kalmasının T9 darbesini tehlikeye atacağına veya F.O.R.A.'ya ihanet/operasyon güvenliği riski oluşturacağına dair Arcturus'u ikna etmesi.
2. Arcturus'un, Deneb'in Horizon'u kendisi öldürmek zorunda kalmaması ya da Deneb'in kalbinin/ruhsal durumunun daha ağır zarar görmemesi için cinayeti kendi üstlenmesi.
3. Darbe gecesi sahte bilgi/telsiz anonslarıyla yaratılmış acil bir kriz içinde Arcturus'un operasyonun bekası için Horizon'u tehdit olarak görmesi.
4. Horizon'un ölümünün “ritüel bedel”, devrimin tetikleyicisi veya Ambrossa'nın gerçeklik manipülasyonunda özel bir kilit olay olması.

Bu seçenekler birbiriyle çelişebilir ve henüz tek bir kesin nedensellik zinciri seçilmedi. Özellikle “Ambrossa'nın yalanı yalnızca kurban inanırsa gerçeğe dönüşür”, “zaman Origin'i yalanlara mutlak bağışıklık verir” ve “Deneb'in önceden Mana Çürümesi'ne yakalanmış olması Ambrossa'nın gücünü doğrudan etkisizleştirir” önermeleri, Gemini'nin mekanik açıklamaları olarak ayrıca onay gerektirir.

### Anlatı sırası için korunacak taslak

1. Deneb, De Paul ile çatışmada, henüz kendisinin de anlamadığı biçimde Mana Çürümesi'ne yakalanır.
2. Ambrossa bunu bilmeden, Horizon'un Deneb'in gözleri önünde ölmesini sağlayarak Deneb'i yıkmayı amaçlar.
3. Ambrossa, Arcturus'u Horizon'u öldürmenin T9'un operasyonu/darbesi için gerekli olduğuna inandırır; **Arcturus'un tam olarak hangi yalanı neden kabul ettiği henüz açık karardır.**
4. March/Arcturus Horizon'u öldürür.
5. Kamuoyu ve Day ailesi Deneb'i katil sanır; yalnızca Deneb ile Arcturus gerçeği bilir.
6. Daha sonraki karşılaşmada Ambrossa, Deneb'in Mana Çürümesi'ni kendisinin tetiklediğini ima ederek Deneb'i alaya alabilir. Deneb'in Felix'in zaman Origin'i sayesinde neyi fark ettiği, neyi sakladığı ve finalde Ambrossa'yı öldürme kararını nasıl verdiği mekanik ve dramatik olarak ileride kesinleştirilecek.

### Kaynak bağlantıları

- Öncelikli dosya `Abyss Evreni: Tam Arşiv v1.2.docx`, s. 3 ve s. 16: Horizon'un kamuya yansıyan ölümü / March'ın gerçek katil olarak yazıldığı karakter özeti.
- Konuşma arşivi `Abyss_OCR.pdf`, fiziksel s. 320: v1.2'nin öncelikli kaynak olmasına dair kullanıcı talimatı.
- Bu konuşmadaki kullanıcı açıklaması: gerçek katil, örtbas anlatısı, yalnızca Deneb ve Arcturus'un gerçeği bilmesi, Ambrossa'nın hedefi ve Deneb'in önceden Mana Çürümesi'ne yakalanmış olması.

---


## 15. Kullanıcı karar kaydı — K-002: Kintoki Sentaro’nun ölümü ve bedeninin akıbeti

**Durum:** Ölüm ve cenaze bilgileri kesinleştirildi; F.O.R.A.’nın beden üzerindeki nihai işlemi açık karar.

### Kullanıcı tarafından kesinleştirilenler

- Kintoki Sentaro, o akşam **Outlander’ların geçtiği portaldaki sızıntı sırasında öldü**.
- Kintoki’nin bedeni ailesine teslim edilmedi.
- **F.O.R.A., Kintoki’nin bedeni üzerinde araştırma yapmayı sürdürdü.**
- Ailesi, beden olmadığı için **boş tabut gömdü**.
- Tam Arşiv v1.2 Bölüm 14.2’deki “Yakında Ölecek” etiketi güncel olay bilgisiyle uyuşmayan eski bir fiş kaydıdır; bu ifade tarihsel kaynak izi olarak tutulur, Kintoki’nin hâlâ yaşadığı anlamında okunmaz.

### Açık bırakılan konu

- F.O.R.A. nihayetinde Kintoki’nin bedeniyle ne yaptı, bedeni nerede veya hangi koşullarda tutuluyor ve araştırmanın sonucu ne oldu? Kullanıcı bu kararı henüz vermedi. Bu boşluk öneriyle doldurulmayacak.

### Kaynak bağlantısı

- Öncelikli kaynak `Abyss Evreni: Tam Arşiv v1.2.docx`, Bölüm 7.4 (Bowling Faciası) ve Bölüm 14.2 (karakter fişi); kullanıcı açıklamasıyla ölümün ve boş tabutun ayrıntıları netleştirildi.


## 16. Kullanıcı karar kaydı — K-003: GATE ifadesinin kanon statüsü

**Durum:** Mevcut kanonda ayrı bir konsept değil; gelecekte değerlendirilebilecek fikir.

### Kullanıcı tarafından kesinleştirilenler

- Kullanıcı Tam Arşiv v1.2 içinde “Brigade” kayıtlarını kontrol etti ve “GATE” aramasında sonuç bulmadı.
- **GATE diye ayrı bir konsept mevcut kanonda yoktur.**
- Kullanıcı bu fikrin gelecek için değerlendirilebileceğini söyledi; bu, şimdilik kanon değil, olası bir gelecek fikridir.

### Kaynak ayrımı

- Öncelikli kaynak `Abyss Evreni: Tam Arşiv v1.2.docx` içinde GATE için tanımlanmış bir konsept bulunmuyor.
- 512 sayfalık konuşma arşivinin başındaki bir oyuncu günlüğünde yalnızca bir kez “GATE (brigade)” ifadesi geçiyor. Bu ifade ham kaynak metninde korunur; ancak tek başına bağımsız bir kurum, kod adı veya Brigade ile resmî ilişki kurmaz.

### İşleme kuralı

GATE; gelecekte kullanıcı tarafından geliştirilip onaylanmadıkça kurum şemasına, kanon sözlüğüne veya olayların nesnel açıklamasına eklenmeyecek. Brigade ile ilişkisi hakkında varsayım yapılmayacak.
