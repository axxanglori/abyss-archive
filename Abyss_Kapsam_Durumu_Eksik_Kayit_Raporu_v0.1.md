# ABYSS — Kaynak Kapsamı ve Eksik Kayıt Durumu v0.1

**Denetlenen ana indeks:** `Abyss_Kaynak_Konum_Eslestirme_v0.8.csv` (318 satır)  
**Kaynak konum düzeltmesi içeren yeni sürüm:** `Abyss_Kaynak_Konum_Eslestirme_v0.9.csv` (318 satır; kayıt sayısı değiştirilmedi)  
**Aday defteri:** `Abyss_Kayip_Kayit_Adaylari_v0.3.csv` (30 aday)  
**Bekleyen Origin/güç listesi:** `Abyss_Origin_Guc_Denetimi_Bekleyen_99_v0.1.csv`

## 1. Denetim sonucu

Envanterin ilk yapısal ve kapsamsal kontrolü tamamlandı. Bu raporun en önemli sonucu, mevcut 318 satırlık envanterin tamamlanmış bir kanon ansiklopedisi olmadığı; belirli kategorilerde kayıtların kaynak kanıtı işlenmişken, Origin ve özel güç fişlerinin önemli bir bölümünde satır düzeyinde kaynak pasajı doğrulamasının hâlâ beklediğidir.

- Ana indekste **318 kayıt** var; aynı görünür kayıt adının noktalama/büyük-küçük harf normalizasyonu sonrası birebir tekrarı bulunmadı. Bu, alias’ların veya kavramsal kayıtların çakışmadığı anlamına gelmez.
- Kategoriler: karakter **109**, Origin/güç sistemi **110**, FRP/oyun mekaniği **29**, olay/kronoloji **28**, kurum/örgüt **22**, coğrafya/yer **17**, nesne/teknoloji **3**.
- **219/318** satırda hem DOCX hem PDF kısa kanıt alanı dolu. **99/318** satırda bu iki kanıt alanı da boş; bekleyen 99 kaydın tamamı Origin/güç sistemi kategorisinde.
- Öncelikli DOCX, fiziksel sayfa numaralarıyla 17 sayfadır. Konuşma arşivi PDF’si 512 fiziksel sayfadır.

Bu rakamlar kaynak alanlarının işlenme kapsamını gösterir; “yüzde 68,9 kanon doğruluğu” veya “evrenin yüzde 68,9’u tamamlandı” diye yorumlanmamalıdır.

## 2. Kaynak dosyalarının metin kapsamı

### 512 sayfalık konuşma arşivi

Mevcut metin çıkarım dosyasında fiziksel sayfa **1’den 512’ye kadar 512 ayrı sayfa bölümü** bulundu; bu bölümlerin hiçbiri boş değil. Çıkarılmış metindeki her fiziksel sayfada en az 86 kelime-benzeri token bulunuyor. Bu, arama yapılabilecek bir metin bölümünün mevcut olduğunu gösterir; OCR’ın her özel adı doğru okuduğunu veya her görsel ayrıntının korunduğunu kanıtlamaz.

Senin açıklamana uygun olarak `merged2pdf.pdf` ile `Abyss_OCR.pdf` aynı içerik kabul edildi; OCR karşılaştırması yeniden yapılmadı. PDF’nin 512 sayfasının tamamı görsel olarak tek tek kontrol edilmedi. Önceki turlarda sayfa örnekleri render edilip incelendi; kaynak görüntüsü üzerinden yüzde 100 görsel doğrulama bu çalışmanın kapsamında değildir.

### Tam Arşiv v1.2

`Abyss Evreni_ Tam Arşiv v1.2.docx` birincil kaynaktır. 17 sayfalık metin ve sayfa yerleşimi çıkarımı mevcut. Belgenin bölüm numaraları 12’den 14’e geçiyor; **13. bölüm görünmüyor**. Bu durum yapısal bulgu olarak korunur; bölümün içeriği tahmin edilmez. E.Y.Ö. açıklamasının tekrarı da sürüm geçmişi bilinmeden silinmemelidir.

## 3. Kategori bazında kaynak kanıtı durumu

