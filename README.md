# Odoo 19 - Docker Environment 🚀

Repositori ini adalah template siap pakai untuk menjalankan **Odoo 19** menggunakan Docker. Struktur ini dirancang agar mudah digunakan di lokal untuk tahap pengembangan (development) dan siap di-deploy ke server produksi (VPS/Cloud).

## 📂 Struktur Direktori

* `/config`: Berisi file `odoo.conf` untuk konfigurasi utama Odoo.
* `/custom_addons`: Folder utama untuk meletakkan modul kustom (pihak ketiga atau buatan sendiri). Folder ini sudah di-mapping langsung ke dalam container Docker.
* `docker-compose.yml`: File orkestrasi untuk menjalankan service Odoo dan PostgreSQL.

## 🛠️ Cara Menjalankan Project (Lokal)

Pastikan Docker dan Docker Compose sudah terinstal di sistem Anda.

1. Buka terminal dan masuk ke direktori proyek ini.
2. Jalankan perintah berikut untuk menyalakan server di *background*:
   ```bash
   docker compose up -d