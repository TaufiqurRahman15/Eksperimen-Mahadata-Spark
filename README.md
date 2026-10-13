# Eksperimen-Mahadata-Spark
Tugas Individu Mahadata - Benchmark Partisi Apache Spark

**Nama:** Taufiqur Rahman  
**NIM:** 123140007  
**Mata Kuliah:** Mahadata  

## Deskripsi Proyek
Eksperimen ini bertujuan untuk mengukur dan menganalisis pengaruh jumlah partisi data (*repartition*) pada Apache Spark terhadap waktu eksekusi proses agregasi data menggunakan dataset **Online Retail** (541.909 baris).

## Ringkasan Hasil Eksperimen
- **1 Partisi:** Rata-rata 2,387 detik (Tercepat)
- **2 Partisi:** Rata-rata 3,104 detik
- **4 Partisi:** Rata-rata 2,444 detik
- **8 Partisi:** Rata-rata 3,882 detik (Terlama)

## Kesimpulan
Pada lingkungan *single-node* (Google Colab), penambahan jumlah partisi yang terlalu banyak justru meningkatkan waktu eksekusi karena adanya *overhead* manajemen partisi dan *data shuffling*.
