# Proyek Pertama : Menyelesaikan Permasalahan departemen Human Resources (HR)

## Bussines Understanding

#### Latar Belakang 

  Jaya Jaya Maju adalah perusahaan multinasional yang telah berdiri sejak tahun 2000 dan memiliki lebih dari 1.000 karyawan yang tersebar di seluruh penjuru Indonesia.  Seiring berkembangnya skala bisnis, kebutuhan terhadap manajemen sumber daya manusia yang efektif menjadi semakin penting.
  Meskipun memiliki skala operasi yang besar, Jaya Jaya Maju menghadapi tantangan dalam mengelola retensi karyawan. Salah satu indikator utama dari masalah ini adalah tingginya tingkat attrition atau tingkat pengunduran diri karyawan, yang telah melampaui 10%. Angka ini tergolong tinggi dan berpotensi menyebabkan masalah jangka panjang seperti meningkatnya biaya rekrutmen dan pelatihan, hilangnya pengetahuan institusional, serta penurunan produktivitas tim.
  Untuk mengatasi permasalahan ini, manajemen HR membutuhkan pendekatan berbasis data guna mengidentifikasi faktor-faktor utama penyebab attrition, serta alat bantu visual seperti dashboard untuk memantau kondisi tersebut secara real time. Oleh karena itu, proyek ini bertujuan untuk membantu perusahaan memahami dan memitigasi penyebab utama attrition melalui analisis data dan pengembangan dashboard bisnis yang informatif.

### Permasalahan Bisnis 

1. Tingginya tingkat attrition (>10%)
Hal ini dapat Mengakibatkan peningkatan biaya rekrutmen, pelatihan, serta kehilangan produktivitas dan pengetahuan organisasi.
2. Tidak jelasnya faktor utama penyebab attrition
Manajemen belum mengetahui secara pasti elemen apa (misal: lembur, usia, penghasilan, status pernikahan) yang paling berpengaruh terhadap keputusan karyawan untuk keluar.
3. Tidak adanya sistem pemantauan berbasis data
HR tidak memiliki alat untuk memantau dan menganalisis kondisi SDM secara real-time, sehingga sulit mengambil tindakan preventif.
4. Kekurangan insight untuk mendesain kebijakan retensi yang efektif
Misalnya: bagaimana mengatur kebijakan lembur, kompensasi, atau skema kerja fleksibel berdasarkan data.

### Cakupan proyek 
1. Eksplorasi dan permbersihan data
- Mengevaluasi kualitas data karyawan Jaya Jaya Maju.
- Membersihkan data dari nilai null, duplikat, atau outlier.
2. Analisis Pentingnya Fitur
- Memberikan interpretasi terhadap fitur-fitur yang paling berpengaruh terhadap attrition.
3. Pembuatan Bussines Dashboard Interaktif
- Menyusun dashboard dengan Google Looker Studio untuk menampilkan:
  - KPI seperti attrition rate, jumlah karyawan, rata-rata gaji
  - Visualisasi dari faktor utama penyebab attrition

### Pesiapan 
#### Sumber Data
Dataset yang digunakan dalam proyek ini adalah Dataset Karyawan Jaya Jaya Maju sesuai dengan instruksi dari submission proyek. Dataset tersebut tersedia dalam format CSV dan berisi informasi lengkap tentang demografi dan kondisi kerja karyawan, seperti: usia, pendapatan, status pernikahan, jarak rumah ke kantor, status lembur, dan lainnya.
- Jumlah data: 1.470 baris dan 35 kolom
- Sumber data: https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee

#### Setup Environment 
Proyek ini menggunakan environment yang sederhana dan dapat dijalankan sepenuhnya menggunakan tools berbasis cloud, tanpa instalasi lokal.
- Langkah - langkah :
1. Buka file notebook.ipynb menggunakan Google Colab
2. Jalankan seluruh sel untuk melakukan:
  - Eksplorasi data (EDA)
  - Pembersihan data
  - Visualisasi faktor-faktor yang berpengaruh terhadap attrition
3. Library yang digunakan meliputi:
  - pandas, numpy – manipulasi dan analisis data
  - matplotlib, seaborn – visualisasi data

#### Menjalankan Dashboard 
Untuk melihat dashboard secara interaktif:
- Gunakan Google Looker Studio
- Dashboard menampilkan KPI dan visualisasi attrition berdasarkan beberapa variabel penting (Overtime, Income, Age, dll)
- Tidak memerlukan setup tambahan atau instalasi software lokal
- Dapat diakses via browser secara langsung

## Bussines Dashboard 
Dashboard ini dirancang untuk membantu tim HR Jaya Jaya Maju dalam memantau, menganalisis, dan mengantisipasi faktor-faktor yang memengaruhi attrition (keluar/mundurnya karyawan). Dashboard dibangun menggunakan Google Looker Studio, sehingga dapat diakses dengan mudah secara online dan diperbarui secara real-time jika data berubah.

