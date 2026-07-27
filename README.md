# 🛡️ CELAH — Kuis Temukan Celah Keamanan

Aplikasi web edukasi interaktif untuk melatih pemahaman **keamanan siber** (cyber security) lewat kuis, latihan code review, dan simulasi serangan — dirancang khusus untuk pemula, bukan ahli keamanan siber.

Dibangun sebagai single-file web app: HTML, CSS, dan JavaScript murni tanpa dependency eksternal, tanpa backend. Berjalan sepenuhnya di browser.

---

## ✨ Fitur Utama

### 📚 Kuis Interaktif — 40 Soal
- Campuran soal **teori** dan **potongan kode nyata** yang mengandung celah keamanan
- Terstruktur progresif: **Dasar (12)** → **Menengah (17)** → **Lanjutan (11)**
- Topik: SQL Injection, XSS, CSRF, hardcoded secret, command injection, CORS misconfig, IDOR, session token lemah, path traversal, JWT tanpa verifikasi, race condition, mass assignment, NoSQL injection, prototype pollution, web cache poisoning, dan lainnya
- Setiap jawaban disertai **"Kenapa begini"** (akar masalah) dan **"Yang perlu diingat"** (cara memperbaiki) — bukan sekadar benar/salah

### 🎯 Tiga Mode Belajar
| Mode | Karakteristik |
|---|---|
| **Belajar** | Tanpa batas waktu, ada tombol Petunjuk, penjelasan lengkap. Direkomendasikan untuk pemula. |
| **Tantangan** | Ada batas waktu per soal (menyesuaikan tipe & tingkat kesulitan). |
| **Jam Terbang** | Latihan praktik: **Temukan** baris kode rentan → **Diagnosis** jenis celahnya → **Perbaiki** dengan kode yang tepat → **Simulasikan Serangan** (lihat before/after apa yang sebenarnya terjadi). 15 soal praktik, tanpa timer. |

### 🗺️ Jalur Belajar Terstruktur
Fokus latihan ke satu tingkat saja — **Fondasi**, **Menengah**, **Lanjutan** — atau kerjakan **Lengkap** (semua 40 soal).

### 🧭 Checkpoint & Anti-Overstudy
Sesi otomatis berhenti sejenak tiap 10 soal untuk koreksi hasil (stage report), dengan opsi lanjut atau berhenti tanpa kehilangan progres.

### 🔁 Latihan Ulang yang Salah
Setelah selesai, fokuskan latihan ulang hanya ke soal yang meleset — tidak perlu mengulang semuanya dari awal.

### 🏆 Papan Skor & Riwayat
Skor tertinggi tersimpan otomatis (localStorage), lengkap dengan mode dan jalur yang dipakai.

### 📖 Panduan Lengkap
Modal berisi Cara Bermain, Contoh Soal, **Kamus Ancaman** (glosarium teknik serangan JS umum secara konseptual), dan **Sumber Belajar** (rekomendasi platform seperti OWASP, PortSwigger Web Security Academy, TryHackMe, BSSN).

### 🌗 Light & Dark Mode
Menyesuaikan preferensi sistem otomatis, tersimpan di perangkat.

---

## 🛠️ Tech Stack
- **HTML5** — struktur multi-screen (SPA sederhana tanpa framework)
- **CSS3** — desain bertema terminal/hacker, custom properties untuk theming
- **JavaScript (Vanilla ES6)** — state management, DOM manipulation, tanpa library
- **localStorage** — persistensi skor, tema, dan progres jam terbang

Tidak ada build step, tidak ada backend. Cukup buka `index.html` di browser.

---

## 🚀 Menjalankan Secara Lokal

```bash
git clone https://github.com/<username>/<repo-name>.git
cd <repo-name>
# buka langsung di browser
open index.html      # macOS
start index.html      # Windows
```

Atau serve dengan server statis sederhana:
```bash
npx serve .
```

---

## 📂 Struktur

Proyek ini adalah **satu file HTML mandiri** — semua CSS dan JavaScript ada di dalamnya. Tidak ada folder `src/`, tidak ada `node_modules`.

---

## ⚠️ Disclaimer

Aplikasi ini adalah **alat latihan kesadaran keamanan siber**, bukan alat produksi maupun alat eksploitasi. Semua contoh kode kerentanan bersifat ilustratif untuk tujuan edukasi.

---

## 📝 Lisensi

Bebas digunakan untuk keperluan pembelajaran.
