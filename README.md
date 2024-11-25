# Machine Learning Untuk Klasifikasi Pesan Spam Bahasa Indonesia Menggunakan Algoritma Naïve Bayes (TF-IDF)

## Deskripsi Project
Proyek ini bertujuan untuk mengembangkan model klasifikasi teks yang dapat membedakan pesan normal/spam/promo menggunakan teknik pemrosesan teks (NLP) dan algoritma Machine Learning. Solusi ini dirancang untuk membantu pengguna menyaring pesan yang tidak relevan dan meningkatkan efisiensi komunikasi.

## Workflow Project
- Business Understanding: Pemahaman terkait masalah, identifikasi tujuan, dan metriks evaluasi
- Data Understanding: Pemahaman terkait karakteristik dan kebutuhan dari data
- Preprocessing Data Teks: Membersihkan dan mempersiapkan data teks mentah untuk pemrosesan.
- Representasi Data: 
  - TF-IDF: Menghitung bobot kata berdasarkan frekuensi di seluruh dokumen.
  - Word2Vec: Representasi vektor berbasis konteks untuk setiap kata.
- Klasifikasi: Mengimplementasikan algoritma Machine Learning seperti Naive Bayes dan Logistic Regression.
- Evaluasi Model: Menggunakan metrik precision, recall, dan F1-score untuk menilai performa model.
- Testing model: Testing final model (Naive Bayes (TF-IDF)) dengan data baru tanpa label.

## Dataset
Dataset yang digunakan mencakup pesan teks pendek dengan label spam atau ham. Dataset ini dapat berasal dari sumber terbuka seperti [Dataset SMS Spam Indonesia](https://www.kaggle.com/datasets/bobsteward/dataset-sms-spam-indonesia).
<br>**Struktur Dataset**:</br>
- `text`: Konten pesan.
- `label`: Kategori pesan ( 0 : `Normal` , 1 :`Spam` , 2 : `ham`).

## **Pendekatan dan Teknik**
1. **Preprocessing Data Teks**:
   - Mengubah teks menjadi huruf kecil (*lowercasing*).
   - Menghapus simbol, angka, dan tanda baca yang tidak relevan.
   - Menghapus *stopwords* untuk menyederhanakan teks.
   - Melakukan *stemming* atau *lemmatization* untuk menyederhanakan bentuk kata.

2. **Feature Engineering**:
   - **TF-IDF**:
     - Menggunakan *TfidfVectorizer* untuk menghitung bobot kata berdasarkan frekuensi kata di seluruh dokumen.
   - **Word2Vec**:
     - Menggunakan *Word Embedding* dengan bantuan library *Gensim* untuk merepresentasikan kata dalam bentuk vektor numerik.

3. **Modeling**:
   - Algoritma yang digunakan:
     - **Naive Bayes**: Untuk klasifikasi teks dengan efisiensi tinggi.
     - **Logistic Regression**: Untuk memprediksi probabilitas pesan sebagai normal/spam/promo.

4. **Evaluasi Model**:
   - Metrik evaluasi yang digunakan:
     - Accuracy
     - Precision
     - Recall
     - F1-Score
   - Visualisasi hasil evaluasi menggunakan *Confusion Matrix*.

---

## **Hasil**
- **Model Terbaik**: Naive Bayes dengan representasi TF-IDF.
- **Evaluasi Model**:
## **Evaluasi Model**
| **Class**       | **Precision** | **Recall** | **F1-Score** | **Support** |
|------------------|--------------|------------|--------------|-------------|
| 0                | **0.97**     | 0.91       | 0.94         | 132         |
| 1                | **0.91**     | 0.94       | 0.92         | 94          |
| 2                | **0.86**     | 0.93       | 0.90         | 60          |
| **Accuracy**     | -            | -          | **0.92**     | **286**     |
| **Macro Avg**    | 0.91         | 0.93       | 0.92         | 286         |
| **Weighted Avg** | 0.93         | 0.92       | 0.92         | 286         |

---

## **Pengembangan Selanjutnya**
- Eksperimen lebih lanjut menggunakan model berbasis *Deep Learning* seperti RNN atau Transformer (BERT).
- Mengintegrasikan model ke dalam aplikasi berbasis web atau API untuk pengelolaan pesan secara real-time.
- Memperluas dataset untuk meningkatkan kemampuan generalisasi model.

---

Copyright (c) [2024] [Zaima .S Asshafa].

---

## **Kontributor**
- **Zaima .S Asshafa** - [GitHub](https://github.com/ZaimaSyarifaAsshafa) | [LinkedIn](www.linkedin.com/in/zaimasyarifaasshafa)
