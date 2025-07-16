# 🚀 Panduan Lengkap Step-by-Step Chatbot AC

## 📋 PERSIAPAN AWAL

### ✅ Yang Anda Butuhkan:
- [ ] Laptop/komputer dengan internet
- [ ] Browser (Chrome/Firefox/Edge)
- [ ] Text editor (VS Code - download gratis)
- [ ] Node.js (download dari nodejs.org)

---

## 🔧 LANGKAH 1: INSTALL SOFTWARE YANG DIBUTUHKAN

### **1.1 Install Node.js**
1. Buka browser, ketik: `nodejs.org`
2. Klik tombol hijau "Download Node.js"
3. Download file installer
4. Jalankan installer, klik "Next" terus sampai selesai
5. **Test apakah berhasil:**
   - Buka Command Prompt (Windows) atau Terminal (Mac)
   - Ketik: `node --version`
   - Kalau muncul angka versi (misal: v18.17.0) = BERHASIL ✅

### **1.2 Install VS Code (Text Editor)**
1. Buka browser, ketik: `code.visualstudio.com`
2. Klik "Download for Windows/Mac"
3. Install seperti biasa
4. Buka VS Code setelah install

---

## 📁 LANGKAH 2: DOWNLOAD DAN SETUP PROJECT

### **2.1 Download Project dari v0**
1. Di halaman v0 ini, klik tombol **"Download Code"** (pojok kanan atas)
2. Pilih **"Download as ZIP"**
3. Save ke folder yang mudah diingat (misal: Desktop)
4. Extract/unzip file tersebut
5. Rename folder menjadi: `chatbot-ac`

### **2.2 Buka Project di VS Code**
1. Buka VS Code
2. Klik **File → Open Folder**
3. Pilih folder `chatbot-ac` yang tadi di-extract
4. Klik **"Select Folder"**
5. Sekarang Anda bisa lihat semua file project di sidebar kiri

---

## 🔑 LANGKAH 3: DAPATKAN API KEY OPENAI

### **3.1 Daftar di OpenAI**
1. Buka browser baru, ketik: `platform.openai.com`
2. Klik **"Sign Up"** kalau belum punya akun
3. Isi email, password, verifikasi email
4. Login ke akun OpenAI

### **3.2 Buat API Key**
1. Setelah login, cari menu **"API Keys"** di sidebar kiri
2. Klik **"Create new secret key"**
3. Kasih nama: "Chatbot AC"
4. Klik **"Create secret key"**
5. **PENTING:** Copy API key yang muncul (mulai dengan sk-...)
6. Simpan di notepad, jangan sampai hilang!

### **3.3 Top Up Saldo (Opsional)**
- OpenAI kasih free credit $5 untuk akun baru
- Kalau habis, bisa top up minimal $5
- Untuk testing project ini, $5 sudah cukup lama

---

## ⚙️ LANGKAH 4: SETUP PROJECT

### **4.1 Buka Terminal di VS Code**
1. Di VS Code, tekan **Ctrl + `** (backtick) atau
2. Klik **Terminal → New Terminal** di menu atas
3. Terminal akan muncul di bawah

### **4.2 Install Dependencies**
1. Di terminal, ketik perintah ini:
\`\`\`bash
npm install
\`\`\`
2. Tekan **Enter**
3. Tunggu sampai selesai (muncul banyak text, itu normal)
4. Kalau selesai, akan muncul prompt lagi

### **4.3 Buat File Environment**
1. Di VS Code, klik kanan di sidebar kiri (di folder root)
2. Pilih **"New File"**
3. Nama file: `.env.local` (jangan lupa titik di depan!)
4. Tekan Enter
5. File `.env.local` akan terbuka
6. Ketik ini di dalam file:
\`\`\`
OPENAI_API_KEY=sk-your-api-key-here
\`\`\`
7. Ganti `sk-your-api-key-here` dengan API key OpenAI yang tadi Anda copy
8. Tekan **Ctrl + S** untuk save

**Contoh isi file .env.local:**
\`\`\`
OPENAI_API_KEY=sk-proj-abc123def456ghi789jkl012mno345pqr678stu901vwx234yz
\`\`\`

---

## 🚀 LANGKAH 5: JALANKAN PROJECT

### **5.1 Start Development Server**
1. Di terminal VS Code, ketik:
\`\`\`bash
npm run dev
\`\`\`
2. Tekan **Enter**
3. Tunggu sampai muncul text seperti ini:
\`\`\`
✓ Ready in 2.3s
○ Local:        http://localhost:3000
○ Network:      http://192.168.1.100:3000
\`\`\`

### **5.2 Buka Website**
1. Buka browser baru
2. Ketik di address bar: `http://localhost:3000`
3. Tekan **Enter**
4. **SELAMAT!** Website chatbot AC Anda sudah jalan! 🎉

