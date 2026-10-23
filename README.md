# Safety 4.0 Bootcamp — Cliopack TS-100 Laboratuvar Çalışması

Safety 4.0 Bootcamp (INSPECCO × KRIPTARIUM) laboratuvar föylerinin **Lab 1–4** bölümleri, genel sürümdeki "şişeleme hattı" yerine **Cliopack TS-100 Yarı Otomatik Tabak Kapatma Makinası** için doldurulmuştur. Ayrıca makine için bir **SWOT analizi** eklenmiştir.

Makine sayfası: <https://www.cliopack.com/ts-100-yari-otomatik-tabak-kapatma-makinasi>

## İçerik

| Dosya | Konu | Evidence Pack |
|---|---|---|
| [00-makine-profili.md](00-makine-profili.md) | Makine verileri, çalışma döngüsü ve yapılan varsayımlar | — |
| [lab1-safety-architecture.md](lab1-safety-architecture.md) | **LAB 1** · Safety Architecture → Safety Function Map | EP 03 |
| [lab2-iec62443.md](lab2-iec62443.md) | **LAB 2** · IEC 62443 Mini Workshop → Zone / Conduit Diagram | EP 05 |
| [lab3-risk-register.md](lab3-risk-register.md) | **LAB 3** · Threat & Risk + Risk Matrix → Risk Register | EP 04 |
| [lab4-secure-remote-access.md](lab4-secure-remote-access.md) | **LAB 4** · Secure Remote Access → Secure Architecture | EP 02 + EP 06 |
| [swot.md](swot.md) | SWOT analizi + TOWS stratejileri | — |

## Özet

- **Ana tehlike:** Operatör her çevrimde (dakikada 2–6 kez) elini kalıba sokuyor; kapanan pnömatik kafa ve 150–200 °C ısıtma plakası **ezilme + yanık** riski yaratıyor.
- **Ana emniyet fonksiyonu:** Çekmece kilitlemeli kapanma izni (SF1, tahmini **PL d**) ve acil stop (SF2).
- **En kritik siber-fiziksel senaryo:** Uzak erişimden reçete manipülasyonu → hatalı kapatma → **gıda zehirlenmesi** (skor 18, Kritik).
- **Hedef mimari:** Jump server + VPN + MFA + kişisel hesap + oturum kaydı + varsayılan kapalı erişim; emniyet fonksiyonları ağdan bağımsız, kablolu ve kilitli.

## Not

Üretici sayfasında kontrol sistemi, emniyet donanımı ve ağ bağlantısı hakkında bilgi bulunmadığından bu konular [makine profilinde](00-makine-profili.md) **varsayım** olarak işaretlenmiştir. Diyagramlar Mermaid ile yazılmıştır ve GitHub'da doğrudan görüntülenir.

> Bu föyler bir eğitim çıktısıdır; resmî denetim, uygunluk değerlendirmesi veya belgelendirme değildir ve CE/mevzuat uygunluğu garantisi vermez.
