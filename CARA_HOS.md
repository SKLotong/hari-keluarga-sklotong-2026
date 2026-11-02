# Cara hos flipbook di GitHub Pages

Folder ini (`output/digital/`) ialah laman statik lengkap. Tiada pelayan, tiada CDN; semua fon, gambar dan pustaka ada di dalam folder.

## Langkah (cara paling mudah, melalui laman web GitHub)
1. Log masuk ke github.com → **New repository** → nama contoh `hari-keluarga-sklotong-2026` → **Public** → Create.
2. Klik **uploading an existing file** → seret **semua isi** folder `output/digital/` (termasuk folder `halaman/`, `lib/`, `fon/` dan fail `.nojekyll`) → **Commit changes**.
3. **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → **Save**.
4. Tunggu 1–2 minit. Pautan: `https://<nama-pengguna>.github.io/hari-keluarga-sklotong-2026/`

## Uji di komputer sendiri
Buka `index.html` terus dalam Chrome/Edge/Safari (klik dua kali). Semua fungsi berjalan tanpa internet.

## Kemas kini kandungan (contoh jika PPD hadir dan aturcara berubah)
1. Ubah `src/buku.html`, kemudian bina semula:
   - `src/binaan.sh` (semak) → `python src/cetak.py .` (PDF) → `python src/digital.py .` (gambar WebP)
2. Muat naik semula fail dalam `halaman/` ke repositori.

## Fungsi
- Selak halaman (sentuh/seret, butang ‹ ›, kekunci anak panah).
- Telefon / potret: satu halaman. Komputer / landskap: dua halaman (bentangan buku).
- **Kandungan**: lompat terus ke mana-mana halaman.
- **Zum**: paparan penuh; cubit (pinch) atau butang + / −.
- Label hari di atas bertukar mengikut halaman (Jumaat 13 Nov / Isnin 16 Nov).
- Gambar dimuat berperingkat supaya halaman pertama cepat keluar walaupun internet lemah.
