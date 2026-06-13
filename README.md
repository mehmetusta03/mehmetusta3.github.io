# 🚀 GitHub Pages'e Yükleme Rehberi

## Dosya Yapısı
```
mehmet-portfolio/
├── index.html    ← Ana sayfa (portfolio)
├── blog.html     ← Blog sayfası
└── style.css     ← Tüm stiller
```

---

## Adım Adım Kurulum

### 1. GitHub'da Repo Oluştur
- github.com → "New repository"
- Repo adı: `kullaniciadin.github.io`  
  *(örn: `mehmetusta03.github.io`)*
- Public seç ✅
- "Create repository" tıkla

### 2. Dosyaları Yükle
**Yöntem A — Web arayüzü (kolay):**
1. Repo sayfasında "uploading an existing file" linkine tıkla
2. 3 dosyayı sürükle bırak: `index.html`, `blog.html`, `style.css`
3. "Commit changes" tıkla

**Yöntem B — Git ile (öğrenmek için daha iyi):**
```bash
cd mehmet-portfolio
git init
git add .
git commit -m "İlk commit: portfolio sitesi"
git remote add origin https://github.com/kullaniciadin/kullaniciadin.github.io.git
git push -u origin main
```

### 3. GitHub Pages'i Aktifleştir
1. Repo → Settings → Pages
2. Source: **Deploy from a branch**
3. Branch: **main** / **(root)**
4. Save

### 4. Yayına Gir! 🎉
Birkaç dakika sonra:  
`https://kullaniciadin.github.io`

---

## Kendi Bilgilerini Ekle

`index.html` dosyasında şunları değiştir:
- `mehmet@ornek.com` → gerçek e-posta
- `linkedin.com/in/mehmetusta` → LinkedIn profilin
- Proje açıklamaları → kendi projelerinle güncelle
- Blog tarihleri ve içerikleri

## Yeni Blog Yazısı Eklemek
`blog.html`'de bir `blog-post-card` div'ini kopyala ve düzenle:
```html
<div class="blog-post-card" id="yazi-adim">
    <div class="blog-post-meta">
        <span class="blog-post-date">GÜN AY YIL</span>
        <span class="blog-post-category">KATEGORİ</span>
    </div>
    <h2>Yazı Başlığı</h2>
    <p>Kısa özet...</p>
    <a href="#" class="read-more">Devamını oku →</a>
</div>
```
