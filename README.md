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

### 🎯 Temel Kazanımlar
*   **Algoritmik Düşünme:** Olayları mantıksal bir sıraya koyma (Sequencing).
*   **Görsel Algı:** Matris, şekil-zemin ilişkisi ve örüntü tamamlama.
*   **Psikomotor Gelişim:** İnce motor becerilerini destekleyen Sürükle-Bırak mekanikleri.

---

## 🧠 Oyun Modülleri ve İçerik

Oyun, Bloom Taksonomisi'nin kavrama basamaklarına uygun olarak 3 farklı modülden oluşur:

### 1. 🎬 Hikaye Modu (Sıralama)
Çocuğun önüne karışık olarak gelen olay kartlarını (Örn: Tohum -> Filiz -> Çiçek) mantıksal bir zaman çizelgesine göre sıralaması istenir. Bu modül, temel kodlama mantığı olan **"Sequence" (Sıralama)** becerisini ölçer.

### 2. 🧩 Zeka Modu (Mantık & Matris)
BİLSEM sınavlarında sıkça sorulan "Matris" sorularının dijital halidir. 2x2 veya daha büyük ızgaralardaki şekil örüntülerini analiz ederek eksik parçayı bulmayı hedefler.

### 3. 🎨 Sanat Modu (Görsel Dikkat)
Piksel tabanlı bir çizim oyunudur. Sol tarafta verilen renkli desenin aynısını, sağ taraftaki boş ızgaraya kodlaması (boyaması) istenir. Görsel dikkat ve uzamsal algıyı güçlendirir.

---

## 🛠 Teknik Mimari ve Özellikler

Bu proje "Single File Component" mantığına benzer şekilde, ancak **Build Tool (Webpack/Vite) kullanmadan** optimize edilmiştir.

### ✅ Zero-Dependency (Sıfır Bağımlılık)
Harici hiçbir kütüphane kullanılmamıştır. `index.html` dosyası tek başına tüm oyunu barındırır. Bu sayede kurulum gerektirmez, USB bellek ile taşınabilir ve internet olmadan çalışabilir.

### ✅ Web Audio API ile Ses Sentezi
Oyunun dosya boyutunu küçültmek için `.mp3` veya `.wav` dosyaları **kullanılmamıştır**. Bunun yerine JavaScript'in **AudioContext API**'si kullanılarak ses dalgaları (Oscillator) kod ile dinamik olarak üretilmiştir.

> **Teknik Not:** Ses motoru, `createOscillator()` ve `createGain()` metodlarını kullanarak Envelope (Zarf) tekniği ile yumuşak sesler üretir. Bu sayede tarayıcıda anlık ses sentezi yapılır.

### ✅ Hibrit Sürükle-Bırak (Drag & Drop)
Hem masaüstü (Mouse) hem de mobil (Touch) cihazlarda sorunsuz çalışması için `mousedown` yerine **Pointer Events API** kullanılarak evrensel bir sürükleme motoru yazılmıştır.

---

## 🚀 Nasıl Çalıştırılır?

Bu projeyi kendi bilgisayarınızda çalıştırmak için hiçbir kuruluma ihtiyacınız yoktur.

1.  Bu depoyu (repository) indirin veya klonlayın.
2.  `index.html` dosyasına çift tıklayın.
3.  Oyun tarayıcınızda açılacaktır. Hepsi bu kadar!

---

## 👨‍💻 Geliştirici ve Emeği Geçenler

Bu proje, **Samsun Üniversitesi** bünyesinde geliştirilmiştir.

| Rol | İsim |
| --- | --- |
| **Geliştirici** | [Yahya Özden](https://github.com/yahyaa147) |
| **Mentör / Danışman** | Dr. Öğr. Üyesi Nurettin Şenyer |
| **Mentör / Danışman** | Dr. Öğr. Üyesi Ömer Durmuş |

---

<div align="center">

**✨ Eğer bu projeyi beğendiyseniz sağ üstteki "Star" ⭐ butonuna basmayı unutmayın!**

</div>
