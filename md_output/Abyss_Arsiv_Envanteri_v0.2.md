# ABYSS — Arşiv Envanteri v0.2

**Durum:** OCR karşılaştırması tamamlandı; ayrıntılı kanon denetimi öncesi  
**Kaynak dosyaları:** `merged2pdf.pdf` (özgün, 512 sayfa, 88,6 MiB) ve `Abyss_OCR.pdf` (OCR sürümü, 512 sayfa, 228,3 MiB)  
**Amaç:** Arşivde nelerin bulunduğunu belirlemek, kaynak türlerini ayırmak ve sonraki kanon belgelerine güvenilir bir yol haritası sağlamak.

> **Önemli uyarı:** Bu dosya bir kanon özeti değildir. Burada geçen hiçbir madde yalnızca bu envantere girdiği için kesinleşmiş kanon sayılmaz. Kullanıcı notları, Gemini önerileri, oyuncu günlükleri ve sahne taslakları farklı türde kaynaklardır. Aralarındaki ayrımlar sonraki aşamada tek tek kaydedilecektir.

## 1. Teknik durum ve kapsama

- Özgün PDF `merged2pdf.pdf`: 512 sayfa, 92.942.222 bayt (yaklaşık 88,6 MiB), şifresiz.
- Kullanıcının OCR sürümü `Abyss_OCR.pdf`: 512 sayfa, 239.300.940 bayt (yaklaşık 228,3 MiB), şifresiz ve ilk 204 sayfada artık aranabilir metin katmanına sahip.
- Sayfa sayısı ve sırası korunmuş görünüyor. Fiziksel sayfa 1–204'te OCR metni eklenmiş; özgün PDF'de bu sayfalar için normal metin çıkarımı boştu.
- Özgün PDF'den çıkarılabilen metin toplam 233.073 kelimeydi (esas olarak fiziksel s. 205–512). OCR PDF'den 328.231 kelime çıkarılıyor. Fark olan **95.158 kelime**, OCR PDF'nin ilk 204 sayfasından alınan metne karşılık geliyor.
- Fiziksel s. 205–512 için iki PDF'den alınan metin, boşluklar normalize edildikten sonra birebir eşleşti: 1.726.620 karakter ve 233.073 kelime. Bu, OCR sürümünün önceki metin katmanını değiştirmediğini gösteren güçlü bir metin karşılaştırmasıdır.
- İlk 204 sayfa için önceki ayrı OCR çıktım (`Abyss_1-204_OCR.txt`) 96.470 kelime içeriyordu. Kullanıcının PDF'sinden alınan metinle sayfa bazında ortalama normalize benzerlik yaklaşık %90,1; kelime sayıları aynı ölçek aralığında. Bu oran doğruluk puanı değildir, yalnızca iki OCR metninin örtüşmesini ölçer. Örnek kontrollerde kullanıcının PDF'si Türkçe karakterleri ve noktalama işaretlerini daha okunaklı koruyor; yine de özel adlar ve kurgu terimleri manuel doğrulama gerektirebilir.
- Tam metin çıkarımı, her fiziksel PDF sayfasını ayıran bir dosya olarak da saklandı: `Abyss_OCR_TumMetin.txt`.

**Sonuç:** İlk 204 sayfa artık aranabilir ve envantere alınabilir. Bu, her OCR kelimesinin hatasız olduğu anlamına gelmez; özellikle özel adlar, kurgusal terimler, İngilizce/Türkçe geçişleri ve diyalog içindeki hitaplar gerektiğinde özgün sayfa görüntüsüyle kontrol edilmeli.

## 2. Belgenin kaynak katmanları

### A. Fiziksel sayfalar 1–204 — Kampanya günlüğü, sezon değerlendirmeleri ve GM hazırlıkları

Kullanıcının OCR PDF'si sayesinde bu bölümün tamamında aranabilir metin mevcut. Aşağıdaki harita sayfa gruplarındaki ana konuları gösterir; bir aralıkta farklı sahneler veya öneriler iç içe geçebilir.

