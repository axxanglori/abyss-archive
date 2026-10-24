# Abyss arşivi — GitHub Desktop ile manuel güncelleme

## GitHub bağlantısının test sonucu

Depodaki dosyalar okundu. Yeni dosya oluşturma denemesi GitHub API tarafından `403 Resource not accessible by integration` hatasıyla reddedildi. Bu sohbet bağlantısıyla doğrudan commit/push yapılamadı. Bu paket GitHub'a gönderilmeye hazırdır; kendi GitHub Desktop oturumunda commit edip push etmen gerekir.

## Paketin içeriği

ZIP'te 14 dosya var. Hiçbiri repodaki mevcut bir dosyanın aynı dosya adı değil; mevcut tarihsel sürümler korunur, yeni sürümler ayrı eklenir. Pakete mevcut `Abyss_OCR.txt` veya başka eski dosyalar yeniden konmadı.

- Karar Kaydı v1.4
- Kaynak Konum Eşleştirme v2.8 (CSV + Markdown özet)
- Kaynak Kapsam Matrisi v0.4 (CSV + Markdown özet)
- Kaynak Bütünlüğü Denetimi v0.2
- Origin/Güç Genel Kapsam ve Çelişki Raporu v0.6
- Origin/Güç Açık Konular v1.0 (CSV + Markdown özet)
- 99 kayıtlık Origin/Güç Takip v1.9 (CSV)
- Dosyalar Arası Senkronizasyon Denetimi v0.1
- Kanon/Taslak Çapraz Kontrol v0.1 (CSV + Markdown)
- `md_output/` içinde Envanter ve Karşılaştırma Raporu Güncelleme Eki v0.1

## Adım adım yükleme

1. ZIP dosyasını indir ve içeriğini çıkar.
2. GitHub Desktop'ta `axxanglori/abyss-archive` yerel deposunu aç. Üstte gösterilen **Local path** klasörünü açmak için `Repository > Show in Explorer` komutunu kullan.
3. ZIP içindeki dosyaları bu yerel depo klasörüne kopyala. `md_output` klasörünü ZIP'teki `md_output` alt klasörü ile birleştir; içindeki eski dosyaları silme.
4. GitHub Desktop'a dön. Changes listesinde yalnızca yukarıdaki 14 yeni dosyanın göründüğünü kontrol et. Bir dosyanın üzerine yazma uyarısı çıkarsa dur ve hedef klasördeki dosya adını kontrol et; bu paket mevcut aynı adlı dosyaları değiştirmemek için hazırlanmıştır.
5. Summary alanına `Add latest Abyss audit and canon files` yazıp **Commit to main** (veya GitHub Desktop'ın önerdiği mevcut branch) ile commit et.
6. **Push origin** düğmesine bas. Başarılı olduktan sonra GitHub web sitesinde dosyaları kontrol et.

## Ne yüklenmiyor ve neden?

- `Abyss_OCR.pdf` (yaklaşık 239 MB) pakete dahil değil: normal Git takibinde GitHub 100 MiB üzeri dosyaları reddeder. Bunun için Git LFS kurulumu/uygun depolama kotası veya başka bir dosya barındırma yeri gerekir.
- `Abyss_OCR.txt`, DOCX v1.2 ve mevcut tarihsel sürümler depoda zaten bulunuyor; aynı dosyalar yeniden eklenmiyor.
- GitHub'daki Envanter v0.8 ve karşılaştırma raporu v0.4 eski sürümleri silinmedi veya bu pakette aynı adla değiştirilmedi. Ek dosya, hangi durumların artık güncel olmadığını belirtir. Bu iki uzun belgenin sonraki tam sürümü, eski içerik eksiltilmeden ayrı çalışma olarak hazırlanmalıdır.
- `Abyss_Origin_Guc_Denetimi_Bekleyen_99_v1.1.csv` bu pakete eklenmedi; mevcut ana takip dosyası `Abyss_Origin_Guc_Denetimi_99_Kayit_Takip_v1.9.csv` olarak tutuluyor. Böylece eski "bekleyen" görünümü yeni takip dosyasıyla karıştırılmaz.

## Doğrulama

`Abyss_GitHub_Manuel_Yukleme_Paketi_v0.1_manifest.json`, pakete giren dosyaların byte büyüklükleri ve SHA-256 değerlerini kaydeder; manifest ayrı indirme dosyasıdır, repoya kopyalanması zorunlu değildir.
