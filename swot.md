# SWOT Analizi — Cliopack TS-100 Yarı Otomatik Tabak Kapatma Makinası

| Ad Soyad | Grup | Tarih |
|---|---|---|
| Ensar Daş | | 23.10.2026 |

> Kapsam: Ürünün **pazar konumu** ile **Safety 4.0** (iş güvenliği + siber güvenlik + mevzuat) boyutu birlikte değerlendirilmiştir. Veriler üretici sayfasından alınmıştır, varsayımlar [00-makine-profili.md](00-makine-profili.md) dosyasında listelenmiştir.

## Özet matris

| | Yardımcı | Zararlı |
|---|---|---|
| **İç** | **S — Güçlü yönler**<br/>• AISI 304 paslanmaz gövde, gıdaya uygun<br/>• Gazlı (MAP) + gazsız vakum tek makinede<br/>• Değiştirilebilir kalıp: 3 farklı tabak düzeni<br/>• 13 dilli LCD panel, IP65 butonlar<br/>• Kompakt (930×1250×690 mm, 120 kg), tek faz 230 V<br/>• CE, sessiz ve titreşimsiz çalışma<br/>• Yerli üretim: servis ve yedek parçaya hızlı erişim | **W — Zayıf yönler**<br/>• Düşük kapasite: 2–3 (gazlı) / 4–6 (gazsız) çevrim/dk<br/>• Manuel çekmece: operatör eli her çevrimde tehlike bölgesinde<br/>• Maks. tabak 325×265 mm, film çapı 220 mm ile sınırlı<br/>• Vakum pompası opsiyonel; spesifikasyonda birim tutarsızlığı (m³/s)<br/>• Emniyet mimarisi, PL seviyesi, sıcaklık aralığı yayımlanmamış<br/>• Veri bağlantısı / Endüstri 4.0 özelliği yok; siber güvenlik dokümantasyonu yok |
| **Dış** | **O — Fırsatlar**<br/>• Hazır yemek, şarküteri ve taze et paketlemede büyüme<br/>• KOBİ, kasap, catering, restoran zincirleri için uygun fiyat/kapasite<br/>• Çok dilli panel sayesinde ihracat (Orta Doğu, Balkanlar, Rusya, Hindistan)<br/>• AB Makine Yönetmeliği ve CRA'yı erken karşılayarak "güvenli makine" farkı<br/>• Opsiyonel IoT modülü: üretim sayacı, reçete kilidi, uzaktan güvenli servis<br/>• Geri dönüştürülebilir mono-materyal film/tabak trendi | **T — Tehditler**<br/>• Düşük fiyatlı Asya menşeli rakipler<br/>• Tam otomatik hat çözümleri (büyük üreticiler)<br/>• **AB 2023/1230 Makine Yönetmeliği** (20.01.2027'den itibaren): siber "bozulmaya karşı koruma" ve emniyet yazılımı gereklilikleri<br/>• **CRA (AB 2024/2847):** bağlantılı ürünlerde zafiyet bildirimi (11.09.2026'dan beri), tam uygulama 11.12.2027<br/>• Ambalaj yönetmeliği (PPWR) ile film/tabak uyumluluk baskısı<br/>• Paslanmaz çelik fiyatı, kur dalgalanması<br/>• Uzaktan servis eklenirse siber saldırı yüzeyi |

## Ayrıntılar

### S — Güçlü Yönler (Strengths)

1. **Gıda hijyenine uygun yapı.** Tüm gövde AISI 304 paslanmaz çelik, butonlar IP65. Yıkamalı gıda ortamlarına dayanıklı, temizliği kolay.
2. **Esneklik.** Aynı makine gazlı (MAP) ve gazsız vakum paketleme yapabiliyor. Değiştirilebilir kalıplarla 1 büyük, 1 orta ya da 2 küçük tabak paketlenebiliyor; ürün çeşitliliği yüksek işletmeler için avantaj.
3. **Kullanım kolaylığı.** 13 dil seçenekli LCD panel, operatör eğitimini kısaltıyor ve ihracatta yerelleştirme maliyetini düşürüyor.
4. **Kompakt ve kolay kurulum.** 120 kg ağırlık ve tek faz 230 V besleme sayesinde küçük atölyelere kolayca giriyor; özel elektrik altyapısı gerekmiyor.
5. **Basit mimari.** Yarı otomatik ve ağ bağlantısız olduğu için standart haliyle **siber saldırı yüzeyi çok küçük**. Bu, Safety 4.0 bakışından bir güçlü yan.
6. **CE işaretli üretim**, sessiz ve titreşimsiz çalışma.

### W — Zayıf Yönler (Weaknesses)

1. **Kapasite.** Gazlı modda 2–3 çevrim/dk (çift tabakla saatte en fazla ~360 paket), orta-büyük üretici için yetersiz.
2. **Operatör maruziyeti.** TS-100'de çekmece manuel (otomatik çekmece yalnızca TS-120 SE'de). Operatör her çevrimde eli ile kalıp/ısıtma bölgesine giriyor. Emniyet tamamen interlock'un güvenilirliğine bağlı (Lab 1: PLr d).
3. **Şeffaflık eksikliği.** Kamuya açık sayfada emniyet fonksiyonları, Performance Level, kapatma sıcaklığı, hava basıncı ve kontrol donanımı belirtilmemiş. Vakum pompası değerinde birim hatası (m³/s) var. Bu durum kurumsal alıcının teknik değerlendirmesini zorlaştırıyor.
4. **Endüstri 4.0 eksikliği.** Üretim verisi, reçete yönetimi, izlenebilirlik (lot, sıcaklık kaydı) için bağlantı yok. Gıda güvenliği denetimlerinde (HACCP, BRC/IFS) kayıt elle tutulmak zorunda.
5. **Siber güvenlik ve SBOM dokümantasyonu yok.** Sonradan uzak erişim eklenirse güvenli kurulum kılavuzu ve yazılım bileşen listesi bulunmuyor.
6. Tabak/film ölçü sınırları büyük porsiyon ve aile boyu paketleri dışarıda bırakıyor.

