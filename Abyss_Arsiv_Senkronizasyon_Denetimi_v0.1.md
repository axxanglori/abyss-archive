# Abyss — Dosyalar Arası Senkronizasyon Denetimi v0.1

**Amaç:** Kullanıcı karar kaydı, kaynak konum eşleştirme indeksi, 99 kayıtlık Origin/güç denetimi ve kapsam matrisi arasındaki temel sayı/statü uyumunu denetlemek. Bu rapor yeni kanon üretmez.

## Denetlenen yerel dosyalar

- `Abyss_Karar_Kaydi_v1.4.md` — K-001–K-013 kararları mevcut; v1.3 tarihsel sürüm olarak korunur.
- `Abyss_Kaynak_Konum_Eslestirme_v2.8.csv` / `.md` — 319 kayıt.
- `Abyss_Origin_Guc_Denetimi_99_Kayit_Takip_v1.9.csv` — 99 veri satırı.
- `Abyss_Origin_Guc_Denetimi_Acik_Konular_v1.0.csv` — 23 takip satırı; C-22, C-17 ile birleştirilmiş pasif geçmiş kaydı.
- `Abyss_Kaynak_Kapsam_Matrisi_v0.4.csv` — kapsam sayımı 319 ile eşitlendi; v0.3 geçmiş sürüm olarak korundu.

## Doğrulama sonuçları

| Kontrol | Sonuç | Not |
|---|---|---|
| Karar kaydı | Uyumlu | K-001–K-013 mevcut; kullanıcı kararları eski kaynakları silmeden işleniyor. v1.4 ile v1.3’teki başlık/dosya adı sürüm farkı düzeltildi; içerik kararları değişmedi. |
| Ana kaynak indeksi | Uyumlu | 319 satır; her satırda DOCX konum, kısa DOCX kanıtı, kısa PDF kanıtı, durum notu ve açık işlem alanı dolu. |
| 99 kayıtlık denetim listesi | Uyumlu | Tam 99 satır; kanıt alanlarının dolu olması tüm sayfaların görsel denetlendiği anlamına gelmez. |
| Eski kapsam matrisi kategori toplamı | Düzeltildi | v0.3 toplamda bir tarihsel taslak kaydını göstermiyordu; kategoriler 318’e ulaşıyordu. v0.4’e 1 adet “Tarihsel taslak / Origin denemesi” eklendi ve toplam 319 oldu. |
| Horizon Day / Kintoki | Yeni raporlarda statü ayrımı | K-001 gerçek fail ile kamu anlatısını ayırır; K-002 ölüm ile bedenin nihai akıbetini ayırır. Kaynak eski ifadeleri tarihsel izdir. |
| Kael / koç | Kimlik ayrımı çözüldü | K-006 iki karakteri ayırır; adların son biçimleri açık. Literal PDF eşleşme eksiği, kişilerin aynı olduğu anlamına gelmez. |
| Caspian “Siren” Locke | Uyumlu | K-004 güncel sınıfı Katalizör olarak belirler; DOCX’teki İnhibitör etiketi tarihsel kaynak izi olarak kalır. |
| Exis Day | Uyumlu | K-005: Enerji Manipülasyonu ana kategori; Chrono-Energy/zaman enerjisi alt enerji türü. Exis’in geleceği açık. |
| The Progenitors / Day | Uyumlu | K-012/K-013: yedi aile; Day, Animus uzantısı, sekizinci aile değil. Aile adları ve ata Origin adları ayrı katmanlardır. |

## Güncellenen çıktılar

1. `Abyss_Kaynak_Kapsam_Matrisi_v0.4.csv` — kategori sayımı 319 ile eşitlendi; literal eşleşme notu K-006/K-008’e göre güncellendi.
2. `Abyss_Origin_Guc_Denetimi_Genel_Kapsam_Celiski_Raporu_v0.6.md` — ana indeks sürümü ve kayıt sayısı v2.8 / 319 olarak güncellendi; senkronizasyon notu eklendi.
3. `Abyss_Kaynak_Butunlugu_Denetimi_v0.2.md` — v0.1 bulgularının güncel kararlar ışığında durumu eklendi.
4. `Abyss_Karar_Kaydi_v1.4.md` — iç sürüm başlığı dosya adıyla eşitlendi; karar metni değiştirilmedi.

## Bilinen sınırlar

- Bu işlem 512 sayfalık PDF’nin tamamını yeniden görsel olarak incelemedi.
- Kaynak indeksi alanlarının dolu olması, tüm mekaniklerin kesinleştiğini veya her literal eşleşmenin görsel doğrulandığını göstermez.
- Bu tur yalnızca yerel dosyaları güncelledi; dosyası burada bulunmayan eski GitHub raporlarının değiştirildiği varsayılmamalıdır.
- Açık Konular v1.0’daki 23 satır, 23 aktif karar bekleyen konu demek değildir: bazıları tamamlanan kararların tarihsel izleri, kapsam notları veya başka bir satırla birleştirilmiş pasif kayıtlardır.


## GitHub aktarım durumu

- Depo dosyaları bağlantı üzerinden okunabildi. Yeni dosya oluşturma isteği GitHub tarafından `403 Resource not accessible by integration` ile reddedildi; bu bağlantı üzerinden commit/push yapılmadı.
- Manuel yükleme paketi yalnızca depoda bulunmayan sürüm dosyalarını içerir. Eski sürümler silinmez veya tekrar yüklenmez.
