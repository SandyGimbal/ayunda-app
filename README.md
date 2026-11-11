# CryptoWeb Suite — Tugas Web Ayunda

<div align="center">

![Cybersecurity Cryptography Suite](https://img.shields.io/badge/Security-Client--Side%20Zero--Trust-06b6d4?style=for-the-badge&logo=shield)
![Single File Web Application](https://img.shields.io/badge/Architecture-Single%20Page%20HTML5-6366f1?style=for-the-badge&logo=html5)
![Tailwind CSS](https://img.shields.io/badge/Styling-Tailwind%20CSS%20CDN-38bdf8?style=for-the-badge&logo=tailwindcss)
![Web Audio API](https://img.shields.io/badge/Audio-Web%20Audio%20Synthesizer-10b981?style=for-the-badge&logo=audio)
![Author: Ayunda](https://img.shields.io/badge/Author-Ayunda-f43f5e?style=for-the-badge)

<p align="center">
  <strong>Aplikasi Web Interaktif Multi-Algoritma Kriptografi & Keamanan Siber</strong><br>
  Didesain dengan antarmuka <em>Dark Mode Glassmorphism</em> futuristik, ramah penggunaan mobile satu jempol, dan ditenagai efek suara siber berbasis Web Audio API.
</p>

[**🌐 Live Demo Website**](https://sandygimbal.github.io/ayunda-app/) &bull; [**📖 Dokumentasi Fitur**](#-fitur-utama) &bull; [**🔐 Detail Algoritma**](#-algoritma-kriptografi)

</div>

---

## 📌 Identitas Proyek
- **Nama Mahasiswa / Pengembang:** Ayunda
- **Mata Kuliah / Pelatihan:** Pemrograman Web & Keamanan Siber
- **Nama Aplikasi:** CryptoWeb Suite (v2.4 Pro Edition)
- **Repositori GitHub:** [SandyGimbal/ayunda-app](https://github.com/SandyGimbal/ayunda-app)
- **Deployment URL:** [https://sandygimbal.github.io/ayunda-app/](https://sandygimbal.github.io/ayunda-app/)

---

## 🎯 Ringkasan Aplikasi
**CryptoWeb Suite** adalah aplikasi web edukatif dan praktis yang dirancang dalam **1 (satu) file `index.html` tunggal** tanpa ketergantungan server backend (*100% Client-Side Zero-Trust Architecture*). Seluruh proses enkripsi, dekripsi, dan pembangkitan kunci dieksekusi langsung di browser pengguna secara aman.

Aplikasi ini menyatukan 3 era kriptografi ke dalam satu dashboard terpadu:
1. **Era Klasik (Classic Substitution Cipher):** Caesar Cipher dan Vigenère Cipher.
2. **Era Modern Simetris (Symmetric Block Cipher):** Advanced Encryption Standard (AES-256) via CryptoJS.
3. **Era Modern Asimetris (Public-Key Cryptography):** RSA Key Pair Generation & Cipher Suite via JSEncrypt.

---

## ✨ Fitur Unggulan (UI/UX "WOW" & Mobile-First)

### 📱 1. Pengalaman Mobile Ramah Jempol (Mobile-First UX)
- **Sticky Bottom Navigation:** Bilah tab navigasi di bagian bawah layar ponsel untuk memudahkan navigasi satu tangan (*thumb-zone navigation*).
- **Auto-Scroll Pintar:** Layar smartphone otomatis bergulir (*smooth scroll*) ke kotak hasil saat tombol Enkripsi/Dekripsi ditekan.
- **Touch Targets Ergonomis:** Seluruh tombol berukuran minimal `48px`–`50px` yang nyaman dan presisi disentuh.
- **Tombol Tempel Cepat (*Paste from Clipboard*):** Memasukkan pesan atau kunci tanpa repot melakukan *long-press* bawaan HP.
- **Caesar Stepper Buttons (`+` / `-`):** Mengubah geseran angka Caesar langsung lewat tombol cepat tanpa harus memunculkan keyboard angka HP.
- **Collapsible RSA Keys:** Drawer buka-tutup untuk kunci publik/privat RSA yang panjang agar tidak memenuhi layar ponsel.

### 🔊 2. Web Audio API Cyber Sound Synthesizer
- Menggunakan **Web Audio API Oscillator** murni tanpa file MP3 eksternal (100% berbunyi instan di semua peramban).
- **Feedback Suara Berbeda:**
  - *Ascending Arpeggio:* Saat data berhasil dienkripsi / dikunci.
  - *Harmonic Unlock Chord:* Saat data berhasil didekripsi / dibuka.
  - *Sci-Fi Telemetry:* Saat membangkitkan pasangan kunci RSA atau mengisi data contoh.
  - *Double Chime:* Saat menyalin hasil ke papan klip (*clipboard*).
  - *Cyber Warning Buzzer:* Saat input kosong atau kunci tidak valid.
- Dilengkapi tombol toggle **SFX: ON / MUTE** dengan visualizer *equalizer* animasi.

### ⚡ 3. Animasi Visual & Interaktivitas
- **Matrix / Cyber Decoding Effect:** Menampilkan animasi pengacakan karakter siber sebelum teks output terbaca sempurna.
- **Cyber Flash Glow:** Efek kilatan cahaya neon pada bingkai kotak hasil.
- **Sistem Toast Notifikasi:** Umpan balik visual transparan elegan untuk setiap aksi berhasil maupun gagal.
- **Kartu Identitas Ayunda Modal:** Pop-up profil pengembang tugas dengan backdrop blur dan emblem terverifikasi.
- **Tombol "Isi Contoh Otomatis":** Mempersingkat waktu uji coba dengan 1 klik untuk mengisi pesan dan kunci bertema Ayunda.

---

## 🔐 Algoritma Kriptografi

| No | Tab Algoritma | Metode | Tipe Kunci | Deskripsi Operasional |
|:---:|:---|:---|:---|:---|
| **01** | **Classic Cipher** | Caesar Cipher | Angka Integer (1 - 25) | Substitusi monoalfabetik dengan pergeseran huruf: $C = (P + K) \pmod{26}$. |
| | | Vigenère Cipher | Kata Teks (A-Z) | Substitusi polialfabetik berulang berdasarkan deret karakter kunci: $C_i = (P_i + K_i) \pmod{26}$. |
| **02** | **AES Encryption** | AES-256 (CBC / OpenSSL) | Secret Passphrase | Standar enkripsi simetris berbasis blok 128-bit dengan kunci 256-bit dan salt acak kriptografis. |
| **03** | **RSA Encryption** | RSA (PKCS#1 v1.5) | Sepasang Kunci PEM | Kriptografi asimetris: Enkripsi dengan **Public Key** dan Dekripsi wajib dengan **Private Key**. |

---

## 🚀 Cara Menjalankan Aplikasi

### Opsi A: Buka Langsung Secara Lokal (Offline Ready)
1. Unduh atau clone repositori ini:
   ```bash
   git clone https://github.com/SandyGimbal/ayunda-app.git
   ```
2. Buka folder repositori dan klik dua kali pada file `index.html`.
3. Aplikasi akan langsung berjalan di browser Anda (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari, atau Brave).

### Opsi B: Akses via GitHub Pages (Online)
Buka tautan berikut di peramban komputer atau smartphone Anda:
👉 **[https://sandygimbal.github.io/ayunda-app/](https://sandygimbal.github.io/ayunda-app/)**

---

## 🛠️ Tumpukan Teknologi
- **Struktur Markup:** HTML5 Semantik
- **Desain & Gaya:** Tailwind CSS (via CDN) + Custom Cyberpunk Glow Utilities
- **Tipografi:** Google Fonts (*Plus Jakarta Sans* & *JetBrains Mono*)
- **Pemrosesan Logika:** Vanilla JavaScript (ES6+)
- **Library Kriptografi:**
  - `CryptoJS v4.2.0` (AES-256 Block Cipher)
  - `JSEncrypt v3.3.2` (RSA Key Pair Generator & Asymmetric Cipher)
- **Audio Engine:** HTML5 Web Audio API (Synthesizer Tones)

---

## 📄 Lisensi & Hak Cipta
Dibuat dengan dedikasi oleh **Ayunda** untuk keperluan pemenuhan tugas akademik Pemrograman Web & Keamanan Siber 2026. Bebas digunakan dan dikembangkan untuk tujuan edukasi.
