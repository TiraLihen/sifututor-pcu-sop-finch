# PCU SOP Finch & Ripple Web App

Panduan ini menerangkan cara untuk menjalankan pelayan pembangunan tempatan (*local dev server*) dan melakukan deployment ke **Vercel**.

## 💻 Cara Menjalankan Secara Tempatan (Local)

Pastikan anda mempunyai **Node.js** terpasang pada komputer anda.

1. Buka terminal (PowerShell / Command Prompt) di dalam folder projek ini.
2. Pasang dependencies:
   ```bash
   npm install
   ```
3. Jalankan pelayar pembangunan tempatan:
   ```bash
   npm run dev
   ```
4. Buka pelayar web dan akses pautan yang dipaparkan (biasanya `http://localhost:5173`).

---

## 🚀 Cara Deployment ke Vercel

Anda boleh menggunakan salah satu daripada dua kaedah berikut untuk melakukan deployment:

### Kaedah A: Menggunakan Sambungan GitHub (Disyorkan)

1. Muat naik folder projek ini ke dalam repositori **GitHub** anda (awam atau peribadi).
2. Log masuk ke papan pemuka **Vercel** ([https://vercel.com/](https://vercel.com/)).
3. Klik **Add New** ➔ **Project**.
4. Import repositori GitHub yang anda muat naik tadi.
5. Vercel akan mengesan konfigurasi static secara automatik (Framework Preset: Other / Vite).
6. Klik **Deploy**. Selesai! Sebarang kemas kini (*push*) pada repositori GitHub akan mengemas kini laman web anda secara automatik.

### Kaedah B: Menggunakan Vercel CLI (Pantas)

1. Pasang vercel secara global menggunakan npm:
   ```bash
   npm install -g vercel
   ```
2. Jalankan arahan login:
   ```bash
   vercel login
   ```
3. Di dalam folder projek ini, jalankan arahan deployment:
   ```bash
   vercel
   ```
4. Jawab soalan konfigurasi di skrin (tekan Enter untuk pilihan lalai).
5. Selepas selesai, jalankan arahan berikut untuk production build:
   ```bash
   vercel --prod
   ```
6. Vercel akan memberikan pautan URL unik untuk mengakses SOP PCU anda secara langsung dari internet!
