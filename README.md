# 🤖 Sistem Chatbot AC - Panduan Mudah

# 🚀 **SETUP SUPER MUDAH - 5 LANGKAH SAJA!**

## **PILIHAN 1: Menggunakan Yarn (RECOMMENDED)**

### **LANGKAH 1: Dapatkan API Key Google Gemini (GRATIS)**
1. **Buka:** `aistudio.google.com`
2. **Login** dengan akun Google
3. **Klik "Get API Key"**
4. **Copy API key** (dimulai dengan `AIzaSy...`)

### **LANGKAH 2: Setup Project**
\`\`\`bash
# Copy semua file dari Code Project
# Buat file .env.local di root folder
# Isi dengan:
GOOGLE_GENERATIVE_AI_API_KEY=AIzaSyYour-Actual-API-Key-Here
\`\`\`

### **LANGKAH 3: Install Dependencies dengan Yarn**
\`\`\`bash
# Install dependencies (lebih cepat dari npm)
yarn install

# Atau bisa juga:
yarn
\`\`\`

### **LANGKAH 4: Jalankan Project**
\`\`\`bash
# Jalankan development server
yarn dev
\`\`\`

### **LANGKAH 5: Test Chatbot**
- Buka `http://localhost:3000`
- Klik "Mulai Konsultasi AI"
- Tanya apapun tentang AC!

---

## **PILIHAN 2: Menggunakan NPM (Alternative)**

## 📋 Langkah-Langkah Setup

