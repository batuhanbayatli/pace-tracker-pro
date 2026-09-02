<div align="center">

# 🧭 PACE TRACKER PRO
### *bGroup Kinetik İntikal ve Sahra Telemetri Terminali*

[![bGroup Ecosystem](https://img.shields.io/badge/bGroup-Ecosystem-0f172a?style=for-the-badge&logo=codeforces&logoColor=38bdf8)](https://github.com/BatuhanBayatli)
[![PWA Ready](https://img.shields.io/badge/PWA-Standalone-0284c7?style=for-the-badge&logo=pwa&logoColor=white)](https://pace-tracker-pro.vercel.app/)
[![Vanilla Stack](https://img.shields.io/badge/Stack-HTML5%20%7C%20CSS3%20%7C%20JS-f59e0b?style=for-the-badge&logo=javascript&logoColor=white)](https://pace-tracker-pro.vercel.app/)
[![Status](https://img.shields.io/badge/Status-Operational-10b981?style=for-the-badge)]()

<p align="center">
  <b>Akıllı telefonları profesyonel birer kinetik telemetri terminaline dönüştüren, sıfır bağımlılıklı web standardı çözümü.</b>
</p>

[Canlı Sistemi İncele](https://pace-tracker-pro.vercel.app/) • [Kurulum Rehberi](#-mobil-cihaza-pwa-kurulumu)

---

</div>

## 🌐 bGroup Ekosistem Etiketi
Bu yazılım; **bGroup** çatı organizasyonunun vizyoner teknoloji yaklaşımı çerçevesinde, modern web mimarileri ve çevrimdışı öncelikli *(offline-first)* prensiplerle tasarlanmış tescilli bir ekosistem ürünüdür.

```yaml
bGroup_Framework:
  Venture_Tier: "Model & Mutfak Tier-1"
  Developer: "Batuhan Bayatlı"
  Architecture: "Serverless PWA & Hardware-Assisted Telemetry"
  Ecosystem_Scope: "bGroup Core Technologies"
```

🎖️ Operasyonel Mimari ve Teknik Kabiliyetler
1. 📊 Canlı HUD & Kinetik Telemetri
Yüksek Hassasiyetli HUD: Süre, kat edilen mesafe (km), anlık hız, ortalama tempo (dk/km), MET tabanlı dinamik kalori sarfiyatı ve donanımsal adımları monospaced tipografiyle yansıtır.

Taktik Yön & Rakım: Cihazın manyetometresi ve ivmeölçeri üzerinden anlık pusula kerterizi (0°-360°), deniz seviyesinden rakım ve kümülatif tırmanış kazancı (+M) takibi.

2. 🛡️ PACE Çökme Koruma Motoru (State-Persistence)
Operasyonel Güvenilirlik Standardı

Cihazın şarjı bittiğinde, tarayıcı belleği temizlediğinde veya işletim sistemi uygulamayı arka planda kapattığında sistem devreye girer.

Yeniden açıldığında geçen "ölü zamanı" ve GPS delta mesafesini otomatik telafi ederek seansı kusursuz bir şekilde kurtarır ve kaldığı yerden devam ettirir.

3. 🫀 Biyometrik & Sıhhi Takip Protokolü
3 Fazlı Nabız Analizi: Yürüyüş öncesi (dinlenme), yürüyüş sırasında (aktif seans ortalaması) ve yürüyüş sonrası (toparlanma) nabız değerlerini faz güvenlik kurallarına göre ayrı ayrı mühürler.

Dehidrasyon & Tartım Analizi: Yürüyüş öncesi ve sonrası vücut ağırlığı mukayesesiyle ter/sıvı kaybını milimetrik olarak hesaplar.

4. ⚙️ Donanım & Harici Bağımsızlık
Sıfır Sunucu Bağımlılığı: Veriler doğrudan tarayıcının yerel güvenli alanında (localStorage) şifresiz ve milisaniyeler içinde saklanır.

Donanımsal Adımsayar: GPS uydularının kör noktada kaldığı kapalı alanlarda 3 eksenli ivmeölçer (DeviceMotion) sensörüyle adımları saymaya devam eder.

GPX Rota İhracı: Tamamlanan yürüyüşleri zaman damgalı .gpx formatında indirerek Garmin, Strava veya CBS yazılımlarına aktarma imkanı sağlar.

Atmosferik Güvenlik Kalkanı: Açık kaynaklı Open-Meteo entegrasyonuyla intikal esnasında yaşanabilecek ani yağış veya aşırı sıcaklık (>=33°C) risklerine karşı erken uyarı mekanizması barındırır.

📱 Mobil Cihaza PWA Kurulumu
Uygulamayı tarayıcı çubuklarından arındırılmış tam ekran yerel bir mobil uygulama gibi kullanmak için:

 iOS (Safari): Adresi açın → Paylaş menüsüne dokunun → "Ana Ekrana Ekle" seçeneğini seçin.

🤖 Android (Chrome): Adresi açın → Sağ üst menüden "Uygulamayı Yükle" veya "Ana Ekrana Ekle" seçeneğini seçin.

📂 Depo Dosya Mimarisi
Plaintext
📦 pace-tracker-pro
 ┣ 📜 index.html        # Ana arayüz, telemetri motoru ve PWA ikon yapılandırması
 ┣ 📜 manifest.json     # Uygulama manifestosu (Standalone & Mobil Kimliği)
 ┗ 📜 sw.js             # Service Worker (Çevrimdışı / Sahra önbellek protokolü)
🏛️ Geliştirici & Telif
Bu yazılım ve mimari, bGroup ekosistemi çatısı altında Batuhan Bayatlı tarafından bağımsız bir teknoloji girişimi olarak tasarlanmış, kodlanmış ve sahaya sürülmüştür.
