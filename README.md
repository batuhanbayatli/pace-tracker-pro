# 🧭 PACE Tracker Pro // bGroup Kinetik İntikal ve Yürüyüş Terminali

**PACE Tracker Pro**, bGroup ekosistemi bünyesinde **Batuhan Bayatlı** tarafından geliştirilmiş; iPhone ve Android cihazlar için optimize edilmiş saf HTML5, CSS3 ve JavaScript tabanlı profesyonel bir PWA (Progressive Web App) yürüyüş ve intikal takip asistanıdır.

## 🚀 Öne Çıkan Özellikler

* **Mobil Uyumlu HUD Ekranı:** Süre, mesafe (km), anlık hız, ortalama tempo, yakılan kalori ve donanımsal adımsayar verilerini devasa ve net kartlarla gösterir.
* **PACE Çökme Koruması (State-Persistence):** Telefonun şarjı bitse veya işletim sistemi sekmeyi kapatsa bile kurtarma motoru ölü zamanı ve mesafeyi telafi ederek oturumu kaldığı yerden kurtarır.
* **3 Fazlı Nabız Takibi:** Yürüyüş öncesi (dinlenme), yürüyüş sırasında (aktif ortalama) ve yürüyüş sonrasını (toparlanma) ayrı ayrı kaydeder.
* **Tartım ve Sıvı Kaybı Analizi:** Yürüyüş öncesi ve sonrası kilo farkından dehidrasyon (ter/sıvı kaybı) miktarını hesaplar.
* **Donanımsal Sensör Entegrasyonu:** Cihazın manyetometresiyle anlık pusula yönü (kerteriz) ve ivmeölçer ile adım kadansı sayımı.
* **GPX Rota İhracı:** Tamamlanan yürüyüşlerin rota koordinatlarını Garmin, Strava veya CBS yazılımlarına uyumlu `.gpx` dosyası olarak indirme imkanı.
* **Hava Durumu Güvenlik Kalkanı:** Open-Meteo altyapısıyla intikal sırasında yağmur veya aşırı sıcaklık uyarıları üretir.
* **Açık / Koyu Tema:** Sahra beji aydınlık tema ile gece operasyonları/akşam yürüyüşleri için AMOLED uyumlu koyu tema desteği.

## 📱 PWA Olarak Telefona Kurulum

Canlı sisteme [https://pace-tracker-pro.vercel.app/](https://pace-tracker-pro.vercel.app/) adresinden ulaştıktan sonra:
1. **iOS (Safari):** Paylaş butonuna bas ve **"Ana Ekrana Ekle"** seçeneğini seç.
2. **Android (Chrome):** Sağ üst menüden **"Uygulamayı Yükle"** veya **"Ana Ekrana Ekle"** de.

Uygulama tam ekran ve çevrimdışı (offline) olarak yerel bir mobil uygulama gibi çalışacaktır.

## 🏢 Geliştirici & Ekosistem
Bu yazılım, **bGroup** çatısı altında bağımsız bir teknoloji girişimi olarak tasarlanmış ve kodlanmıştır.

## 📂 Dosya Yapısı
Depo kök dizininde şu üç dosya yer almalıdır:
- `index.html` (Ana arayüz, tüm JavaScript motoru ve iOS/PWA ikon yapılandırması)
- `manifest.json` (PWA uygulama manifestosu)
- `sw.js` (Çevrimdışı önbellek için Service Worker)