### 1. Persiapan Awal
\`\`\`bash
# Download project dari v0
# Buka terminal/command prompt
# Masuk ke folder project
cd sistem-chatbot-ac
\`\`\`

### **LANGKAH 3: Install Dependencies dengan NPM**
\`\`\`bash
# Install dependencies
npm install
\`\`\`

### 2. Install Dependencies
\`\`\`bash
# Install semua package yang dibutuhkan
npm install
\`\`\`

### 3. Setup API Key OpenAI
\`\`\`bash
# Buat file .env.local di root folder
# Isi dengan:
OPENAI_API_KEY=sk-your-api-key-here
\`\`\`

### 4. Jalankan Project
\`\`\`bash
# Jalankan development server
npm run dev
\`\`\`

### **LANGKAH 4: Jalankan Project**
\`\`\`bash
# Jalankan development server
npm run dev
\`\`\`

---

## 🔧 **TROUBLESHOOTING YARN**

### **Kalau Yarn Belum Terinstall:**
\`\`\`bash
# Install Yarn globally
npm install -g yarn

# Cek versi Yarn
yarn --version
\`\`\`

### **Kalau Ada Conflict Dependencies:**
\`\`\`bash
# Clear cache dan install ulang
yarn cache clean
rm -rf node_modules
rm yarn.lock
yarn install
\`\`\`

### **Kalau Error Permission (Mac/Linux):**
\`\`\`bash
# Install dengan sudo
sudo yarn install
\`\`\`

---

## ⚡ **KEUNGGULAN YARN vs NPM:**

### **Yarn Advantages:**
- ✅ **Lebih cepat** install dependencies
- ✅ **Lock file** lebih reliable (yarn.lock)
- ✅ **Parallel downloads** - install bersamaan
- ✅ **Better caching** - tidak download ulang
- ✅ **Deterministic** - hasil sama di semua device

### **Speed Comparison:**
- **Yarn:** ~30-60 detik
- **NPM:** ~60-120 detik

---

## 📋 **SCRIPT COMMANDS:**

### **Dengan Yarn:**
\`\`\`bash
yarn dev          # Jalankan development server
yarn build        # Build untuk production
yarn start        # Jalankan production server
yarn lint         # Check code quality
\`\`\`

### **Dengan NPM:**
\`\`\`bash
npm run dev       # Jalankan development server
npm run build     # Build untuk production
npm run start     # Jalankan production server
npm run lint      # Check code quality
\`\`\`

### 5. Buka Browser
\`\`\`
http://localhost:3000
\`\`\`

## 🔧 Struktur Project Sederhana

\`\`\`
sistem-chatbot-ac/
├── app/
│   ├── page.tsx          # Halaman utama
│   ├── chat/
│   │   └── page.tsx      # Halaman chat
│   ├── panduan/
│   │   └── page.tsx      # Halaman panduan
│   └── api/
│       └── chat/
│           └── route.ts  # API chatbot (PENTING!)
├── components/
│   └── ui/               # Komponen UI
├── .env.local            # API key (BUAT SENDIRI)
└── package.json          # Dependencies
\`\`\`

## 🎯 File Penting yang Perlu Dipahami

### 1. API Chatbot (`app/api/chat/route.ts`)
- File ini yang membuat AI bisa menjawab
- Berisi database pengetahuan AC
- Menggunakan OpenAI GPT-4

### 2. Halaman Chat (`app/chat/page.tsx`)
- Interface untuk berbicara dengan AI
- Mengirim pesan ke API
- Menampilkan jawaban AI

### 3. Halaman Utama (`app/page.tsx`)
- Landing page website
- Informasi tentang sistem
- Tombol untuk mulai chat

## 🚀 Cara Mendapatkan API Key OpenAI

1. Buka https://platform.openai.com
2. Daftar/login akun
3. Masuk ke API Keys
4. Buat API key baru
5. Copy dan paste ke file .env.local

## ✅ Checklist Testing

- [ ] Website bisa dibuka di browser
- [ ] Halaman utama tampil dengan baik
- [ ] Bisa masuk ke halaman chat
- [ ] Bisa mengirim pesan ke chatbot
- [ ] AI memberikan jawaban tentang AC
- [ ] Halaman panduan bisa diakses

## 🎓 Untuk Presentasi/Demo

### Fitur yang Bisa Ditunjukkan:
1. **Landing Page Profesional**
2. **Chatbot AI yang Cerdas**
3. **Diagnosis Masalah AC**
4. **Panduan Perawatan**
5. **Interface User-Friendly**

### Contoh Pertanyaan untuk Demo:
- "AC saya tidak dingin, apa penyebabnya?"
- "AC bocor air, bagaimana mengatasinya?"
- "AC berbunyi aneh, apa solusinya?"

## 🔍 Troubleshooting Mudah

### Masalah: Website tidak bisa dibuka
**Solusi:**
\`\`\`bash
# Pastikan sudah install dependencies
npm install

# Jalankan ulang
npm run dev
\`\`\`

### Masalah: Chatbot tidak menjawab
**Solusi:**
1. Periksa file `.env.local` ada atau tidak
2. Pastikan API key OpenAI benar
3. Restart server (`Ctrl+C` lalu `npm run dev`)

### Masalah: Error saat install
**Solusi:**
\`\`\`bash
# Hapus node_modules dan install ulang
rm -rf node_modules
npm install
\`\`\`

## 📱 Teknologi yang Digunakan

- **Next.js 14** - Framework React
- **AI SDK** - Untuk integrasi AI
- **OpenAI GPT-4** - Model AI
- **Tailwind CSS** - Styling
- **TypeScript** - Programming language

## 🎯 Poin Penting untuk Laporan

1. **Problem**: Sulitnya diagnosis masalah AC untuk orang awam
2. **Solution**: Chatbot AI yang bisa mendiagnosis masalah AC
3. **Technology**: AI/ML dengan OpenAI GPT-4
4. **Features**: Chat interface, knowledge base, panduan perawatan
5. **Benefits**: Diagnosis cepat, solusi praktis, 24/7 available

## 📊 Hasil yang Diharapkan

- ✅ Chatbot bisa mendiagnosis 6+ masalah AC umum
- ✅ Interface yang mudah digunakan
- ✅ Response time < 5 detik
- ✅ Akurasi diagnosis tinggi berdasarkan knowledge base
- ✅ Panduan perawatan yang praktis