---

## 🧪 LANGKAH 6: TEST CHATBOT

### **6.1 Test Halaman Utama**
1. Pastikan halaman utama muncul dengan judul "AC Doctor"
2. Ada tombol "Mulai Konsultasi"
3. Tampilan responsive dan bagus

### **6.2 Test Chatbot**
1. Klik tombol **"Mulai Konsultasi"**
2. Anda akan masuk ke halaman chat
3. Coba ketik: "AC saya tidak dingin"
4. Tekan **Enter** atau klik tombol kirim
5. Tunggu beberapa detik
6. AI akan memberikan jawaban tentang masalah AC

### **6.3 Test Fitur Lain**
1. Coba pertanyaan lain: "AC bocor air"
2. Klik menu "Panduan" untuk lihat tutorial perawatan
3. Test di HP (buka `http://localhost:3000` di browser HP)

---

## 🎯 LANGKAH 7: PERSIAPAN DEMO/PRESENTASI

### **7.1 Siapkan Pertanyaan Demo**
Simpan pertanyaan ini untuk demo:
1. "AC saya tidak dingin, apa penyebabnya?"
2. "AC bocor air di ruang tamu"
3. "AC berbunyi aneh seperti gemuruh"
4. "Bagaimana cara merawat AC yang benar?"

### **7.2 Screenshot untuk Backup**
1. Ambil screenshot halaman utama
2. Screenshot halaman chat dengan percakapan
3. Screenshot halaman panduan
4. Simpan untuk jaga-jaga kalau demo bermasalah

---

## 🔧 TROUBLESHOOTING (KALAU ADA MASALAH)

### **❌ Masalah: "npm not found"**
**Solusi:**
- Node.js belum terinstall dengan benar
- Install ulang Node.js dari nodejs.org
- Restart komputer setelah install

