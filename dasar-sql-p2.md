# ⚙️ Perintah SQL & Cara Kerjanya dalam Sistem Database

## 📌 SQL Itu Bahasa Apa Sih?

**SQL (Structured Query Language)** adalah **bahasa teks** yang digunakan untuk ngobrol sama database.

- Gampang dipakai untuk hal sederhana, seperti ambil data dari tabel.
- Tapi juga bisa sangat kompleks, misalnya buat analisis data, trigger otomatis, atau mengelola relasi antar tabel.

Meskipun banyak **tool visual (GUI)** buat lihat database, penting banget buat tetap **paham perintah SQL secara manual**.

Kenapa?

> Karena **SQL Injection** terjadi justru saat perintah SQL disusun dari input user tanpa pengamanan.  
> Jadi, kamu harus ngerti gimana perintah SQL ditulis dan dikirim ke server.

---

## 🛠️ SQL & Server: Selalu Butuh Server?

Nggak selalu.

Ada dua tipe penggunaan SQL:

### 1. 📂 **Tanpa Server (Embedded DB)**  
Database langsung disimpan di file dan bisa diakses langsung.

Contoh:
- `SQLite`
- `HSQLDB`
- `DuckDB`

Kelebihannya:
- Simpel
- Cocok untuk aplikasi kecil atau desktop

---

### 2. 🌐 **Dengan Server (Server-Based DBMS)**  
Database dijalankan di server terpisah dan diakses oleh aplikasi dari luar.

Contoh:
- `MySQL` / `MariaDB`
- `PostgreSQL`
- `Oracle`
- `Microsoft SQL Server`

Biasanya digunakan oleh **aplikasi web dan enterprise**.

Untuk mengaksesnya, kita butuh **client**:
- 🖥️ CLI (misalnya: `mysql`, `psql`)
- 🧩 GUI (misalnya: DBeaver, pgAdmin, HeidiSQL)

---

## 🔁 Peran SQL di Aplikasi Web (CRUD)

Dalam aplikasi web, interaksi dengan database umumnya terjadi seperti ini:

```text
Client (Browser)
   ↓
Web Server
   ↓  (mengirim perintah SQL)
DBMS (Database)
   ↓
Kembaliin hasil → ditampilkan di browser
  

Perintah SQL biasanya digunakan untuk operasi CRUD:

CREATE → Menambahkan data baru

READ → Mengambil data

UPDATE → Mengubah data

DELETE → Menghapus data


