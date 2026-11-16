# Cliopack TS-100 · Safety 4.0 Güvenlik ve Emniyet Analizi

**Hazırlayan:** Ensar Daş · **Grup:** Gündüz B

Safety 4.0 Bootcamp laboratuvar föylerinin tamamı (**Lab 1–7**) genel sürümdeki şişeleme hattı yerine **Cliopack TS-100 Yarı Otomatik Tabak Kapatma Makinası** için doldurulmuştur. Ek olarak makinenin **SWOT analizi** hazırlanmıştır.

## Makine

TS-100, taze ya da pişmiş gıdaları plastik tabak içinde film ile kapatan yarı otomatik bir paketleme makinesidir. Tabaktaki hava vakumla alınır, gerekirse koruyucu gaz (MAP) basılır ve film ısıyla tabağa kaynatılır. Gövdesi AISI 304 paslanmaz çeliktir; 230 V ile çalışır, 1,5–3 kW güç çeker; gazlı modda dakikada 2–3, gazsız modda 4–6 çevrim yapar.

Emniyet açısından en kritik nokta: çekmece manuel olduğu için operatörün eli **her çevrimde** kalıp ve ~150–200 °C ısıtma plakası bölgesine girer.

Kaynak: <https://www.cliopack.com/ts-100-yari-otomatik-tabak-kapatma-makinasi>

## Dosyalar

| Dosya | İçerik |
|---|---|
| [Makine-Anlatimi.pdf](Makine-Anlatimi.pdf) | Üretici verileri, çalışma döngüsü, varsayımlar, tehlike özeti |
| [Laboratuvar1.pdf](Laboratuvar1.pdf) | **Safety Architecture:** tehlikeler, emniyet fonksiyonları, PLr, safe state, Safety Function Map (EP 03) |
| [Laboratuvar2.pdf](Laboratuvar2.pdf) | **IEC 62443 Mini Workshop:** 6 bölge, 6 conduit, uzak erişim kararları (EP 05) |
| [Laboratuvar3.pdf](Laboratuvar3.pdf) | **Threat & Risk + Risk Matrix:** 3 siber-fiziksel senaryo, L×S×E puanlama, Risk Register (EP 04) |
| [Laboratuvar4.pdf](Laboratuvar4.pdf) | **Secure Remote Access:** mevcut → hedef mimari, emniyet bağımsızlığı gereksinimleri (EP 02 + EP 06) |
| [Laboratuvar5.pdf](Laboratuvar5.pdf) | **SBOM / CVE / Patch:** üç şart kontrolü, durdurma kararı, test ve yama planı, safety validation, telafi edici önlemler (EP 09 · 10 · 11) |
| [Laboratuvar6.pdf](Laboratuvar6.pdf) | **CRA Incident Simulation:** 15 dk / 2 s / 24 s / 72 s / 14 gün müdahale akışı, kanıt ve sorumlular (EP 13) |
| [Laboratuvar7.pdf](Laboratuvar7.pdf) | **AI Safety Challenge:** YZ kapatma kalite kontrolünde üç başarısızlık için güvenli davranış, karar tablosu (EP 03 + EP 15) |
| [Cliopack-TS100-SWOT-Analizi.pdf](Cliopack-TS100-SWOT-Analizi.pdf) | SWOT matrisi, ayrıntılı maddeler, TOWS stratejileri |

## Öne çıkan sonuçlar

- **Ana emniyet fonksiyonu:** Çekmece kilitlemeli kapanma izni. Çekmece kapalı ve kilitli değilse kafa inemez (tahmini **PL d**).
- **En kritik senaryo:** Uzak servis erişiminden reçete manipülasyonu, hatalı kapatma ve **tüketicide gıda zehirlenmesi** (skor 18, Kritik).
- **S=3 kuralı:** USB üzerinden sıcaklık limitinin yükseltilmesi (yanık/yangın) skoru düşük olsa da öne alındı.
- **Hedef mimari:** Jump server, VPN, MFA, kişisel hesap, oturum kaydı ve varsayılan kapalı erişim. Emniyet fonksiyonları ağdan bağımsız, kablolu ve kilitli.
- **Zafiyet kararı:** Kritik CVE için üretim durdurulmaz. Erişim hemen kapatılır, yama önce test edilip planlı duruşta uygulanır ve emniyet fonksiyonları yeniden test edilir.
- **Olay müdahalesi:** Önce kontrollü durdurma ve emniyet testi, hemen ardından kanıt; reset yok. CRA bildirimini üretici (Cliopack) yapar, kullanıcı olayı üreticiye bildirir.
- **YZ:** Yalnızca kalite kararı verir; tek başına RED diyebilir ama OK diyemez. Emniyet fonksiyonları YZ'den bağımsızdır.

## Kapsam notu

Üretici sayfasında kontrol sistemi, emniyet donanımı ve ağ bağlantısı hakkında bilgi yoktur. Bu konular **varsayım** olarak işaretlenmiştir (bkz. Makine Anlatımı, V1–V7). Uzak erişim modemi (V6) föylerin istediği dijital kesişim noktalarını işlemek için, YZ kamera kalite kontrolü (V7) ise Lab 7 için eklenmiş senaryolardır.

> Bu çalışma bir eğitim çıktısıdır; resmî denetim, uygunluk değerlendirmesi veya belgelendirme değildir ve CE/mevzuat uygunluğu garantisi vermez.