| Kategori | Kayıt | Kanıt alanları dolu (DOCX + PDF) | Ayrıntılı doğrulama bekliyor | Denetim özeti |
|---|---:|---:|---:|---|
| Karakter | 109 | 109 | 0 | 98 ayrıntılı karakter denetimi, 2 mevcut alias/persona güncellemesi, 9 yeni tamamlayıcı kaynak karakter kaydı. Kaynakta görülmek, her karakterin tüm olaylarının oynandığını kanıtlamaz. |
| Origin / güç sistemi | 110 | 11 | 99 | 10 temel Origin/Mana kaydı ayrıntılı kontrol edildi; Yün gücü için bir sınırlı not eklendi. Kalan 99 özel güç/Origin kaydı satır düzeyinde pasaj denetimi bekliyor. |
| Kurum / örgüt | 22 | 22 | 0 | 21 kayıt kurum/coğrafya aşamasında denetlendi; Gridlock ekip düzeyinde sınırlı bir kayıt olarak eklendi. |
| Coğrafya / yer | 17 | 17 | 0 | 16 yer kaydı denetlendi; Vault-7 tesis kaydı ters taramada eklendi. |
| Olay / kronoloji | 28 | 28 | 0 | 27 kayıt denetlendi; Wooly’ye suikast girişimi yalnızca senaryo öncülü olarak eklendi. |
| FRP / oyun mekaniği | 29 | 29 | 0 | Kaynak pasajı ve statü kontrolü yapıldı; bütün mekaniklerin kullanıcı tarafından nihai onay aldığı sonucu çıkarılmadı. |
| Nesne / teknoloji | 3 | 3 | 0 | Üç kayıt ters taramada açıldı; teknik limitler ve kanonik statü için GM sahnesi ile kullanıcı kaynağı ayrımı korunmalı. |
| **Toplam** | **318** | **219** | **99** | **Eksik ayrıntılı denetim tamamen Origin/güç sistemi kayıtlarında yoğunlaşıyor.** |

“Kanıt alanı dolu” ifadesi, o satırın her tarihsel tekrarının veya sayfa görüntüsünün denetlenmiş olduğunu değil, kaynak pasajı ve konum alanının işlenmiş olduğunu ifade eder.

## 4. Fiziksel sayfa eşleştirmesinde bulunan açık

v0.8’in `Konuşma arşivi PDF metin eşleşme sayfaları (fiziksel)` sütunundaki sayısal aralıkların birleşimi **511/512** fiziksel sayfayı kapsıyordu. Eksik sayfa **427** idi.

PDF s. 427’de şu içerikler yer alıyor:

- Resphu ve Atum Abargil çevresindeki sahnenin devamı;
- “When the Silent Song, silenced even further” başlığı;
- Thea’nın “Chile” soyadını taşıdığı ve yeni anne olduğu bilgisi;
- Lukas’ın beşikteki bebek olarak tanıtılması.

v0.9’da Thea Chile kaydına s. 427–428 **bağlamsal kaynak konumu** olarak eklendi. Bu sayfalarda bitişik “Thea Chile” dizesi yok; Thea adı ve Chile soyadı aynı sahne bağlamında yer alıyor. Bu nedenle kayıt, literal tam-ad eşleşmesi değil, bağlamsal sayfa eşleştirmesi olarak işaretlendi. Bu düzeltmeyle sayısal sayfa eşleştirme aralığı 512/512’ye ulaşıyor; bu yalnızca her sayfanın en az bir kayıt konumuyla ilişkilendirildiği anlamına gelir, sayfadaki her unsurun envantere alındığı anlamına gelmez.

Bu kontrol sırasında ayrıca:

- **Rhodes Kilisesi:** PDF s. 207’de “Rhodes kilisesinin sahibi” ifadesi bulundu; v0.9’da konum düzeltildi. Bu ifade tek başına Rhodes’taki Demir Şapel ile Helenaport’taki din merkezi arasında kurumsal bağ kurmaz.
- **Seans 0:** PDF s. 209’da “session 0” biçiminde İngilizce varyant ve oyuncu günlükleri bağlamı var; v0.9’da bu kaynak izi eklendi. Asistan değerlendirmesi, oyuncu günlüklerinin kendisiyle karıştırılmamalı.
- **Ouroboros:** v1.2 DOCX Bölüm 14.4’te kayıtlı, fakat PDF metninde literal ad eşleşmesi bulunamadı. Birincil kaynak var; eksik olan tamamlayıcı PDF konumudur.
- **Koç Yamino Kuni:** v1.2’de “Koç Yamino ‘Furiko’ Kuni / Kael Vesper” şeklinde birleşik başlık var; PDF s. 224’te “Koç Kael Vesper” geçiyor ama “Yamino Kuni” literal eşleşmesi bulunamadı. Alias veya derleme hatası kararı verilmedi.

## 5. Yeni eksik-kayıt adayları: fiziksel PDF s. 427

Aday defteri v0.3, eski 27 adayı koruyup bu kapsam denetiminden üç kayıt ekliyor. Bunlar ana indekse otomatik olarak eklenmedi:

