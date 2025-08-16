# Analisis Sentimen Publik Terhadap Danantara Menggunakan IBM Granite

## 📜 Gambaran Umum Proyek (Project Overview)

Proyek ini bertujuan untuk menganalisis dan mengklasifikasikan sentimen masyarakat Indonesia terhadap **Danantara**, sebuah lembaga Pengelola Investasi (LPI) yang dibentuk oleh pemerintah Indonesia. Dengan memanfaatkan kemampuan *Natural Language Processing* (NLP) dari model AI **IBM Granite**, proyek ini menggali persepsi, kekhawatiran, dan harapan publik yang tercermin dalam percakapan di platform media sosial X (sebelumnya Twitter).

Analisis dilakukan pada kumpulan data tweet publik dari periode **Januari - Maret 2025** untuk mengidentifikasi sentimen dominan dan tema-tema kunci yang mendasarinya. Hasil dari analisis ini kemudian digunakan untuk merumuskan kesimpulan dan rekomendasi strategis yang dapat ditindaklanjuti bagi para pemangku kepentingan.

## 💾 Dataset

Dataset yang digunakan dalam proyek ini adalah `data_clean_danantara.csv`, yang berisi kumpulan tweet publik mengenai Danantara.

- **Sumber:** Platform X (Twitter)
- **Periode:** Januari - Maret 2025
- **Link Dataset:** `[Masukkan link langsung ke file data_clean_danantara.csv di repositori GitHub Anda di sini]`

## 🛠️ Tools dan Library

- **Bahasa Pemrograman:** Python
- **Lingkungan Kerja:** Google Colab
- **Library Utama:**
    - `Pandas`: Untuk manipulasi dan analisis data.
    - `Matplotlib` & `Seaborn`: Untuk visualisasi data.
    - `LangChain` & `Replicate`: Untuk berinteraksi dengan API model AI.
- **Model AI:** `ibm/granite-13b-instruct`

## ⚙️ Proses Analisis

Proses analisis dalam proyek ini mengikuti langkah-langkah berikut:
1.  **Setup Lingkungan:** Menginstal library yang dibutuhkan dan mengkonfigurasi API *key* untuk mengakses model IBM Granite.
2.  **Memuat Data:** Mengimpor dataset tweet dari file CSV ke dalam DataFrame Pandas.
3.  **Rekayasa *Prompt* (Prompt Engineering):** Merancang *prompt* yang efektif untuk menginstruksikan model AI agar mengklasifikasikan setiap tweet ke dalam kategori sentimen (Positif, Negatif, Netral) dan memberikan alasan singkat di balik klasifikasinya.
4.  **Aplikasi Model AI:** Menerapkan fungsi klasifikasi pada seluruh dataset untuk menghasilkan analisis sentimen untuk setiap tweet.
5.  **Parsing & Strukturisasi Hasil:** Mengurai hasil teks dari model AI dan memisahkannya ke dalam kolom-kolom terstruktur (`Sentimen` dan `Alasan`) untuk analisis lebih lanjut.
6.  **Analisis & Visualisasi:** Melakukan analisis kuantitatif untuk menghitung distribusi sentimen dan membuat visualisasi data (diagram batang) untuk menyajikan temuan secara efektif.
7.  **Penarikan Kesimpulan:** Merumuskan *insight*, kesimpulan, dan rekomendasi berdasarkan hasil analisis data.

## 📊 Temuan Utama (*Insight* & Findings)

Analisis terhadap **`[Isi dengan jumlah total tweet]`** tweet menghasilkan temuan-temuan kunci berikut:

- **Sentimen Dominan:** Sentimen publik terhadap Danantara didominasi oleh sentimen **`[Isi dengan sentimen mayoritas, misal: Negatif]`**, yang mencakup **`[Isi dengan persentase mayoritas]%`** dari total data.
- **Distribusi Sentimen:** Sentimen Positif tercatat sebesar **`[Isi persentase positif]%`**, sementara **`[Isi persentase netral]%`** sisanya bersifat Netral.
- **Pemicu Sentimen Negatif:** Analisis kualitatif menunjukkan bahwa kekhawatiran utama publik berpusat pada isu **`[Sebutkan 1-2 tema utama negatif, misal: transparansi tata kelola dan potensi penyalahgunaan dana/korupsi]`**.
- **Pendorong Sentimen Positif:** Di sisi lain, optimisme publik didorong oleh harapan terhadap **`[Sebutkan 1-2 tema utama positif, misal: percepatan pertumbuhan ekonomi dan pendanaan proyek strategis nasional]`**.

## 🤖 Penjelasan Dukungan AI (AI Support Explanation)

Proyek ini memanfaatkan model *Large Language Model* (LLM) **IBM Granite (`granite-13b-instruct`)** sebagai mesin utama untuk klasifikasi sentimen. Peran AI dalam proyek ini adalah sebagai berikut:
- **Klasifikasi Kontekstual:** Model AI tidak hanya mengklasifikasikan sentimen berdasarkan kata kunci, tetapi juga memahami konteks dan nuansa dalam setiap tweet untuk menentukan apakah sentimennya Positif, Negatif, atau Netral.
- **Ekstraksi Alasan:** Melalui *prompt* yang dirancang khusus, model diinstruksikan untuk memberikan justifikasi atau alasan atas klasifikasinya. Kemampuan ini memungkinkan analisis kualitatif yang lebih dalam untuk memahami "mengapa" di balik setiap sentimen, yang merupakan inti dari temuan proyek ini.

## 🚀 Kesimpulan dan Rekomendasi

### Kesimpulan
Persepsi publik terhadap Danantara cenderung **`[Sebutkan sentimen dominan]`** dan terpolarisasi. Terdapat kesenjangan yang signifikan antara tujuan strategis pemerintah dalam membentuk Danantara dengan persepsi risiko (terutama terkait tata kelola) yang ditangkap oleh masyarakat luas.

### Rekomendasi
1.  **Tingkatkan Transparansi Proaktif:** Danantara direkomendasikan untuk mengembangkan **portal transparansi publik** guna menyajikan laporan alur investasi dan mekanisme pengawasan secara berkala untuk menjawab kekhawatiran utama publik.
2.  **Perkuat Narasi Dampak Positif:** Tim komunikasi pemerintah disarankan untuk mengamplifikasi narasi tentang **dampak nyata Danantara** bagi masyarakat, seperti studi kasus penciptaan lapangan kerja dari proyek yang didanai, untuk menyeimbangkan narasi negatif yang ada.
