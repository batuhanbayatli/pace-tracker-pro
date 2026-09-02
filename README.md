# 🧭 PACE Tracker Pro 
> *bGroup Kinetik İntikal ve Yürüyüş Terminali*

[![PWA Ready](https://img.shields.io/badge/PWA-Ready-success?style=for-the-badge)](https://pace-tracker-pro.vercel.app/)
[![JavaScript](https://img.shields.io/badge/Vanilla-JS-yellow?style=for-the-badge&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)

**PACE Tracker Pro**, akıllı telefonları profesyonel birer kinetik intikal ve sahra telemetri terminaline dönüştüren, harici API maliyeti/bağımlılığı olmaksızın saf web standartlarıyla (HTML5, CSS3, Modern JS) inşa edilmiş yüksek performanslı bir **PWA (Progressive Web App)** çözümüdür. 

🔗 **Canlı Sistem:** [https://pace-tracker-pro.vercel.app/](https://pace-tracker-pro.vercel.app/)

---

## 🎖️ Operasyonel Mimari & Özellikler

### 1. Canlı HUD ve Kinetik Telemetri
* **Optimizasyonlu HUD:** Süre, kat edilen mesafe (km), anlık hız, ortalama tempo (`dk/km`), yakılan kalori (MET tabanlı) ve donanımsal adımları devasa tipografiyle anlık olarak yansıtır.
* **Taktik Yön & Rakım:** Cihazın manyetometresi ve ivmeölçeri üzerinden anlık pusula kerterizi (0°-360°), deniz seviyesinden rakım ve tırmanış kazancı (`+M`) takibi yapar.

### 2. PACE Çökme Koruma Motoru (State-Persistence)
> *Operasyonel Güvenilirlik Standardı*
* Cihazın şarjı bittiğinde, tarayıcı belleği temizlediğinde veya işletim sistemi uygulamayı arka planda kapattığında sistem devreye girer. 
* Yeniden açıldığında geçen "ölü zamanı" ve GPS delta mesafesini telafi ederek seansı kusursuz bir şekilde kurtarır ve kaldığı yerden devam ettirir.

### 3. Biyometrik & Sıhhi Takip Protokolü
* **3 Fazlı Nabız Analizi:** Yürüyüş öncesi (dinlenme), yürüyüş sırasında (aktif seans ortalaması) ve yürüyüş sonrası (toparlanma) nabız değerlerini faz güvenlik kurallarına göre ayrı ayrı mühürler.
* **Dehidrasyon & Tartım Analizi:** Yürüyüş öncesi ve sonrası vücut ağırlığı mukayesesiyle ter/sıvı kaybını otomatik hesaplar.

### 4. Harici Bağımsızlık & Donanım Entegrasyonu
* **Sıfır Sunucu Bağımlılığı:** Veriler doğrudan tarayıcının yerel güvenli alanında (`localStorage`) şifresiz ve hızlı bir şekilde saklanır.
* **Donanımsal Adımsayar:** GPS uydularının kör noktada kaldığı tünel veya kapalı alanlarda 3 eksenli ivmeölçer (DeviceMotion) sensörüyle adımları saymaya devam eder.
* **GPX Rota İhracı:** Tamamlanan yürüyüşleri zaman damgalı `.gpx` formatında indirerek Garmin, Strava veya CBS yazılımlarına aktarma imkanı sağlar.
* **Atmosferik Güvenlik Kalkanı:** Açık kaynaklı Open-Meteo entegrasyonuyla intikal esnasında yaşanabilecek ani yağış veya aşırı sıcaklık (`>=33°C`) risklerine karşı tek seferlik uyarı mekanizması barındırır.

---

## 📱 PWA Olarak Cihaza Kurulum

Uygulamayı tarayıcı çubuklarından arındırılmış tam ekran yerel bir mobil uygulama gibi kullanmak için:

* **iOS (Safari):** Adresi açın $\rightarrow$ Paylaş menüsüne dokunun $\rightarrow$ **"Ana Ekrana Ekle"** deyin.
* **Android (Chrome):** Adresi açın $\rightarrow$ Sağ üst menüden **"Uygulamayı Yükle"** veya **"Ana Ekrana Ekle"** seçeneğini seçin.

---

## 📂 Depo Dosya Mimarisi

```text
📦 pace-tracker-pro
 ┣ 📜 index.html        # Ana arayüz, telemetri motoru ve PWA ikon yapılandırması
 ┣ 📜 manifest.json     # Uygulama manifestosu (Standalone & Mobil Kimliği)
 ┗ 📜 sw.js             # Service Worker (Çevrimdışı / Sahra önbellek protokolü)
