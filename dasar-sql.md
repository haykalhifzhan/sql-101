# 📚 Apa Itu SQL?

**SQL (Structured Query Language)** adalah bahasa khusus yang digunakan untuk **mengelola dan mengolah data** dalam sistem **database relasional**.

> Gampangnya, SQL itu kayak bahasa komunikasi antara kita (manusia) dengan database. Kita bisa:  
> - 📥 Memasukkan data  
> - 📤 Mengambil data  
> - ✏️ Mengubah data  
> - 🗑️ Menghapus data

---

## 🧱 Apa Itu Database Relasional?

Database relasional menyimpan data dalam bentuk **tabel** mirip seperti Excel atau Google Sheets.  
Setiap **tabel** terdiri dari:

- **Baris (row)** 👉 mewakili satu data/entri  
- **Kolom (column)** 👉 jenis informasinya (nama, umur, dll)

Contoh tabel:

| id | nama   | umur |
|----|--------|------|
| 1  | Andi   | 25   |
| 2  | Budi   | 30   |

➡️ Di atas ada:
- **2 baris data** → Andi dan Budi  
- **3 kolom** → id, nama, umur

---

## 🔧 Apa yang Bisa Kita Lakukan dengan SQL?

Beberapa perintah dasar SQL yang sering digunakan:

| Perintah | Fungsi                                           |
|----------|--------------------------------------------------|
| `SELECT` | Mengambil data dari tabel                        |
| `INSERT` | Menambahkan data baru ke tabel                   |
| `UPDATE` | Mengubah data yang sudah ada                     |
| `DELETE` | Menghapus data dari tabel                        |

---

## 🚀 Contoh Penggunaan

```sql
-- Ambil semua data dari tabel "pengguna"
SELECT * FROM pengguna;
