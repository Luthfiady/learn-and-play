# Learn & Play 🎈 — Grade 1 Math & English

PWA belajar untuk anak kelas 1. Auto-deploy ke GitHub Pages setiap push ke `main`.

## Struktur
```
app/                       ← seluruh isi aplikasi (yang di-publish)
  index.html               ← semua logika & materi ada di sini
  manifest.webmanifest, sw.js, icon-*.png
.github/workflows/deploy.yml  ← workflow auto-deploy
```

## Cara update materi
1. Edit `app/index.html`
2. `git add . && git commit -m "update materi" && git push`
3. Tunggu ±1 menit → cek tab **Actions** → live di URL Pages.

Versi cache service worker di-stamp otomatis oleh workflow, jadi
tidak perlu edit `sw.js` manual tiap update.
