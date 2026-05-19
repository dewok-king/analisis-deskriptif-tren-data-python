# Analisis Deskriptif dan Tren Data Penjualan

## Deskripsi Project
Project ini merupakan tugas mata kuliah Data Infrastructure and Analytics mengenai analisis deskriptif dan analisis tren data menggunakan Python pada Google Colab.

Dataset yang digunakan adalah dataset Superstore yang berisi data penjualan, profit, kategori produk, dan tanggal transaksi.

Analisis dilakukan untuk:
- Mengetahui statistik deskriptif data Sales dan Profit
- Menganalisis performa per kategori produk
- Melihat tren penjualan dan profit dari waktu ke waktu
- Membuat visualisasi data menggunakan Python

---

## Tools dan Library
- Python
- Google Colab
- Pandas
- Matplotlib
- Seaborn

---

## Dataset
Dataset menggunakan Sample Superstore Dataset.

---

## Analisis yang Dilakukan

 Statistik Deskriptif
Analisis dilakukan menggunakan fungsi:
```python
df[['Sales','Profit']].describe()

df.groupby("Category")[["Sales","Profit"]].agg(["mean","sum","count"])

sns.boxplot(x=df["Sales"])

