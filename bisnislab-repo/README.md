# 🧪 BisnisLab

Racik ide bisnis → uji di simulasi usaha 12 bulan → praktikkan di dunia nyata dalam 30 hari.

Satu file HTML statis. **Tanpa API AI, tanpa backend, tanpa login.** Data tersimpan di browser pengguna (localStorage).

## Fitur
1. **Racik Ide** — pemantik ide acak, lembar ide, skor kelayakan 6 kriteria, business canvas otomatis.
2. **Simulasi Usaha** — 5 sektor (kuliner, fashion, jasa digital, produk digital, reseller skincare), 12 bulan dengan musim Ramadan/Lebaran & 11.11, kejadian acak (FYP TikTok, kompetitor banting harga, pinjol, bazar kampus), grafik kas, rapor + pelajaran, dan riwayat percobaan.
3. **Rencana Praktik** — kalkulator titik impas (BEP), checklist 30 hari sesuai sektor, ekspor ringkasan .txt.

## Online-kan di GitHub Pages (± 3 menit)
1. Buat repo baru di github.com, misalnya `bisnislab` (Public).
2. Klik **Add file → Upload files**, lalu upload `index.html`, `README.md`, dan `.nojekyll`.
3. Buka **Settings → Pages → Build and deployment → Source: Deploy from a branch**, lalu pilih branch `main` dan folder `/ (root)`. Klik **Save**.
4. Tunggu ±1 menit. Situs aktif di `https://<username>.github.io/bisnislab/`.

Lewat terminal:
```bash
git init && git add . && git commit -m "BisnisLab v1"
git branch -M main
git remote add origin https://github.com/<username>/bisnislab.git
git push -u origin main
```

## Mengubah angka simulasi
Semua parameter ada di objek `SEK` di `index.html` (harga pasar, HPP, biaya tetap, biaya promosi per calon pembeli, konversi, retensi, kapasitas, musim). Gaji pemilik diatur di `GAJI_PEMILIK`. Ubah angkanya, simpan, lalu push. Situs akan ter-update sendiri.

> Model simulasi sengaja disederhanakan untuk latihan berpikir, bukan untuk proyeksi keuangan.
