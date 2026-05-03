# ⚔️ Kelime Savaşı

Mynet Kelime Savaşı'nın açık kaynaklı web klonu. Firebase ile gerçek zamanlı çevrimiçi düello desteği!

## 🎮 Oyun Modları

| Mod | Açıklama |
|-----|----------|
| 🌐 Çevrimiçi — Arkadaşla | Farklı cihazlardan gerçek zamanlı düello (Firebase) |
| 🤖 Yapay Zekaya Karşı | Bilgisayar rakibine karşı |
| 👥 İki Kişi (Aynı Cihaz) | Aynı cihazda sırayla |

## 🚀 Oyna

👉 **[Buradan Oyna](https://KULLANICI_ADIN.github.io/kelime-savasi)**

## 📖 Çevrimiçi Nasıl Oynanır?

1. İkisi de aynı siteye girer
2. Biri **"Çevrimiçi — Arkadaşla"** seçer → ad girer → lobi ekranında **4 haneli oda kodunu** alır
3. Diğeri aynı moda girer → **kodu girerek katılır**
4. Host **"Oyunu Başlat"** der → kategori seçer → düello başlar!

## 🛠 Kurulum & Yayınlama

### 1. Repo oluştur
```bash
git init
git add .
git commit -m "Kelime Savaşı - ilk sürüm"
git remote add origin https://github.com/KULLANICI_ADIN/kelime-savasi.git
git push -u origin main
```

### 2. GitHub Pages'i aç
GitHub repo → **Settings** → **Pages** → Source: `main` → `/ (root)` → **Save**

Birkaç dakika sonra: `https://KULLANICI_ADIN.github.io/kelime-savasi`

### 3. Firebase güvenlik kurallarını güncelle (önemli!)
Firebase Console → Realtime Database → **Rules** sekmesi:
```json
{
  "rules": {
    "rooms": {
      "$roomId": {
        ".read": true,
        ".write": true
      }
    }
  }
}
```

## 📦 Teknoloji

- Saf HTML + CSS + JavaScript
- Firebase Realtime Database (gerçek zamanlı senkronizasyon)
- Google Fonts (Bebas Neue + Nunito)
- **Sıfır bağımlılık**, tek dosya

## 🗂 Kategoriler

🍎 Meyve & Sebze · 🦁 Hayvanlar · 🌍 Ülkeler · 🏙️ Türkiye Şehirleri  
⚽ Spor · 🍕 Yemekler · 👨‍💼 Meslekler · 🎨 Renkler & Şekiller

## 📄 Lisans

MIT — Özgürce kullanın, geliştirin, paylaşın.
