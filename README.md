# Pasar Aksara

Pasar Aksara adalah permainan simulasi pasar tradisional yang interaktif, dirancang khusus untuk mempermudah dan mencerahkan pembelajaran Aksara Jawa bagi pemula. Di dalam game ini, pemain dapat memilih peran sebagai **Pembeli** atau **Penjual**, berinteraksi dengan simulasi transaksi jual beli bahan-bahan tradisional, dan belajar membaca serta merangkai Aksara Jawa.

## 🌟 Fitur Utama

- **Dua Peran Interaktif:**
  - **Pembeli:** Pemain bertugas mencari barang yang tertulis dalam label Aksara Jawa atau merangkai ejaan Aksara Jawa dari nama barang yang diminta.
  - **Penjual:** Pemain melayani permintaan pelanggan yang memesan barang dalam Aksara Jawa, melatih kemampuan membaca sandhangan dan ejaan.
- **Sistem Level (Tingkatan Pembelajaran):**
  - **Level 1 (Nglegena):** Aksara dasar tanpa sandhangan (vokal 'a').
  - **Level 2 (Sandangan):** Aksara dasar yang ditambahkan sandhangan (vokal i, u, e, o).
  - **Level 3 (Pasangan):** Aksara dengan pasangan untuk mematikan konsonan.
- **Papan Peringkat (Leaderboard):** Pemain bersaing mengumpulkan koin (Koin emas) terbanyak berdasarkan tingkat keakuratan dan kecepatan menjawab.
- **Percakapan AI (Mbah Karso):** Asisten virtual berbasis AI (Gemini) bernama Mbah Karso yang siap menuntun pemain, menjelaskan fungsi sandhangan, dan memberikan tips belajar Aksara Jawa.
- **Sistem Progres & Akun:** Login menggunakan Google atau Apple ID untuk menyimpan progres permainan, koin, level, dan posisi di leaderboard.

## 🚀 Konsep Permainan

1. **Pasar:** Mode inti permainan.
   - Pembeli menebak aksara atau merangkai aksara dari barang tradisional yang ada.
   - Penjual menebak barang dari aksara yang diminta pembeli atau merangkai aksara dari pesanan.
2. **Koin & Nyawa:**
   - Menjawab dengan benar akan memberikan **Koin** (+10 Koin) dan mengembalikan 1 nyawa.
   - Jawaban salah akan mengurangi 1 **Koin** dan 1 **Nyawa** (maksimal 3 nyawa).
   - Jika nyawa habis (0), progres level akan dikunci sementara atau direset ke awal.
3. **Papan Peringkat:** Bandingkan pendapatan koinmu dengan saudagar lainnya di pasar.

## 💻 Tech Stack

- **Frontend:** React 18, TypeScript, Vite, Tailwind CSS, Framer Motion
- **Backend/API:** Node.js, Express
- **Database & Auth:** Firebase (Firestore & Firebase Authentication)
- **AI Integration:** Google Gemini API (@google/genai)

## 🛠️ Cara Menjalankan Secara Lokal

Ikuti langkah-langkah di bawah ini untuk menjalankan proyek secara lokal:

### Prasyarat

- **Node.js** (versi 18+)
- **NPM** atau **Yarn**
- Konfigurasi Firebase Project (Database Firestore dan Authentication)
- API Key Google Gemini (untuk layanan asisten Mbah Karso)

### Instalasi

1. Pastikan Anda telah meng-clone repository ini ke mesin loka.
2. Buka terminal pada root direktori proyek.
3. Install semua dependensi menggunakan NPM:
   ```bash
   npm install
   ```

### Konfigurasi Environment Variables

Buka atau buat file `.env` di direktori utama, dan isikan kredensial berikut:

```env
# Gemini API Key untuk asisten Mbah Karso
GEMINI_API_KEY=your_gemini_api_key_here
```

Konfigurasi Firebase Authentication disesuaikan dari Google Cloud Console atau Firebase Dashboard Anda, sesuaikan dengan `firebase-applet-config.json` dan utilitas setup otentikasi.

### Menjalankan Development Server

Jalankan perintah berikut untuk memulai server frontend (Vite) dan backend (Express) secara serentak via `tsx`:

```bash
npm run dev
```

Aplikasi akan berjalan pada port `3000`. Akses `http://localhost:3000` di peramban web Anda.

### Menjalankan Build untuk Produksi

Jika Anda ingin membungkus source code untuk deployment, jalankan:

```bash
npm run build
```
Perintah ini akan menjalankan building Vite untuk frontend (masuk ke folder `dist/`) lalu membundel backend Express ke `dist/server.cjs`.

Untuk menjalankannya:
```bash
npm run start
```

Selamat bermain dan sinau Aksara Jawa! ꧋ꦱꦸꦒꦼꦁꦱꦶꦤꦲꦸ꧉
