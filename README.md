# Cliopack TS-100 · Safety 4.0 Güvenlik ve Emniyet Analizi

**Hazırlayan:** Ensar Daş

Safety 4.0 Bootcamp laboratuvar föylerinden **Lab 1–4**, genel sürümdeki şişeleme hattı yerine **Cliopack TS-100 Yarı Otomatik Tabak Kapatma Makinası** için doldurulmuştur. Ek olarak makinenin **SWOT analizi** hazırlanmıştır.

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
| [Cliopack-TS100-SWOT-Analizi.pdf](Cliopack-TS100-SWOT-Analizi.pdf) | SWOT matrisi, ayrıntılı maddeler, TOWS stratejileri |

## Öne çıkan sonuçlar

- **Ana emniyet fonksiyonu:** Çekmece kilitlemeli kapanma izni. Çekmece kapalı ve kilitli değilse kafa inemez (tahmini **PL d**).
- **En kritik senaryo:** Uzak servis erişiminden reçete manipülasyonu, hatalı kapatma ve **tüketicide gıda zehirlenmesi** (skor 18, Kritik).
- **S=3 kuralı:** USB üzerinden sıcaklık limitinin yükseltilmesi (yanık/yangın) skoru düşük olsa da öne alındı.
- **Hedef mimari:** Jump server, VPN, MFA, kişisel hesap, oturum kaydı ve varsayılan kapalı erişim. Emniyet fonksiyonları ağdan bağımsız, kablolu ve kilitli.

## Kapsam notu

Üretici sayfasında kontrol sistemi, emniyet donanımı ve ağ bağlantısı hakkında bilgi yoktur. Bu konular **varsayım** olarak işaretlenmiştir (bkz. Makine Anlatımı, V1–V6). Uzak erişim modemi, föylerin istediği dijital kesişim noktalarını işlemek için eklenmiş bir senaryodur.

> Bu çalışma bir eğitim çıktısıdır; resmî denetim, uygunluk değerlendirmesi veya belgelendirme değildir ve CE/mevzuat uygunluğu garantisi vermez.
