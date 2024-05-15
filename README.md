# Sampling Method 

## Deskripsi
Proyek ini bertujuan untuk mengatasi masalah data tidak seimbang dengan menerapkan berbagai teknik sampling menggunakan pustaka `imbalanced-learn`. Data tidak seimbang terjadi ketika distribusi kelas dalam sebuah dataset tidak seimbang, yang menyebabkan kinerja model machine learning menjadi buruk, terutama dalam kasus di mana kelas minoritas menjadi fokus perhatian.

## Teknik Sampling
Berikut ini adalah teknik sampling yang diimplementasikan dalam proyek ini:

- **Random Over-Sampling**: Teknik ini secara acak menduplikasi instance dari kelas minoritas untuk menyeimbangkan distribusi kelas.
- **SMOTE (Synthetic Minority Over-sampling Technique) Tomek Links**: Teknik ini menggabungkan over-sampling menggunakan SMOTE dan under-sampling menggunakan Tomek links untuk menciptakan instance sintetis dari kelas minoritas sambil menghapus instance yang bising dan borderline.
- **ADASYN (Adaptive Synthetic Sampling)**: Teknik ini menghasilkan instance sintetis dari kelas minoritas dengan distribusi densitas berdasarkan densitas lokal dari instance minoritas.
- **Random Under-Sampling**: Teknik ini secara acak menghapus instance dari kelas mayoritas untuk menyeimbangkan distribusi kelas.
- **NearMiss**: Teknik ini memilih instance kelas mayoritas yang paling dekat dengan instance kelas minoritas berdasarkan metrik jarak untuk melakukan under-sampling pada kelas mayoritas.
- **Cluster Centroids**: Teknik ini melakukan under-sampling pada kelas mayoritas dengan mengelompokkan instance kelas mayoritas dan memilih centroid klaster sebagai perwakilan.
