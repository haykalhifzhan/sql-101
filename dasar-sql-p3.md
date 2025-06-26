# 🌐 Server Publik, Schema, dan Tipe Data dalam Database

## 🔓 Server SQL yang Terbuka (Publik)

Secara umum, **server SQL dilindungi dengan username dan password** untuk membatasi siapa yang boleh mengakses database.

Namun, jika:
- Server tersebut **bisa diakses dari internet (publik)**, dan
- Password-nya **bocor atau lemah**,

...maka **siapa pun** bisa masuk dan mengakses database tersebut — tanpa perlu SQL Injection! 😱

> 🎯 Dalam kasus seperti ini, celah keamanannya bukan SQLi, tapi **akses langsung ke server**.  
> Inilah pentingnya menjaga kredensial dan membatasi akses publik.

---

## 🗂️ Apa Itu Schema dalam Database?

Banyak DBMS modern mendukung konsep **schema**, yaitu:

> Cara untuk mengelompokkan tabel-tabel dalam satu database.

Contohnya:
- Di **PostgreSQL**, satu database bisa punya banyak schema.
- Di **MySQL**, istilah “schema” sering dianggap sama dengan “database”.

### 🔐 Fungsi Schema

Schema bisa dipakai untuk:
- Mengelompokkan data berdasarkan aplikasi atau fitur,
- Memberikan **permission berbeda** ke tiap user berdasarkan schema.

Contoh:
- User A cuma boleh akses `schema_pengguna`,
- User B hanya bisa lihat `schema_keuangan`.

---

## 🧪 Cobain Sendiri: Install Database Server

Biar makin paham, coba install dan eksplorasi sendiri.

Misalnya:
- Install **MariaDB** (turunan dari MySQL),
- Coba bikin database, tabel, isi data, dan akses via CLI atau GUI.

> 💡 Belajar SQL itu paling nempel kalau langsung praktik, bukan cuma baca teori.

---

## ❗ Pentingnya Paham SQL, Bukan Cuma Pakai Tool

SQL Injection itu teknik manipulasi **perintah SQL** supaya database melakukan hal yang tidak seharusnya.

Contoh target:
- Login tanpa password
- Dump semua data user
- Hapus tabel, dll

Tapi...

> Kalau kamu **nggak ngerti struktur SQL**, kamu bakal **tergantung sama tool otomatis**.  
> Dan kenyataannya: **tool nggak selalu bisa nemuin bug**.

Jadi, paham dasarnya itu wajib banget kalau mau serius di dunia security 🔐

---

## 🧱 Field & Tipe Data

Dalam spreadsheet, kita punya **header kolom**.  
Nah di database, header itu disebut **field**.

Setiap field punya **tipe data**. Misalnya:
- `INTEGER` untuk angka
- `VARCHAR` untuk teks
- `DATE` untuk tanggal
- `BOOLEAN` untuk true/false

> 🧮 Kita nggak bisa sembarangan masukin teks ke field angka, atau sebaliknya.  
> Beberapa DBMS memang auto-convert, tapi sebaiknya tetap sesuai tipe biar aman & efisien.

Contoh yang salah:
```sql
-- Salah: masukin teks ke kolom angka
INSERT INTO produk (nama, harga) VALUES ('Es Teh', 'dua ribu');
