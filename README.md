<div align="center">

# 🦁 Galaksi Akademisi: Bilişsel Gelişim Platformu

**Okul öncesi (5-6 yaş) çocuklar için BİLSEM müfredatından ilham alan, algoritma ve görsel zeka odaklı, %100 Vanilla JS ile geliştirilmiş web tabanlı oyun.**

<!-- Rozetler -->
[![Live Demo](https://img.shields.io/badge/DEMO-Oyunu%20Oyna-success?style=for-the-badge&logo=google-chrome&logoColor=white)](https://yahyaa147.github.io/galaksi-akademisi/)
[![YouTube](https://img.shields.io/badge/VIDEO-Tanıtımı%20İzle-red?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/dNgb_fWWnCk)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Proje%20Detayları-blue?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/posts/yahya-%C3%B6zden-806319359_javascript-ve-ai-ile-e%C4%9Fitici-oyun-geli%C5%9Ftirme-activity-7402056807084650496-2KhK?utm_source=share&utm_medium=member_desktop&rcm=ACoAAFk2xkYBSxTGin65zUoHF_zVU0Ju-Bb0ees)

<!-- Teknoloji Stack -->
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![No Framework](https://img.shields.io/badge/Zero-Dependency-green?style=flat)

</div>

---
👨‍💻 Geliştirici ve Emeği Geçenler

Bu proje, Samsun Üniversitesi bünyesinde, akademik bir proje kapsamında geliştirilmiştir.
Geliştirici	
Yahya Özden	

## 📖 Proje Hakkında

**Galaksi Akademisi**, dijital okuryazarlığın temellerini atmak ve çocukların analitik düşünme becerilerini geliştirmek amacıyla tasarlanmış bir "EdTech" (Eğitim Teknolojileri) projesidir.

Günümüzde çocuklara yönelik birçok uygulama ya reklam barındırmakta ya da pedagojik altyapıdan yoksun olmaktadır. Bu proje, **Milli Eğitim Bakanlığı BİLSEM (Bilim ve Sanat Merkezleri)** sınavlarında kullanılan soru tiplerini (Matris, Örüntü, Sıralama) oyunlaştırarak güvenli ve eğitici bir ortam sunar.

Proje, herhangi bir oyun motoru veya JavaScript framework'ü (React, Vue vb.) kullanılmadan, tamamen **Saf (Vanilla) JavaScript** mimarisiyle geliştirilmiştir.

---

## 🎯 Temel Kazanımlar ve Pedagojik Altyapı

Oyun, Bloom Taksonomisi'nin "Bilgi" ve "Kavrama" basamaklarına hitap edecek şekilde kurgulanmıştır.

| İkon | Beceri Alanı | Açıklama |
| :---: | :--- | :--- |
| 🔄 | **Algoritmik Düşünme** | Olayları mantıksal bir sıraya koyma (Sequencing) ve neden-sonuç ilişkisi kurma. |
| 🧩 | **Soyut Düşünme** | Şekil-zemin ilişkisini kavrama, eksik parçayı tamamlama ve matris çözme. |
| 🎨 | **Görsel Dikkat** | Piksel tabanlı haritalama yaparak görsel odaklanma süresini artırma. |
| 👆 | **Psikomotor Gelişim** | Sürükle-Bırak mekanikleri ile ince motor becerilerini destekleme. |

---

## 🧠 Oyun Modülleri

### 1. 🎬 Hikaye Modu (Sıralama Algoritması)
Çocuğun önüne karışık olarak gelen olay kartlarını (Örn: Tohum -> Filiz -> Çiçek) mantıksal bir zaman çizelgesine göre sıralaması istenir.
*   **Teknik Detay:** `Drag & Drop API` kullanılarak nesnelerin yer değiştirmesi sağlanır.
*   **Eğitsel Hedef:** Kodlamanın temeli olan "adım adım işlem yapma" mantığını öğretir.

### 2. 🧩 Zeka Modu (Mantık & Matris)
2x2 veya daha büyük ızgaralardaki şekil örüntülerini analiz ederek eksik parçayı bulmayı hedefler.
*   **Teknik Detay:** Dinamik olarak oluşturulan DOM elementleri ve dizi (Array) karşılaştırmaları kullanılır.
*   **Eğitsel Hedef:** IQ testlerinde sıkça karşılaşılan matris mantığını kavratır.

### 3. 🎨 Sanat Modu (Görsel Kopyalama)
Sol tarafta verilen renkli desenin aynısını, sağ taraftaki boş ızgaraya kodlaması (boyaması) istenir.
*   **Teknik Detay:** Grid yapısı üzerinde tıklama olayları (Click Events) ile durum yönetimi (State Management) yapılır.
*   **Eğitsel Hedef:** Uzamsal algıyı ve dikkati güçlendirir.

---

## 🛠 Teknik Mimari ve Geliştirme Detayları

Bu proje, modern web teknolojilerinin sınırlarını zorlayarak **"Framework-Free"** (Kütüphanesiz) bir yaklaşımla geliştirilmiştir.

### ✅ 1. Zero-Dependency (Sıfır Bağımlılık)
Proje, harici hiçbir kütüphaneye (jQuery, Bootstrap, React vb.) ihtiyaç duymaz. Tek bir `index.html` dosyası tüm oyunu, stilleri ve mantığı barındırır.
*   **Avantajı:** Çok düşük dosya boyutu (<50KB), anında yüklenme süresi ve internet gerektirmeyen çalışma yapısı.

### ✅ 2. Web Audio API ile Kod Tabanlı Ses Sentezi
Oyunun boyutunu artırmamak için `.mp3` veya `.wav` dosyaları kullanılmamıştır. Bunun yerine JavaScript'in **AudioContext API**'si kullanılarak ses dalgaları kod ile üretilmiştir.

```javascript
/* Ses Motoru Örneği: Dosyasız Ses Üretimi */
const audioCtx = new (window.AudioContext || window.webkitAudioContext)();

function playTone(freq, type = 'sine') {
    const osc = audioCtx.createOscillator();
    const gain = audioCtx.createGain();
    
    osc.frequency.value = freq; // Frekans (Nota)
    osc.type = type;            // Dalga Tipi (Sine, Square vs.)
    
    // Envelope (Zarf) Tekniği: Sesi yumuşatma
    gain.gain.linearRampToValueAtTime(0.1, audioCtx.currentTime + 0.05);
    gain.gain.exponentialRampToValueAtTime(0.001, audioCtx.currentTime + 0.5);
    
    osc.connect(gain);
    gain.connect(audioCtx.destination);
    osc.start();
}