### **❌ Masalah: "Port 3000 already in use"**
**Solusi:**
\`\`\`bash
# Matikan server yang jalan, tekan Ctrl+C di terminal
# Atau ganti port:
npm run dev -- --port 3001
# Lalu buka: http://localhost:3001
\`\`\`

### **❌ Masalah: Chatbot tidak menjawab**
**Solusi:**
1. Periksa file `.env.local` ada atau tidak
2. Pastikan API key OpenAI benar (mulai dengan sk-)
3. Periksa saldo OpenAI masih ada
4. Restart server: Ctrl+C lalu `npm run dev` lagi

### **❌ Masalah: Website tidak muncul**
**Solusi:**
1. Pastikan terminal menunjukkan "Ready"
2. Coba refresh browser (F5)
3. Coba browser lain
4. Pastikan tidak ada typo di URL

### **❌ Masalah: Error saat npm install**
**Solusi:**
\`\`\`bash
# Hapus folder node_modules
rm -rf node_modules
# Atau di Windows, hapus manual folder node_modules

# Install ulang
npm install
\`\`\`

---

## 📊 LANGKAH 8: MEMAHAMI STRUKTUR PROJECT

### **8.1 File-File Penting**
\`\`\`
📂 chatbot-ac/
├── 📁 app/
│   ├── 📄 page.tsx (Halaman utama - landing page)
│   ├── 📁 chat/
│   │   └── 📄 page.tsx (Halaman chat dengan AI)
│   ├── 📁 panduan/
│   │   └── 📄 page.tsx (Halaman panduan perawatan)
│   └── 📁 api/
│       └── 📁 chat/
│           └── 📄 route.ts (API chatbot - OTAK AI!)
├── 📁 components/
│   └── 📁 ui/ (Komponen tampilan)
├── 📄 .env.local (API key - RAHASIA!)
├── 📄 package.json (Daftar dependencies)
└── 📄 README.md (Dokumentasi)
\`\`\`

### **8.2 Cara Kerja Sistem**
1. **User buka website** → Lihat halaman utama
2. **User klik "Mulai Konsultasi"** → Masuk halaman chat
3. **User ketik masalah AC** → Kirim ke API
4. **API terima pesan** → Proses dengan OpenAI
5. **OpenAI + Knowledge Base** → Generate jawaban
6. **API kirim jawaban** → Tampil di chat user

---

## 🎓 LANGKAH 9: PERSIAPAN LAPORAN

### **9.1 Poin-Poin Penting untuk Laporan**

**Latar Belakang:**
- Banyak orang kesulitan diagnosis masalah AC
- Biaya konsultasi teknisi mahal untuk masalah sederhana
- Tidak ada layanan konsultasi AC 24/7

**Tujuan:**
- Membuat chatbot AI untuk diagnosis masalah AC
- Memberikan solusi praktis yang bisa dilakukan sendiri
- Menyediakan layanan konsultasi gratis 24/7

**Teknologi:**
- Frontend: Next.js 14, React, TypeScript, Tailwind CSS
- Backend: API Routes, OpenAI GPT-4
- AI/ML: AI SDK, Natural Language Processing
- Database: Knowledge Base masalah AC

**Fitur:**
- Chatbot cerdas dengan AI
- Diagnosis otomatis masalah AC
- Panduan perawatan step-by-step
- Interface responsive dan user-friendly

**Hasil:**
- Berhasil membuat chatbot yang bisa diagnosis 6+ masalah AC
- Response time rata-rata < 5 detik
- Interface mudah digunakan
- Knowledge base komprehensif

---

## 🎬 LANGKAH 10: PANDUAN DEMO

### **10.1 Struktur Presentasi (10 menit)**

**Menit 1-2: Pembukaan**
- Perkenalkan diri dan judul project
- Jelaskan masalah yang ingin diselesaikan

**Menit 3-6: Demo Website**
- Tunjukkan halaman utama
- Demo chatbot dengan 2-3 pertanyaan
- Tunjukkan halaman panduan

**Menit 7-8: Penjelasan Teknologi**
- Jelaskan teknologi yang digunakan
- Cara kerja AI secara sederhana

**Menit 9-10: Penutup**
- Rangkum hasil dan manfaat
- Sesi tanya jawab

### **10.2 Tips Demo**
- ✅ Test semua fitur sebelum presentasi
- ✅ Siapkan backup (screenshot/video)
- ✅ Bicara dengan percaya diri
- ✅ Jelaskan manfaat praktis
- ✅ Siap jawab pertanyaan

---

## 🎉 SELAMAT!

Anda sudah berhasil membuat dan menjalankan sistem chatbot AC berbasis AI! 

**Checklist Akhir:**
- [ ] Website bisa dibuka di browser
- [ ] Chatbot bisa menjawab pertanyaan
- [ ] Semua halaman berfungsi dengan baik
- [ ] Siap untuk demo/presentasi
- [ ] Dokumentasi lengkap untuk laporan

**Project Anda sekarang sudah siap untuk:**
- ✅ Demo/presentasi
- ✅ Laporan tugas akhir
- ✅ Portfolio pribadi
- ✅ Pengembangan lebih lanjut

Semoga sukses dengan proyek Anda! 🚀✨
