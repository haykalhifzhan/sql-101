# 📘 Belajar SQL dari Nol — Catatan Santai tapi Nendang!

> Repository ini berisi catatan saya selama belajar SQL dasar dari nol. Cocok buat kamu yang pengen ngerti gimana cara kerja database, query, relasi antar tabel, dan latihan CRUD (Create, Read, Update, Delete).

SQL itu penting banget kalau kamu:
- Lagi belajar backend development
- Pengen jadi data analyst/data engineer
- Atau... lagi ngulik SQL Injection buat CTF/hacking 😏

---

## 🧭 Daftar Isi

📁 `dasar-sql/`  
Perintah-perintah dasar SQL seperti `SELECT`, `WHERE`, `JOIN`, dll.

📁 `function/`  
Fungsi-fungsi umum di SQL kayak `CONCAT()`, `NOW()`, `ROUND()`, dll.

📁 `latihan/`  
Soal latihan + file dummy database buat ngelatih skill query-mu.

📁 `cheatsheet/`  
Ringkasan perintah SQL penting, cocok buat nyontek cepet pas butuh.

---

## ⚡ Tools yang Digunakan

- 💾 **MariaDB** (alternatif open-source MySQL)
- 🖥️ **Terminal CLI** (biar hafal sintaks)
- 🐿️ **DBeaver** (opsional, buat lihat data secara visual)
- 🐧 **Ubuntu/Linux** (bisa juga pakai WSL)

---

## 🔥 Progress Belajar

| Topik                        | Status     |
|-----------------------------|------------|
| SQL Dasar (`SELECT`, `WHERE`) | ✅ Selesai |
| `JOIN` (INNER, LEFT, dll)   | 🔄 On Progress |
| Fungsi `COUNT`, `SUM`, `AVG`| 🔜 Soon    |
| Subquery & Nested Query     | 🔜 Soon    |

---

## 🧪 Contoh Query Dasar

```sql
-- Menampilkan semua data
SELECT * FROM users;

-- Menampilkan nama user yang umurnya di atas 20
SELECT username FROM users WHERE age > 20;

-- Menambah data baru
INSERT INTO users (username, age) VALUES ('haykal', 22);
