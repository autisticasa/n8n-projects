# 📊 Google Sheets Data Schema — SARI Chatbot

| Column Name        | Data Type | Description |
|--------------------|------------|-------------|
| id_produk          | String     | Unique ID for each product |
| nama_pupuk         | String     | Fertilizer name |
| stok_kg            | Number     | Available stock (in kilograms) |
| nama_tanaman       | String     | Related crop name |
| alat_pertanian     | String     | Associated agricultural tool |
| harga_tanaman_rp   | Number     | Crop price in Indonesian Rupiah |
| prediksi_pasar     | String     | Market trend prediction |
| pemasok_utama      | String     | Main supplier name |
| tanggal_update     | Date       | Last updated date |

---

### 📄 Example Data

| id_produk | nama_pupuk        | stok_kg | nama_tanaman | alat_pertanian | harga_tanaman_rp | prediksi_pasar | pemasok_utama       | tanggal_update |
|------------|-------------------|----------|---------------|----------------|------------------|----------------|--------------------|----------------|
| P001       | Pupuk NPK Mutiara | 120      | Padi          | Cangkul        | 5500             | Up 10%         | PT Agro Tani Jaya  | 2025-11-06     |
| P002       | Pupuk Urea        | 300      | Jagung        | Mini Tractor   | 4700             | Stable         | CV Makmur Subur    | 2025-11-05     |
