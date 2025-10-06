# 💨 Analisis Komprehensif Indeks Standar Pencemar Udara (ISPU) DKI Jakarta

## 🌟 Ringkasan Proyek Eksekutif

Proyek ini menyajikan analisis data komprehensif Indeks Standar Pencemar Udara (ISPU) di DKI Jakarta. Dengan memanfaatkan Python dan *library* visualisasi data, *dashboard* ini dikembangkan untuk mengidentifikasi **pola polusi**, **wilayah *hotspot***, dan **polutan dominan** yang memerlukan tindakan mitigasi.

Analisis dibagi menjadi empat bagian visual utama untuk memberikan wawasan strategis, mencakup aspek Temporal (Waktu), Spasial (Lokasi), dan Komposisi Pencemar.

---

## 🔑 Data dan Alat

| Komponen | Deskripsi |
| :--- | :--- |
| **Data Sumber** | Data Indeks Standar Pencemar Udara (ISPU) DKI Jakarta (Format XLSX/CSV). |
| **Lingkungan** | Google Colaboratory (direkomendasikan untuk eksekusi kode Python). |
| **Library Kunci** | `pandas` (Manipulasi Data), `matplotlib` & `seaborn` (Visualisasi Profesional). |
| **Analisis Fokus** | Dominasi $\text{PM}_{2.5}$, Tren Bulanan, Pola Hari-Minggu, dan Korelasi Antar-Pencemar. |

---

## 📈 Struktur *Dashboard* dan Wawasan Kunci

*Dashboard* ini terstruktur untuk menjawab pertanyaan analitik utama melalui serangkaian visualisasi yang saling melengkapi:

### 1. Status Risiko & Komposisi Polutan (Bagian I & III)

* **Risiko Kesehatan:** Mengukur **persentase hari** yang dikategorikan **TIDAK SEHAT** ($\text{ISPU} > 100$) secara keseluruhan.
* **Pencemar Dominan Global:** Mengidentifikasi polutan mana ($\text{PM}_{2.5}, \text{O}_3, \text{CO}$, dll.) yang memiliki **nilai ISPU rata-rata tertinggi** di seluruh wilayah, menetapkan target mitigasi utama.
* **Korelasi Polutan:** Matriks Korelasi digunakan untuk mengidentifikasi **sumber polusi bersama** (misalnya, korelasi tinggi antara $\text{CO}$ dan $\text{NO}_2$ sering berasal dari emisi kendaraan).

### 2. Pola Waktu (Temporal) (Bagian II)

* **Tren Musiman:** Analisis tren bulanan menunjukkan apakah ada **bulan atau musim tertentu** yang secara konsisten mengalami tingkat polusi yang lebih tinggi.
* **Pola Aktivitas Mingguan:** Analisis pola **Hari dalam Seminggu** menyoroti dampak aktivitas kerja/lalu lintas, seperti memburuknya kualitas udara pada hari kerja.

### 3. Hotspot Spasial (Lokasi) (Bagian III & IV)

* **Stasiun Terburuk:** Mengidentifikasi stasiun pemantauan yang mencatat **rata-rata ISPU tertinggi** (Hotspot umum).
* **Profil Polutan Spesifik:** Visualisasi mendalam memetakan rata-rata konsentrasi **setiap polutan** di stasiun, memungkinkan kebijakan yang ditargetkan berdasarkan jenis polutan per wilayah.

---

## ⚠️ Catatan Teknis

* **Kinerja Kode:** *Script* telah dioptimalkan untuk performa yang baik di Colab dan mencakup *error handling* untuk masalah *encoding* (mendukung `.xlsx` dan `.csv`).
* **Keterbatasan:** Analisis ini bersifat deskriptif, mengidentifikasi pola dan korelasi. Untuk memprediksi polusi atau menetapkan sebab-akibat yang kuat, diperlukan model statistik dan integrasi data tambahan (misalnya, resolusi per jam, data cuaca, atau lalu lintas).

***
