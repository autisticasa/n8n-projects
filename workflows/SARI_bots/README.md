# 🌾 SARI – Sistem Tani Cerdas Indonesia (Si Tani Cerdas)

*Kategori:* Aplikasi Digital Berbasis AI untuk Agritech  
*Tahap:* Prototipe (Chatbot Telegram)

SARI adalah prototipe chatbot AI yang berfungsi sebagai asisten virtual pertanian. Fokusnya adalah membantu petani dengan *prediksi cuaca, **rekomendasi pupuk, dan **diagnosis penyakit tanaman*.

---

## Cara Kerja

1. *Input Pengguna*
   - Petani mengirim pertanyaan melalui chatbot Telegram, misal:  
     - "Cuaca hari ini di [lokasi]?"  
     - "Rekomendasi pupuk untuk padi?"

2. *Proses AI*
   - *Prediksi Cuaca:* Mengambil data dari API cuaca → memproses untuk rekomendasi waktu tanam.  
   - *Rekomendasi Pupuk:* Model AI menganalisis jenis tanaman, kondisi lahan, dan cuaca → menghasilkan rekomendasi pupuk.  
   - *Diagnosis Penyakit Tanaman (future):* Menggunakan model klasifikasi gambar untuk mendeteksi penyakit dari foto daun.

3. *Output*
   - Chatbot mengirim jawaban kepada pengguna secara real-time, berupa:
     - Informasi cuaca  
     - Rekomendasi pupuk  
     - Saran perawatan tanaman  

---

## Arsitektur Singkat

- *Chatbot AI:* Gateway komunikasi dengan pengguna.  
- *AI Engine:* Menjalankan logika prediksi dan rekomendasi.  
- *API Integrations:* Mengambil data eksternal (cuaca, jenis tanaman).  

---

## Teknologi
- Telegram Bot API  
- Python / Node.js (backend AI)  
- Machine Learning Models (Prediksi & Rekomendasi)  
- REST API untuk integrasi data  

---

## Catatan
- Marketplace hasil panen dan diagnosis penyakit berbasis gambar masih dalam tahap pengembangan.  
- Prototipe ini fokus pada workflow input → proses AI → output ke pengguna.
