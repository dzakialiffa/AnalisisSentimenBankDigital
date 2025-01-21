# Analisis Sentimen Bank Digital

## Deskripsi Proyek
Proyek ini bertujuan untuk melakukan analisis sentimen terhadap tiga aplikasi bank digital populer: Seabank, Bank Jago, dan Blu BCA. Dengan memanfaatkan model **BERT**, kami menganalisis ulasan pengguna untuk memahami sentimen mereka (positif, negatif, atau netral) dan memberikan rekomendasi untuk pengembangan layanan aplikasi tersebut.

## Hasil Penelitian
### **1. Seabank**
- **Hasil Analisis**:
  - Akurasi model: **90%**.
  - Sentimen positif dominan (58,5%) dengan kata-kata utama seperti *bagus*, *cepat*, *gratis*, dan *senang*.
  - Keluhan negatif (41,5%) sering terkait dengan pinjaman, kecewa, dan masalah minor lainnya.
- **Rekomendasi Pengembangan**:
  - Peningkatan layanan pelanggan untuk respons cepat terhadap keluhan.
  - Pengembangan fitur tambahan, seperti edukasi keuangan.
  - Pengoptimalan performa aplikasi agar tetap ringan dan stabil.

### **2. Bank Jago**
- **Hasil Analisis**:
  - Akurasi model: **91%**.
  - Sentimen positif (52,1%) menonjol pada aspek seperti *membantu*, *cepat*, dan *aman*.
  - Sentimen negatif (47,9%) didominasi oleh keluhan prosedur yang ribet, kegagalan transaksi, dan kendala login.
- **Rekomendasi Pengembangan**:
  - Simplifikasi proses penggunaan untuk kemudahan pengguna.
  - Penguatan sistem keamanan.
  - Optimalisasi performa aplikasi untuk mengatasi keluhan login.

### **3. Blu BCA**
- **Hasil Analisis**:
  - Akurasi model: **88%**.
  - Sentimen positif (50,4%) terkait dengan kata-kata seperti *bagus*, *mudah*, *cepat*, dan *oke*.
  - Sentimen negatif (40,6%) sering menyebutkan keluhan seperti *lambat*, *berat*, dan *lemot*.
- **Rekomendasi Pengembangan**:
  - Pengurangan biaya administrasi untuk menarik pengguna baru.
  - Optimalisasi performa aplikasi agar lebih stabil.
  - Peningkatan fitur layanan transaksi agar lebih cepat dan mudah digunakan.

### **Kesimpulan Umum**
Model **BERT** menunjukkan akurasi tinggi dalam analisis sentimen terhadap tiga aplikasi bank digital. Hasil penelitian menyoroti pentingnya pengembangan layanan yang lebih berorientasi pada pengguna, penyederhanaan proses, dan optimalisasi aplikasi untuk meningkatkan kepuasan pengguna.

## Struktur Proyek
- **Data**: Dataset ulasan pengguna dari ketiga aplikasi bank digital.
- **Model**: Implementasi model BERT untuk analisis sentimen.
- **Analisis**: Hasil analisis sentimen dan visualisasi data.
- **Rekomendasi**: Rekomendasi berdasarkan hasil analisis untuk masing-masing aplikasi.

## Teknologi yang Digunakan
- **Python**: Bahasa pemrograman utama.
- **BERT**: Model pembelajaran mesin untuk analisis sentimen.
- **Pandas & NumPy**: Pengolahan data.
- **Matplotlib & Seaborn**: Visualisasi data.

## Cara Menggunakan
1. Clone repositori ini:
   ```bash
   git clone https://github.com/dzakialiffa/AnalisisSentimenBankDigital.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Jalankan skrip analisis:
   ```bash
   python main.py
   ```

## Kontribusi
Kami sangat terbuka terhadap kontribusi untuk pengembangan proyek ini lebih lanjut. Silakan buat pull request atau buka issue jika ada saran atau perbaikan.

## Lisensi
Proyek ini dilisensikan di bawah [MIT License](LICENSE).

---

### Kontak
Jika ada pertanyaan atau masukan, jangan ragu untuk menghubungi:
- **Email**: dzakialifa.work@gmail.com
- **GitHub**: [dzakialiffa](https://github.com/dzakialiffa)
