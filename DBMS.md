# 🏗️ Dasar DBMS (Database Management System)

## 📦 Apa Itu DBMS?

**DBMS (Database Management System)** adalah software yang digunakan untuk menyimpan, mengatur, dan mengelola data dalam sebuah database.

Contoh DBMS yang populer:
- MySQL / MariaDB
- PostgreSQL
- SQLite
- SQL Server
- Oracle DB

---

## 🗃️ Database dan Tabel

Di dalam sebuah **database**, terdapat banyak **tabel**.  
Misalnya, di database bernama `myshop`, kita bisa punya tabel seperti:

- `users` → menyimpan data pengguna
- `products` → menyimpan data barang
- `stocks` → menyimpan data stok barang

---

## 🧾 Ilustrasi Tabel dalam Database

Bayangkan tabel itu seperti lembaran di spreadsheet (Excel / Google Sheets), yang punya **baris** dan **kolom**.

Contoh tabel `products`:

| Produk | Harga |
|--------|-------|
| P1     | 2000  |
| P2     | 4000  |

Keterangan:
- **Setiap kolom** menunjukkan tipe informasi (Produk, Harga).
- **Setiap baris** berisi data satu produk.

---

## 🔄 Hubungan Antartabel

Tiap tabel biasanya **terhubung satu sama lain**.  
Contoh:
- Tabel `products` punya data barang
- Tabel `stocks` bisa menunjuk ke `products` lewat **product_id**

Inilah mengapa disebut **database relasional** — karena antar tabel **saling berelasi**.

---

## 📌 Kesimpulan

- DBMS = software pengelola database
- Database = tempat menyimpan data
- Tabel = struktur penyimpan data dalam bentuk baris & kolom
- SQL = bahasa untuk berinteraksi dengan DBMS