| Fiziksel PDF sayfaları | İçerik haritası | Statü açısından dikkat |
|---|---|---|
| 1–8 | Birinci yıl/sezon değerlendirmesi; ikinci yıl için öneriler; Eli'nin günlük devamı; Sylan/Sylas'ın 25.09.2041–08.10.2041 günlüğü. Lapis-7, GATE/Brigade sorgusu, Anastasia ile karşılaşma, March'la yeraltı işi, PvP ve parti içi güven kaybı. | Günlükler oyuncu perspektifidir; Gemini değerlendirmeleri ayrı yorum katmanıdır. “Sezon 2 / birinci yıl” gibi etiketler kronolojiyle çapraz kontrol edilmeli. |
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

Fiziksel s. 22–26 arasında kullanıcı, “Abyss Evreni: Tam Arşiv v1.2” belgesini ana kaynak olarak kullanma ve yeni bilgileri bu belgeyle karşılaştırma talimatını kayda geçiriyor. Bu dosyanın kendisi 512 sayfalık PDF'nin içinde görünmüyor; dolayısıyla arşivde bu belgeye bağlı bir kaynak önceliği beyanı var, ancak ana belgeyi karşılaştırmalı denetlemek için dosyanın ayrıca sağlanması gerekir. Bu eksiklik, mevcut PDF'yi işe yaramaz yapmaz; yalnızca geçmişte verilmiş “ana kaynak” kuralını doğrulamak için gerekli bir referansın eksik olduğu anlamına gelir.

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
- **GATE / Brigade:** Askerî/güvenlik müdahaleleri ve Outlander/kriz olaylarına müdahale ile ilgili kayıtlar var; aralarındaki kurumsal ilişki tutarlı tek tanıma bağlanmalı.

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
| C-011 | GATE ve Brigade | Bazı kampanya kayıtlarında adlar güvenlik/müdahale gücü olarak birbirine yakın kullanılıyor. | Kurumsal ayrım ve bağlılık zincirini kaynaktan çıkar. |
| C-012 | Oynanmış olay ile öneri | Gemini yanıtları gerçekleşmiş olayları yorumluyor ve hemen ardından gelecek olaylar öneriyor. | Her olay kaydına [OYNANDI], [PLAN], [ÖNERİ] statüsü ekle. |
| C-013 | September'ın güç tanımı | İlk Kuro sahnesi vektör manipülasyonu yazar; kullanıcı bunu açıkça reddedip zaman çarkı/backup ve saldırıyı durdurma-tekrarlama mekaniklerini açıklıyor. | Kullanıcı düzeltmesini esas al; yalnızca hangi sınırların kesin olduğu belirsizse soru listesine taşı. |
| C-014 | T9–F.O.R.A. hiyerarşisi | Bazı sahne önerileri T9'u devlet/askeri yapı ile iç içe anlatabilir; kullanıcı T9'un F.O.R.A.'nın altında olmadığını özellikle belirtiyor. | Ayrı güç odağı ve bağlantı/ittifak ilişkilerini ayır. |
| C-015 | Kampanyanın hangi sınıfta/yılda olduğu | Erken sayfalar sezon 1/2 ve birinci yıl dilini kullanırken s. 188 kullanıcı 2. sınıfın ikinci döneminde olduklarını söylüyor. | Her kayıt için kaynak tarihi ve masa içi zaman noktası ekle; geç dönem kullanıcı düzeltmesini zaman çizelgesine yerleştir. |
| C-016 | T9'un dokuzlu ve mevsim kodları | Kullanıcı 12 kişilik öneriyi reddediyor; dokuzlu ve mevsim temasını tutuyor. Her ay/mevsim kodunun hangi üyeye bağlandığı tüm kayıtlarla karşılaştırılmalı. | T9 roster'ında sayı, alias, mevsim/birim, görev ve kaynak sütunları aç. |
| C-017 | Üçüncü ajan kategorisi | “Blackbox” önceki seçenek, “Rogue” ise kullanıcının tercih ettiği ad. | Güncel dokümanlarda Rogue kullan; Blackbox'ı eski adlandırma olarak işaretle. |
| C-018 | Indigo Çocuk Projesi'nin tanımı | Kullanıcı s. 184'te amaç kopyalama ve Origin çaprazlamasıdır diye düzeltiyor. | Proje tanımında bu formülasyonu kaynak notuyla kullan; ayrıntıları sonraki kaynaklarla eşleştir. |
| C-019 | “Abyss Evreni: Tam Arşiv v1.2” ana kaynağı | Bu PDF, başka bir dosyanın öncelikli kaynak olması gerektiğini kaydediyor ancak söz konusu dosya bu paket içinde değil. | Dosya sağlanırsa mevcut arşivle fark karşılaştırması yapılmalı; yoksa bu envanter geçici kaynak envanteri kalmalı. |
| C-020 | Sylas/Sylan yazımları | İlk günlüklerde “Sylan”, diğer bölümlerde “Sylas” geçiyor. Bu, OCR veya eski karakter adı olabilir. | Oyuncu/karakterin tercih edilen yazımını bir kez onayla; kaynak yazımını tarihsel kayıtta sakla. |
| C-021 | Kuro/September sahnesinin statüsü | Kuro'nun akademiye sızması ve Deneb ile dövüşü ayrıntılı biçimde yazılmış ama sahne offscreen taslağıdır. | GM notu olarak tut; oynandı kaydı gelmedikçe [PLAN]/[SAHNE TASLAĞI] statüsünde bırak. |

