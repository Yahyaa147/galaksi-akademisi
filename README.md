<div align="center">

# 🦁 Galaksi Akademisi: Bilişsel Gelişim Platformu

**Okul öncesi (5-6 yaş) çocuklar için BİLSEM müfredatından ilham alan, algoritma ve görsel zeka odaklı web tabanlı oyun.**

[![Live Demo](https://img.shields.io/badge/DEMO-Oyunu%20Oyna-success?style=for-the-badge&logo=google-chrome&logoColor=white)](https://yahyaa147.github.io/galaksi-akademisi/)
[![YouTube](https://img.shields.io/badge/VIDEO-Tanıtımı%20İzle-red?style=for-the-badge&logo=youtube&logoColor=white)](BURAYA_YOUTUBE_VIDEO_LINKINI_YAPISTIR)

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat-square&logo=javascript&logoColor=%23F7DF1E)

</div>

---

## 📖 Proje Hakkında

**Galaksi Akademisi**, dijital okuryazarlığın temellerini atmak ve çocukların analitik düşünme becerilerini geliştirmek amacıyla tasarlanmış bir "EdTech" (Eğitim Teknolojileri) projesidir. 

Proje, herhangi bir oyun motoru veya JavaScript framework'ü (React, Vue vb.) kullanılmadan, **%100 Saf (Vanilla) JavaScript** ile geliştirilmiştir. Bu tercih, projenin en düşük donanımlı cihazlarda bile yüksek performansla çalışmasını ve harici kütüphane bağımlılığı olmamasını sağlar.

### 🎯 Temel Amaçlar
*   **Algoritmik Düşünme:** Olayları mantıksal bir sıraya koyma (Sequencing).
*   **Görsel Algı:** Matris ve örüntü tamamlama becerileri.
*   **Psikomotor Gelişim:** İnce motor becerilerini destekleyen Sürükle-Bırak mekanikleri.

---

## 📸 Oyun İçi Görüntüler

Oyun, çocuk dostu arayüz prensipleri (büyük butonlar, canlı renkler, ikonografi) gözetilerek tasarlanmıştır.

| **Giriş ve Ana Menü** | **Görev Haritası** |
|:---:|:---:|
| <img src="assets/intro_screen.jpg" width="400" alt="Giriş Ekranı"> | <img src="assets/map_screen.jpg" width="400" alt="Harita Sistemi"> |
| *Sade ve anlaşılır karşılama ekranı.* | *Seviye bazlı ilerleme ve kilit sistemi.* |

<br>

| **Mod 1: Hikaye (Sıralama)** | **Mod 2: Zeka (Mantık)** |
|:---:|:---:|
| <img src="assets/game_story.jpg" width="400" alt="Hikaye Modu"> | <img src="assets/game_logic.jpg" width="400" alt="Zeka Modu"> |
| *Olay kartlarını doğru sıraya dizme.* | *Eksik parçayı bularak matrisi tamamlama.* |

<br>

| **Mod 3: Sanat (Görsel Dikkat)** | **Başarı ve Geri Bildirim** |
|:---:|:---:|
| <img src="assets/game_art.jpg" width="400" alt="Sanat Modu"> | <img src="assets/success_modal.jpg" width="400" alt="Başarı Ekranı"> |
| *Piksel tabanlı desen kopyalama.* | *Sesli ve görsel motivasyon sistemi.* |

---

## 🛠 Teknik Mimari ve Özellikler

Bu proje "Single File Component" mantığına benzer şekilde, ancak **Build Tool (Webpack/Vite) kullanmadan** optimize edilmiştir.

### 1. Zero-Dependency (Sıfır Bağımlılık)
Harici hiçbir kütüphane kullanılmamıştır. `index.html` dosyası tek başına tüm oyunu barındırır. Bu sayede kurulum gerektirmez ve USB bellek ile çevrimdışı çalışabilir.

### 2. Web Audio API ile Ses Sentezi
Oyunun dosya boyutunu küçültmek için `.mp3` veya `.wav` dosyaları kullanılmamıştır. Bunun yerine JavaScript'in **AudioContext API**'si kullanılarak ses dalgaları (Oscillator) kod ile dinamik olarak üretilmiştir.
```javascript
// Örnek: Kod ile üretilen yumuşak 'başarı' sesi
playSoft: (freq, type = 'sine') => {
    const osc = ctx.createOscillator();
    const gain = ctx.createGain();
    osc.frequency.value = freq; 
    // Envelope (Zarf) tekniği ile sesi yumuşatma
    gain.gain.linearRampToValueAtTime(0.1, ctx.currentTime + 0.05);
    osc.start();
}
