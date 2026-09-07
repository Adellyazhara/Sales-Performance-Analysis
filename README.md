# Sales-Performance-Analysis🛒

## Background
Overview performa penjulan supermarket berdasarkan sales, product, customer, city, payment method, rating, dan time period.

## Data Overview
Dashboard menggunakan dataset transaksi penjualan supermarket yang berisikan 1.000 transaksi dengan informasi sebagai berikut:

## 📊 Struktur data
| **Kolom**              | **Deskripsi**                                        |
|------------------------|------------------------------------------------------|
| `Invoice ID`             | ID unik untuk setiap transaksi pesanan                     |
| `Branch`           | Cabang supermarket tempat transaksi dilakukan                    |
| `City`            | Kota tempat cabang supermarket berada                             |
| `Customer Type`            | Jenis pelanggan (Member atau Normal)                     |
| `Gender`          | Jenis kelamin pelanggan                                           |
| `Product Line`        | Kategori/jenis produk yang dibeli (Food and Beverages, Electronic Accessories, dan Fashion Accessories)                                                                    |
| `Unit Price`              | Harga satu unit produk                                    |
| `Quantity`              | Jumlah unit produk yang dibeli dalam satu transaksi         |
| `Tax 5%`                 | Pajak sebesar 5% yang dikenakan pada transaksi             |
| `Total`                | Total nilai transaksi setelah pajak                          |
| `Date`          | Tanggal transaksi dilakukan                                         |
| `Payment`               | Metode pembayaran yang digunakan (Cash, Credit Card, atau E-wallet) |
| `Cogs`           | Biaya perolehan barang yang terjual                                |
| `Gross Margin Percent`             | Persentase margin kotor dari transaksi           |
| `Gross Income`         | Pendapatan kotor yang diperoleh dari transaksi               |
| `Rating`         | Penilaian pelanggan terhadap pengalaman/produk setelah transaksi   |

## Contoh Data


## Business Questions❓
Pertanyaan bisnis yang yang dapat dijawab melalui analisis data penjualan supermarket:
1. Berapa total penjualan, jumlah produk yang terjual, gross income, dan rata-rata rating pelanggan yang dihasilkan?
2. Bagaimana tren penjualan dan jumlah produk terjual dari waktu ke waktu?
3. Product line apa yang dapat memberikan kontribusi penjualan (terbesar dan terendah)?
4. Bagaimana performa penjualan berdasarkan kota dan cabang?
5. Bagaimana perbandingan penjualan antara pelanggan Member dan Normal?
6. Metode pembayaran apa yang paling banyak digunakan oleh pelanggan?
7. Kota atau kelompok pelanggan mana yang memiliki tingkat kepuasan pelanggan tertinggi dan terendah?

## Methodology
Tools: Python dan Microsoft Excel
Berikut merupakan metode untuk analisis data penjualan:

### 1. Collection data
- Pengumpulan data penjualan diperoleh dari youtube dalam format excel. Data yang dikumpulkan berisi 1000 data transaksi yang mencakup informasi mengenai penjualan, pelanggan, dan produk yang dijual.

### 2. Cleaning
Proses pembersihandata dilakukan menggunakan Python untuk memastikan data yang digunakan memiliki kualitas yang baik dan siap untuk dilakukan analisis. Berikut langkah-langkah pembersihan data:
- Mengecek duplikat, baris data yang hilang, karakteristik setiap kolom
- Melakukan pengecekan terhadap data lengkap dan data yang memiliki informasi yang tidak lengkap (incomplete)
- Melakukan split data menjadi 2 bagian, yakni data complete dan data incomplete
- Data complete selanjutnya dilakukan analisis untuk mendapatkan informasi bisnis, sedangkan data incomplete dilakukan pengelompokan terhadap jenis ketidaklengkapan data (ringan, sedang, berat)

















