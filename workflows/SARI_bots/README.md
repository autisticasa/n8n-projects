# 🚀 Proyek n8n Saya (n8n-projects)

Selamat datang di repositori proyek n8n saya! Ini adalah kumpulan alur kerja (workflow) dan node kustom yang saya gunakan untuk mengotomatiskan berbagai tugas.

## 📁 Struktur Repositori

* **/workflows**: Berisi semua file `.json` workflow n8n. Anda bisa mengimpornya langsung ke instance n8n Anda.
* **/nodes**: (Opsional) Berisi kode untuk [node n8n kustom](https://docs.n8n.io/create-nodes/introduction/) yang saya buat.

## ⚙️ Cara Menggunakan Workflow

Setiap workflow dalam folder `/workflows` adalah file JSON yang independen.

1.  **Download:** Unduh file `.json` yang Anda perlukan.
2.  **Impor ke n8n:**
    * Buka kanvas (canvas) n8n Anda.
    * Gunakan pintasan `Ctrl + I` (atau `Cmd + I` di Mac) untuk "Import from File".
    * Pilih file `.json` yang sudah Anda unduh.

## ⚠️ Peringatan Kredensial

**Repositori ini tidak menyimpan kredensial (API keys, token, password).**

Saat Anda mengimpor workflow, Anda harus mengkonfigurasi **Kredensial** Anda sendiri di dalam instance n8n agar workflow tersebut dapat berfungsi.