## 7. Önerilen ana bilgi tabanı

Sonraki aşamada bu envanterden şu ana belgeler türetilebilir:

1. **00 — Abyss Ana İndeks ve Karar Kaydı:** kaynak önceliği, kanon statüleri, açık sorular ve değişiklik günlüğü.
2. **01 — Kozmoloji ve Origin Sistemleri:** mana, Origin sınıfları, Anomali, Mana Çürümesi, Origin Felaketi, aktarım kuralları.
3. **02 — Coğrafya, Devletler ve Kurumlar:** kıtalar, ülkeler, F.O.R.A., T.O.W.E.R., Rhodes, Verdun, T9, GATE/Brigade.
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
6. Kullanıcının atıf yaptığı “Abyss Evreni: Tam Arşiv v1.2” ayrıca sağlanırsa onu da karşılaştırma kaynaklarına ekle.

## 10. OCR karşılaştırması — v0.2

| Ölçüt | Özgün PDF | Kullanıcının OCR PDF'si | Sonuç |
|---|---:|---:|---|
| Sayfa sayısı | 512 | 512 | Eşit |
| Dosya boyutu | 88,6 MiB | 228,3 MiB | OCR sürümü yaklaşık 2,58 kat büyük |
| Metin çıkarımı | 233.073 kelime | 328.231 kelime | Aradaki 95.158 kelime ilk 204 sayfanın metninden geliyor |
| Fiziksel s. 205–512 | 233.073 kelime | 233.073 kelime | Boşluklar normalize edilince tüm çıkarılmış metin birebir eşleşiyor |
| Fiziksel s. 1–204 | Aranabilir metin yok | 95.158 kelime | Kullanıcının OCR'si eksik metin erişimini gideriyor |

Önceki OCR metniyle yapılan karşılaştırma yaklaşık %90,1 ortalama normalize sayfa benzerliği gösterdi; bu, birbirinden farklı iki OCR çıktısının ne ölçüde örtüştüğünü gösterir ve bağımsız OCR doğruluk ölçümü değildir. Yeni OCR PDF'si, örnek kontrollerde daha okunaklı Türkçe karakterlerle tam metin araması için tercih edilmelidir. Ham OCR metni, OCR hatalarının izlenebilmesi ve gerektiğinde kaynak sayfaya dönülebilmesi için korunmalı.
