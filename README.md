# Data Visualization: Pola Pemilihan Mata Kuliah Mahasiswa

- **Nama :Yohanes Tiyas Prasetiyo
- NIM    :2318125
  
## Dataset
- **File:** `data/clean_data_anonim.csv`
- **Ukuran:** 100 mahasiswa, 16 kolom, tanpa missing value dan tanpa duplikat
- **Isi:** 9 kolom biner pilihan mata kuliah (1 = dipilih), `jumlah_pilihan`, `kategori_beban` (Ringan 1-3, Sedang 4-5, Tinggi 6-9), dan 4 kolom jumlah pilihan per rumpun keilmuan

## Tujuan
Mengeksplorasi mata kuliah yang diminati, sebaran beban pilihan, dominasi rumpun keilmuan, dan keterkaitan antar mata kuliah.

## Teknik Visualisasi
Bar chart, histogram, boxplot, heatmap (korelasi, co-occurrence, profil per kategori), stacked bar, dan grafik interaktif Plotly. Line chart tidak dipakai karena data tidak memiliki dimensi waktu.

## Insight Utama
1. Pemrograman CMS (94%) dan Realitas Virtual (87%) paling diminati; Sistem Informasi Pendidikan hanya 10%.
2. Rata-rata mahasiswa memilih 4,79 mata kuliah; 67% berada di kategori Sedang (4-5).
3. Multimedia dan Visual rumpun terbesar (249 pilihan), tetapi per mata kuliah Pengembangan Web paling kuat.
4. Korelasi antar mata kuliah lemah (|r| < 0,3): pilihan hampir independen.
5. Data Mining naik dari 20% (beban Ringan) ke 96% (beban Tinggi): menjadi pilihan tambahan bagi mahasiswa dengan beban besar.

## Hasil Visualisasi
![Popularitas](images/01_popularitas_matkul.png)
![Histogram](images/02_histogram_jumlah_pilihan.png)
![Rumpun](images/04_rumpun_keilmuan.png)
![Korelasi](images/06_heatmap_korelasi.png)
![Profil](images/08_profil_per_beban.png)

## Cara Menjalankan
1. Buka notebook di Google Colab (atau Jupyter lokal).
2. Upload `data/clean_data_anonim.csv`, ubah namanya menjadi `clean_data.csv` (atau ubah path di sel load data).
3. Jalankan semua sel (`Runtime > Run all`).

Library: pandas, numpy, matplotlib, seaborn, plotly.
```
