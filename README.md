# 🚀 Technical Assessment: Task Management API

## 📌 Gambaran Umum

Tugas ini adalah membuat aplikasi sederhana bernama **Task Tracker**.

Tujuan dari assessment ini adalah untuk menunjukkan kemampuan dalam:

- Menggunakan asynchronous programming di Python
- Melakukan validasi data
- Menghubungkan backend ke antarmuka pengguna (UI) sederhana

---

## 📋 Requirements

### 1️⃣ Backend

Buat RESTful API untuk mengelola daftar task. 
Direkomendasikan menggunakan **FastAPI**, namun kandidat diperbolehkan menggunakan framework backend lain.

Setiap task harus memiliki atribut berikut:

- `id`
- `title`
- `description`
- `status` (contoh: `"pending"` atau `"completed"`)

Endpoint yang harus tersedia:

- `POST /tasks`  
  Membuat task baru

- `GET /tasks`  
  Mengambil semua task

- `GET /tasks/{id}`  
  Mengambil task berdasarkan ID

- `PUT /tasks/{id}`  
  Mengupdate status atau detail task

- `DELETE /tasks/{id}`  
  Menghapus task

#### Catatan:

- Gunakan **Pydantic** untuk validasi request dan response bila menggunakan FastAPI.
- Anda boleh menggunakan:
  - In-memory list (penyimpanan sementara), atau
  - Database SQLite sederhana dengan SQLAlchemy atau SQLModel.

---

### 2️⃣ Frontend (Simple UI)

Buat single-page interface menggunakan HTML dan JavaScript yang:

- Mengambil dan menampilkan daftar task
- Memiliki form sederhana untuk menambahkan task baru
- Menggunakan `fetch()` untuk berkomunikasi dengan backend FastAPI

---

### 3️⃣ Testing (Opsional)

Sertakan file `tests.py` menggunakan:

- `pytest`

Untuk menguji endpoint API yang telah dibuat.

---

## Additional Question

Sertakan jawaban dari pertanyaan berikut di dalam README:
1. Apakah Anda sering menggunakan tools AI dalam melakukan koding? 
2. Apa ekspektasi Anda terhadap jobdesc dan tanggung jawab di posisi ini?
3. Bagaimana pendekatan Anda dalam menyelesaikan suatu problem teknis?

---

## 📦 Submission Guidelines

### 🔗 GitHub Repository

Push seluruh kode ke repository publik di GitHub.

### 📄 README.md

Repository wajib memiliki file `README.md` yang berisi:

- Cara menjalankan aplikasi
- Jawaban dari pertanyaan tambahan