1. **Resphu:** Konuşma arşivinde 34 ayrı fiziksel sayfada geçiyor; v0.8 ana indeksinde karakter/alias olarak yok. Karakter kaydı olma ihtimali yüksek; kimlik, Origin ve sahne statüsü ayrıca doğrulanmalı.
2. **Lukas:** PDF s. 427–428’de adı verilen küçük yaştaki sahne karakteri; Thea yeni anne olarak tanıtılıyor. Ana indekste ayrı kayıt yok. Kaynağın anlatı sahnesi olması, bu olayın FRP’de oynandığını kanıtlamıyor.
3. **“When the Silent Song, silenced even further”:** PDF s. 427’de sahne/bölüm başlığı. Olay kaydı değil, anlatı segmenti başlığı olarak beklemede tutuluyor.

Thea Chile zaten ana indekste var; yeni kayıt açılmadı, yalnızca kaynak konumu genişletildi. Rina adı da aynı sahnede geçiyor, ancak burada yalnızca “Rina” yazdığı için bunu otomatik olarak `Rina Torres` ile birleştirmedim.

Önceki aday defteri v0.2’deki 27 maddeden 16’sı yeni ana kayıt olarak işlendi, 2 alias/persona güncellemesi yapıldı ve 9 aday beklemede kaldı. v0.3’te bu üç yeni aday eklendi; yeni satırlar kullanıcı onayı veya kaynak türü değerlendirmesi olmadan kanon kabul edilmiyor.

## 6. Öncelik sırası

### P1 — 99 Origin/güç kaydını ayrıntılı denetle

`Abyss_Origin_Guc_Denetimi_Bekleyen_99_v0.1.csv` bu listenin tamamını içeriyor. İlk önce temel/ortak mekaniklerden başlanmalı: Origin aktarımı/manipülasyonu, Zero O’clock/zaman çarkı, Perde enerjisi, The Progenitors ve Creation; ardından v1.2 Bölüm 14.1–14.8’deki yetenek fişleri bölüm bölüm incelenmeli.

Her güç için şu alanlar doğrulanmalı: doğru ad ve alias, sahibi/karakteri, Origin sınıfı, kanıtlı işlev, açık sınırlar/bedel, DOCX’teki ana sayfa, PDF’deki fiziksel sayfa/konuşmacı ve kaynak çelişkisi. Bir sahnede görülen etkinin genel evren kuralı olduğu varsayılmamalı.

### P2 — Açık kimlik ve taslak adaylarını ayır

Koç Yamino Kuni/Kael Vesper, Poloz Will/Kael, General Accel/De Paul, Lucien Asa Bellone/Asa, Luda Oksana, Selene, Sage Baez ve Gridlock bireysel üyeleri gibi açık adaylar yalnızca kaynak desteklediği ölçüde tutulmalı. Asistan kaynaklı isim ve mekanikler, kullanıcı onayı olmadan ana kanona alınmamalı.

### P3 — Görsel doğrulama ve son indeks standardı

Tüm 512 sayfayı görsel olarak tek tek kontrol etmek ayrı ve daha geniş bir iş kalemidir. İlk hedef, metin çıkarımında şüpheli özel adlar, sayfa/konuşmacı sınırları ve tablo/karakter fişlerini örnekleyerek düzeltmek; kritik sayfalarda görüntüyle doğrulamadır. Bu yapılmadan “OCR yüzde 100 doğru” veya “envanter tamamen eksiksiz” denmemeli.

## 7. Kaynak ve sürüm bütünlüğü

- Birincil referans `Abyss Evreni_ Tam Arşiv v1.2.docx` olarak kalır.
- `merged2pdf.pdf` ile `Abyss_OCR.pdf` kullanıcı açıklaması uyarınca aynı içerik kabul edilir.
- Kaynakta bulunan her ayrıntı otomatik kanon değildir: kullanıcı kararı, oynanmış oturum, oyuncu günlüğü, anlatı sahnesi, kurgu içi haber ve asistan taslağı ayrı statülerde tutulur.
- v0.8 değiştirilmedi; p.427 ve diğer kaynak konum düzeltmeleri v0.9’a yazıldı.
- Hiçbir belirsiz kimlik veya asistan önerisi sessizce kesinleştirilmedi.

**Sonuç:** İndeks kullanılabilir düzeyde yapılandırılmıştır ancak henüz tam kaynak doğrulaması değildir. En somut kalan teknik iş, 99 Origin/güç kaydının gerçek kaynak pasajlarına tek tek bağlanmasıdır. Bunun ardından envanterde bulunmayan isimler ve alt kayıtlar ikinci tur ters taramada kontrol edilmelidir.
