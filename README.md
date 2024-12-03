# ETL Batch Processing Project

## Deskripsi Proyek

Proyek ini adalah implementasi **ETL (Extract, Transform, Load)** sederhana untuk memindahkan data dari database produksi `marketplace` ke data warehouse `data_warehouse`. Proyek ini bertujuan untuk membuat tabel agregasi yang akan digunakan oleh tim data analyst untuk membuat dashboard tanpa membebani database produksi.

Tabel hasil migrasi akan berisi informasi detail terkait pesanan (order), pembayaran, pengiriman, voucher, dan rating yang dapat diolah lebih lanjut dalam visualisasi bisnis.

---

## Tujuan Proyek

1. Membuat pipeline ETL sederhana untuk migrasi data dari database produksi ke data warehouse.
2. Mengasah kemampuan menggunakan **Python**, **SQL**, dan **PostgreSQL** untuk batch processing data.
3. Menyediakan tabel yang siap digunakan untuk pembuatan dashboard oleh tim data analyst.

---

## Arsitektur Proyek

Pipeline ETL ini mencakup langkah berikut:

1. **Extract**: Mengambil data dari tabel produksi `tb_orders`, `tb_payments`, `tb_shippers`, `tb_vouchers`, dan `tb_ratings` dari database `marketplace`.
2. **Transform**: Membersihkan dan mempersiapkan data agar sesuai dengan kebutuhan tabel di data warehouse.
3. **Load**: Memasukkan data hasil transformasi ke tabel `dim_orders` di data warehouse `data_warehouse`.

---

## Tools yang Digunakan

- **Python (≥3.7)**  
  Digunakan untuk membuat pipeline ETL.
- **PostgreSQL**  
  Database source dan data warehouse.
- **pandas**  
  Untuk transformasi data di Python.
- **psycopg2**  
  Library untuk koneksi ke PostgreSQL.
- **SQLAlchemy**  
  Abstraksi query SQL menggunakan Python.
- **Git**  
  Untuk versi kontrol kode proyek.
- **DBeaver/PgAdmin**  
  GUI untuk memanage database PostgreSQL.
