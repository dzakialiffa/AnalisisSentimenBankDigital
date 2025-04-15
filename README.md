# 🧠 Sentiment Analysis: Digital Bank (Seabank)

Analisis sentimen terhadap ulasan pengguna bank digital menggunakan model pre-trained **IndoBERT**. Proyek ini mencakup preprocessing data, fine-tuning model, evaluasi, prediksi, dan visualisasi hasil.

---

## 📁 Struktur Proyek

### 1. 🔧 Persiapan Lingkungan
- Mount Google Drive agar dapat mengakses dataset dan menyimpan model.
- Install dan import library:
  - `transformers`
  - `pandas`
  - `numpy`
  - `sklearn`
  - `matplotlib`
  - `seaborn`

### 2. 📥 Load Dataset
- Dataset diload dari Google Drive menggunakan `pandas`.
- Format: `.csv` atau `.xlsx`
- Kolom: `text` (ulasan) dan `label` (sentimen)

### 3. 🧹 Preprocessing Data
- **Clean text**: hapus URL, angka, karakter khusus, dan ubah huruf menjadi lowercase.
- **Encoding label**: mengubah label (positif/negatif) ke bentuk numerik.

### 4. ✂️ Train-Test Split
- Membagi data ke dalam set pelatihan dan pengujian menggunakan `train_test_split`.

### 5. 🧾 Tokenisasi
- Menggunakan tokenizer IndoBERT (`indobenchmark/indobert-base-p1`) dari `transformers`.
- Format input: `input_ids`, `attention_mask`.

### 6. 🧠 Fine-Tuning Model
- Model: `BertForSequenceClassification` dari HuggingFace.
- Konfigurasi:
  - Epochs: 10
  - Batch size: 32
  - Learning rate: 2e-5
- Menggunakan API `Trainer` dari Huggingface.

### 7. 📊 Evaluasi Model
- Metrik evaluasi:
  - Accuracy
  - Confusion Matrix
  - Classification Report
- Visualisasi:
  - Kurva akurasi dan loss
  - Confusion matrix

### 8. 🔍 Prediksi Sentimen
- Fungsi prediksi terhadap teks baru:
```python
input_text = "Aplikasi ini sangat membantu!"
predict_sentiment(input_text)  # Output: "Positif"
