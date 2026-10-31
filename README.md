# 🧟 Zombi Hayatta Kalma

Tarayıcıda çalışan, tek dosyalık 3D zombi hayatta kalma oyunu. Kurulum yok, derleme yok: `index.html` dosyasını açman yeterli. Hem bilgisayarda (klavye + fare) hem telefonda (dokunmatik butonlar) oynanır.

> Three.js (r128) ile yazıldı. Ses efektleri WebAudio ile koddan üretilir, harici ses/görsel dosyası yoktur.

## ✨ Özellikler

**Dünya**
- 4×4 km'lik, oynarken yüklenen sonsuz hissi veren harita
- Küçük evlerden 10 katlı binalara kadar farklı bina tipleri
- Dört farklı ağaç tipi, bahçelere rastgele dağılır
- Gündüz / akşam / gece döngüsü, geceleri pencereler yanar

**Evler**
- Tüm binalara girilebilir, açılıp kapanan kapıları var
- İçlerinde televizyon, kanepe ve yatak bulunur
- İç merdivenle üst kata çıkılabilir
- Kapıyı kapatırsan zombiler giremez, açık bırakırsan içeri girip her katta kovalarlar
- Yatakta dinlenince can yenilenir

**Zombiler**
- Sürüler halinde gelir, her dalgada güçlenir
- Oyuncak oranlı insan figürü (büyük kafa, eller, ayakkabılar)
- **Geceleri mutantlar** çıkar: büyük, dayanıklı ve çok sert vuruyorlar. Gün doğunca güneşte yanıp ölürler
- Hepsinin sesi var, gece geçişinde ürkütücü bir ses çalar

**Araçlar ve silahlar**
- Araba, tank ve uçak
- Tank mermisi zombileri havaya savurur, kan fışkırır, ekran sarsılır
- 4 silah: AK-47, pompalı, tabanca, taramalı
- Yumruk, fener, şarjör sistemi, can/mermi toplama

**Diğer**
- Silahlı askerler: sen ateş etmedikçe ekibe katılıp zombileri vurur, ona ateş edersen sana saldırır
- 10 katlı binaların üstünde roket atan helikopterler
- Mini harita, skor, dalga sistemi

## 🎮 Kontroller

| Eylem | Klavye / Fare | Mobil |
|---|---|---|
| Yürü | W A S D | Sol joystick |
| Bak / nişan | Fare | Sağ ekranı sürükle |
| Ateş | Sol tık | 🔥 |
| Koş | Shift | 🏃 |
| Zıpla | Boşluk | 🦘 |
| Şarjör | R | ↺ |
| Silah değiştir | Q | 🔄 |
| Yumruk | E | 👊 |
| Kapı aç/kapat | G | 🚪 |
| Fener | L | 🔦 |
| Araca bin / in | F | 🚗 |

Uçakta: W ile gaz ver, hız 25'i geçince fareyi yukarı çek.

## ▶️ Çalıştırma

**En kolayı:** `index.html` dosyasını tarayıcıda aç.

> Three.js CDN'den yüklendiği için internet bağlantısı gerekir.

**GitHub Pages ile yayınlamak için:**
1. Repo → **Settings** → **Pages**
2. Source: `main` branch, `/ (root)`
3. Birkaç dakika sonra `https://KULLANICI_ADIN.github.io/REPO_ADI/` adresinden oynanır

## 🛠️ Teknik notlar

- Tek dosya: HTML + CSS + JS bir arada (`index.html`)
- Render: Three.js r128 (cdnjs)
- Harita parçalar halinde (chunk) üretilir ve uzaklaşınca silinir
- Mobilde gölge ve piksel yoğunluğu düşürülür, zombi sayısı sınırlanır

## 📄 Lisans

İstediğin lisansı ekleyebilirsin (örneğin MIT).