#### Fungsi Utama Dashboard 
- Memberikan gambaran menyeluruh tentang kondisi karyawan dan tingkat attrition perusahaan.
- Mengidentifikasi faktor-faktor yang paling berpengaruh terhadap keputusan karyawan untuk keluar, berdasarkan data historis.
- Memungkinkan tim HR melakukan analisis cepat dan mengambil tindakan preventif terhadap kelompok berisiko tinggi.

#### Komponen Utama dalam dashboard 
- KPI Utama	 : Menampilkan jumlah karyawan, jumlah yang keluar, attrition rate (16,92%), dan rata-rata pendapatan bulanan
- Attrition by Overtime	: Menunjukkan bahwa karyawan yang lembur memiliki tingkat attrition jauh lebih tinggi
- Attrition by Marital Status	 : Visualisasi pie chart: karyawan single menyumbang 52% dari total attrition
- Attrition by Job Role	: Tabel interaktif yang menunjukkan perbandingan attrition antar posisi (misalnya, Sales Representative memiliki angka tertinggi)
- Age vs Attrition	: Grafik distribusi umur dan kaitannya dengan risiko keluar
- Distance From Home	- Visualisasi hubungan jarak rumah-kantor dengan tingkat attrition
- Income vs Attrition:  pendapatan rata-rata antara karyawan yang bertahan vs. keluar


#### Link Akses Dashboard 
https://lookerstudio.google.com/reporting/e8664caf-ce83-42d5-a4d8-413154342d8d/page/RujNF

### Conclusion 
Faktor-Faktor yang mempengaruhi Attrion rate =
1. Overtime (Lembur)
Karyawan yang sering lembur memiliki kemungkinan 3–5 kali lebih tinggi untuk mengalami attrition dibanding yang tidak lembur. Ini menunjukkan bahwa beban kerja berlebih dapat berdampak negatif terhadap kepuasan dan keseimbangan hidup.

2. Monthly Income (Gaji Bulanan) Karyawan dengan pendapatan lebih rendah cenderung lebih tinggi tingkat attrition-nya. Ketidakpuasan terhadap kompensasi menjadi faktor penting dalam keputusan untuk keluar.

3. Age (Usia)
Karyawan lebih muda (terutama di bawah 30 tahun) memiliki tingkat attrition lebih tinggi. Mereka cenderung lebih mobile secara karier dan mencari peluang yang lebih sesuai dengan aspirasi mereka.

4. Marital Status (Status Pernikahan)  Karyawan yang belum menikah (single) memiliki kecenderungan lebih tinggi untuk keluar. Mereka cenderung lebih fleksibel dan memiliki komitmen yang lebih rendah terhadap organisasi jangka panjang.

5. Travel Frequency (Frekuensi Perjalanan Dinas)
Karyawan yang sering melakukan perjalanan bisnis menunjukkan tingkat attrition yang lebih tinggi, kemungkinan karena kelelahan, stress, dan work-life imbalance.

6. DistanceFromHome (Jarak dari rumah ke kantor)
Karyawan yang tinggal lebih jauh dari kantor memiliki kemungkinan lebih tinggi untuk keluar, yang menunjukkan bahwa jarak tempuh harian dapat menjadi beban tambahan yang berpengaruh terhadap retensi.

## Rekomendasi 
1. Terapkan Program Manajemen Beban Kerja & Work-Life Balance
- Batasi lembur dengan kebijakan tegas dan pantauan berkala.
- Sediakan opsi kerja fleksibel (remote/hybrid).
- Promosikan budaya kerja sehat dengan jam kerja yang wajar.

2. Evaluasi dan Penyesuaian Skema Kompensasi
- Lakukan benchmarking gaji secara berkala.
- Buat insentif tambahan untuk karyawan dengan performa tinggi/Lembur.
- Tawarkan benefit non-finansial seperti cuti tambahan, pelatihan karier, atau program kesejahteraan.

3. Bangun Strategi Retensi Karyawan Muda dan Single
- Sediakan jalur karier yang jelas dan cepat untuk karyawan muda.
- Berikan kesempatan belajar dan berkembang (misalnya sertifikasi, pelatihan).
- Perkuat engagement melalui mentoring dan komunitas internal.

4. Kelola Beban Perjalanan Bisnis
- Evaluasi ulang kebutuhan perjalanan dinas yang berlebihan.
- Berikan kompensasi khusus atau fleksibilitas waktu bagi karyawan yang sering dinas.
- Gunakan alternatif digital seperti video conference bila memungkinkan.

5. Dukungan Transportasi dan Lokasi
- Sediakan fasilitas antar-jemput atau subsidi transportasi untuk karyawan yang tinggal jauh.
- Pertimbangkan kebijakan kerja hybrid untuk mengurangi waktu perjalanan.
- Petakan sebaran tempat tinggal karyawan untuk merancang solusi transportasi yang efisien.