### O — Fırsatlar (Opportunities)

1. **Pazar büyümesi.** Hazır yemek, paket et/şarküteri ve online market siparişlerinde raf ömrü uzatan MAP paketlemeye talep artıyor. KOBİ, kasap, restoran zinciri ve catering segmenti bu kapasite için ideal.
2. **İhracat.** 13 dilli arayüz ve CE işareti; Orta Doğu, Balkanlar, BDT ve Hindistan pazarlarına giriş için hazır bir altyapı sunuyor.
3. **Mevzuatı fırsata çevirmek.** AB Makine Yönetmeliği 2023/1230 ve CRA'yı rakiplerden önce karşılayan bir sürüm ("TS-100 Secure"): kablolu emniyet rölesi (PL d), kilitli emniyet parametreleri, SBOM, güvenli uzak servis. AB'ye satış yapan gıda üreticileri bunu tedarikçiden talep edecek.
4. **Opsiyonel güvenli IoT modülü.** Üretim sayacı, sıcaklık/süre kaydı (HACCP kanıtı), reçete kilidi, jump server üzerinden varsayılan kapalı uzak servis. Hem yeni gelir kalemi hem gıda izlenebilirliği için değer.
5. **Sürdürülebilir ambalaj.** Geri dönüştürülebilir mono-materyal film ve tabaklarla uyumlu kalıp/reçete paketleri.
6. **Servis ve sarf geliri.** Kalıp setleri, film ve bakım sözleşmeleri.

### T — Tehditler (Threats)

1. **Fiyat rekabeti.** Düşük maliyetli Asya menşeli tabak kapatma makineleri, özellikle ihracat pazarlarında.
2. **Otomasyon baskısı.** Büyüyen müşteriler kısa sürede tam otomatik hat (in-line tray sealer) çözümlerine geçebiliyor.
3. **Regülasyon maliyeti.**
   - **AB 2023/1230 Makine Yönetmeliği** 20 Ocak 2027'de uygulanmaya başlıyor. Kontrol sistemlerinin kötü niyetli bozulmaya karşı korunmasını ve emniyet yazılımının kayıt altında olmasını istiyor.
   - **Siber Dayanıklılık Yasası (CRA, AB 2024/2847):** Dijital bileşenli/bağlantılı ürünlerde aktif istismar edilen zafiyetlerin 24 saat / 72 saat / 14 gün içinde bildirilmesi **11 Eylül 2026'dan beri** zorunlu; tüm gereklilikler 11 Aralık 2027'de devreye giriyor. Uzak erişim modülü eklenirse TS-100 bu kapsama girer.
   - **PPWR (AB Ambalaj Yönetmeliği)** film ve tabaklarda geri dönüştürülebilirlik şartları getiriyor; makinenin yeni malzemelerle uyumlu olması gerekebilir.
4. **Siber-fiziksel risk.** Sahada servis firmalarının eklediği güvensiz 4G modemler (Lab 3 R1, R2) hem itibar hem sorumluluk riski yaratıyor. Bir gıda zehirlenmesi vakası makineye bağlanırsa marka zarar görür.
5. **Ekonomik etkenler.** Paslanmaz çelik ve elektronik bileşen fiyatları, kur dalgalanmaları.
6. **İş kazası sorumluluğu.** Manuel çekmeceli tasarımda interlock arızasına bağlı bir el yaralanması ürün sorumluluğu davasına yol açabilir.

## SWOT'tan stratejiler (TOWS)

| Strateji | Açıklama |
|---|---|
| **S-O (güçle fırsatı yakala)** | Paslanmaz, çok dilli ve kompakt yapıyı "HACCP kayıtlı, güvenli IoT opsiyonlu" bir paketle ihracat ve KOBİ pazarına sun. |
| **W-O (zayıflığı fırsatla gider)** | Kayıt/izlenebilirlik eksikliğini opsiyonel IoT modülüyle kapat; emniyet ve siber dokümantasyonu (PL, SBOM, güvenli kurulum kılavuzu) yayımla. |
| **S-T (güçle tehdide karşı koy)** | Ağsız, basit mimariyi "küçük saldırı yüzeyi" olarak pazarla; CE dosyasını 2023/1230'a göre şimdiden güncelle. |
| **W-T (savunma)** | Manuel çekmece riskini PL d kablolu interlock, iki el kumanda veya otomatik çekmece opsiyonuyla azalt; sahada eklenen modemler için servis politikası belirle (jump server, MFA, varsayılan kapalı). |

*Bu çalışma bir eğitim çıktısıdır; resmî denetim, uygunluk değerlendirmesi veya belgelendirme değildir.*
