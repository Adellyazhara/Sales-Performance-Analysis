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
1. Bagaimana performa penjualan supermarket secara keseluruhan berdasarkan total penjualan, jumlah produk terjual, dan nilai penjualan setelah pajak?
2. Bagaimana tren penjualan dan jumlah produk terjual selama periode transaksi?
3. Product line mana yang memberikan kontribusi terbesar terhadap penjualan dan jumlah produk terjual?
4. Bagaimana tingkat kepuasan pelanggan berdasarkan rata-rata rating di setiap kota?
5. Bagaimana preferensi pelanggan berdasarkan customer type dan metode pembayaran yang digunakan?

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

## 3. Exploratory Data Analysis (EDA)
Tahap ini dilakukan untuk memperoleh informasi awal mengeneai distribusi dan pola data dengan teknik seperti:
- **Analisis Deskriptif:** Menganalisis performa penjualan berdasarkan product line, cabang, dan customer type
- **Trend Analisis:** Menganalisis tren penjualan dan gross income berdasarkan waktu
- **Pivot Table:** Membuat tabel pivot untuk merangkum sales, quantity, dan gross income berdasarkan bproduct line, city, customer type, dan payment method untuk mempermudal perbandingan performa antar dimensi
- **Product Line Analysis:** Membandingkan performa dan kontribusi masing-masing kategori produk
- **Analisis Profitabilitas:** Membandingkan gross income dan gross margin antar product line dan cabang

## 4. Visualisasi Data
Berikut merupakan dashboard visualisasi dari data penjualan swalayan yang telah dianalisis.
![Sales Dashboard](https://github.com/Adellyazhara/Sales-Performance-Analysis/blob/main/Dashboard?raw=true)

## Insight 💡
Beberapa informasi yang diperoleh dari analisis data pejualan supermarket:
**1. Performa penjualan supermarket secara keseluruhan**
- Total penjualan menghasilkan $322,967k selama periode transaksi dengan produk terjual mencappai 5.510 unit
- Setelah memperhitungkan pajak, nilai penjualan mencapai $307,587k
Hasil tersebut menunjukkan bahwa supermarket memiliki volume transaksi dan penjualan yang cukup tinggi selama periode pengamatan
**2. Tren penjualan dan jumlah produk terjual**
- Penjualan menunjukkan peningkatan dari Februari ke Maret dari $63,170k menjadi $72,749k
- Pada April, penjualan mengalami penurunan menjadi 7,958k
- Pola jumlah produk terjual juga menunjukkan adanya fluktuasi antarbulan, sehingga periode Maret menjadi periode dengan performa penjualan paling tinggi. Fluktuasi tersebut menunjukkan bahwa performa penjualan belum sepenuhnya konsisten dari bulan ke bulan
**3. Kontribusi product line terhadap penjualan dan jumlah produk terjual**
- Food and baverages menjadi poruct line dengan kontribusi penjualan terbesar dengan total penjualan $56,145k, disusul dengan Sport and travel dengan total penjualan $53,123k
- Sementara itu, Health and beauty memiliki kontribusi penjualan paling rendah dengan total penjualan $49,194k
- Perbedaan tersebut menunjukkan bahwa kontribusi terhadap penjualan tidak tersebar secara merata di seluruh product line
**4. Tingkat kepuasan pelanggan berdasarkan kota**
- Naypyitaw memiliki rata-rata rating pelanggan tertinggi sebesar 7.07, sementara Mandalay memiliki rata-rata terendah sebesai 6.81
- Perbedaan tingkat kepuasan pelanggan antar kota dapat menjadi salah satu aspek yang perlu dievaluasi pada masing-masing lokasi
**5. Preferensi pelanggan berdasarkan customer type & metode pembayaran**
- Metode pembayaran, E-wallet menjadi metode yang paling banyak digunakan, yaitu sekitar 35% transaksi

## Reccomendation
1. Perusahaan perlu mempertahankan performa penjualan dengan memastikan ketersediaan stok produk dan memantau perubahan jumlah produk terjual secara berkala. Product line dengan kontribusi tinggi juga dapat dijadikan prioritas dalam pengelolaan stok dan strategi penjualan.
2. Penurunan penjualan setelah periode Maret perlu dievaluasi dengan membandingkan jumlah transaksi, jumlah produk terjual, product line, dan aktivitas promosi antarbulan. Hasil evaluasi dapat digunakan untuk menentukan strategi yang dapat menjaga kestabilan penjualan.
3. Food and Beverages memiliki kontribusi penjualan tertinggi sehingga dapat dipertahankan melalui ketersediaan stok dan promosi yang sesuai. Sementara itu, Health and Beauty yang memiliki kontribusi terendah perlu dievaluasi dan dapat didorong melalui bundling, promosi, atau penawaran khusus.
4. Karena terdapat perbedaan rata-rata rating antar kota, perusahaan dapat mengevaluasi kualitas pelayanan, ketersediaan produk, dan pengalaman pelanggan terutama pada kota dengan rating lebih rendah seperti Mandalay.
5. Karena E-wallet menjadi metode pembayaran yang paling banyak digunakan, perusahaan dapat mempertahankan kemudahan pembayaran digital dan mempertimbangkan promo atau loyalty program berbasis E-wallet untuk meningkatkan transaksi dan mempertahankan pelanggan.

## Conclusion
Secara keseluruhan, perusahaan perlu mempertahankan product line dengan performa tinggi, meningkatkan strategi untuk kategori dengan kontribusi rendah, mengevaluasi penyebab fluktuasi penjualan, serta meningkatkan customer experience pada lokasi dengan rating lebih rendah. Preferensi pembayaran digital juga dapat dimanfaatkan sebagai bagian dari strategi promosi dan customer retention.





























