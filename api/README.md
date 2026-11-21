# Data Intro Tools LOL – Wild Rift

Pengganti server lama (introtoolsml.my.id). Dibaca langsung oleh aplikasi dari:
`https://raw.githubusercontent.com/bangzvl/LOL-ADS/main/api/<file>.json`

| File | Isi |
|---|---|
| `show.json` | Daftar intro: `id`, `name`, `category` (ANIME/TIKTOK/GAME/HERO/E-SPORT), `url_image`, `url_data` (zip), `url_video` (preview), `mode` (`public`/`private`) |
| `show_backup.json` | Intro asli (backup) dengan format yang sama |
| `show_ads.json` | Banner Rekomendasi: `url_image`, `url_data` (link saat diketuk) |
| `path_now.json` | Catatan nama file intro game terakhir yang diketahui (mis. `DynamicDownload/Video/Compliance/loginLoop_6D_01.mp4`). Aplikasi mendeteksi file otomatis |
| `thumbs/` | Thumbnail, diambil dari video preview tiap intro |

## Menambah intro baru
1. Upload zip intro ke repo konten (misal LOL-X-ANIME) dan video preview-nya.
2. Upload gambar thumbnail ke `api/thumbs/`.
3. Tambahkan satu entri di `show.json` (id harus unik). Urutan teratas tampil sebagai "Intro terbaru".

Perubahan langsung terbaca aplikasi (cache GitHub raw ±5 menit).
