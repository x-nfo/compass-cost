🍳 Cuisine Cost Compass
Cuisine Cost Compass adalah aplikasi web modern yang dirancang untuk membantu pemilik bisnis F&B (Makanan & Minuman) dalam menghitung Harga Pokok Penjualan (HPP), mensimulasikan strategi harga, dan menganalisis profitabilitas secara akurat.

✨ Fitur Utama
Manajemen Biaya: Kelola semua komponen biaya mulai dari bahan baku, kemasan, tenaga kerja, hingga overhead pabrik dan operasional.

Kalkulator HPP Dinamis: Bangun resep untuk produk jadi atau sub-resep, dan dapatkan perhitungan HPP per porsi secara otomatis dan real-time.

Visualisasi Struktur Biaya: Pahami komposisi biaya produk Anda melalui diagram lingkaran yang interaktif.

Kalkulator Harga Jual: Tentukan harga jual optimal berdasarkan HPP dan target margin keuntungan yang Anda inginkan.

Analisis Profitabilitas: Simulasikan dampak dari biaya channel penjualan (Gojek, Grab, dll.) dan promosi terhadap laba bersih Anda.

Integrasi AI (Google Genkit): Dapatkan penjelasan detail tentang struktur HPP dan analisis strategis dari AI untuk membantu pengambilan keputusan.

Dashboard Intuitif: Pantau metrik-metrik kunci bisnis F&B Anda dalam satu tampilan ringkas.

🛠️ Tumpukan Teknologi (Tech Stack)
Komponen	Teknologi
Backend	
Frontend	
Database	
UI/Styling	
AI	

Export to Sheets
📂 Struktur Repositori
Proyek ini menggunakan struktur monorepo sederhana dengan dua folder utama:

/server: Berisi aplikasi backend Express.js.

/client: Berisi aplikasi frontend Vue.js.

🚀 Instalasi dan Menjalankan Proyek
Untuk menjalankan proyek ini di lingkungan lokal Anda, ikuti langkah-langkah berikut.

Prasyarat
Node.js (v18 atau lebih tinggi)

NPM atau Yarn

MySQL Server

Langkah-langkah
Clone repositori ini:

Bash

git clone https://github.com/[NAMA_PENGGUNA_ANDA]/[NAMA_REPO_ANDA].git
cd [NAMA_REPO_ANDA]
Setup Backend (/server):

Bash

# Masuk ke direktori server
cd server

# Install dependensi
npm install

# Salin file .env.example menjadi .env
cp .env.example .env

# Sesuaikan variabel di dalam file .env dengan konfigurasi database Anda
# Jalankan migrasi untuk membuat tabel (jika menggunakan ORM seperti Prisma/Sequelize)
# Jika tidak, impor file skema .sql secara manual ke database MySQL Anda

# Jalankan server backend
npm run dev
Setup Frontend (/client):

Bash

# Buka terminal baru, kembali ke root proyek, lalu masuk ke direktori client
cd ../client

# Install dependensi
npm install

# Salin file .env.example menjadi .env
cp .env.example .env

# Sesuaikan variabel di dalam file .env jika diperlukan (misalnya URL API)

# Jalankan server frontend
npm run dev
Selesai!

Aplikasi frontend akan berjalan di http://localhost:5173 (atau port lain yang tersedia).

API backend akan berjalan di http://localhost:3000 (atau port yang Anda atur di .env).

📄 Variabel Lingkungan (.env)
Pastikan Anda membuat file .env di dalam folder /server dan /client berdasarkan contoh .env.example yang tersedia.

Contoh /server/.env:

PORT=3000
DATABASE_URL="mysql://USER:PASSWORD@HOST:PORT/DATABASE_NAME"
# Tambahkan variabel lain seperti kunci API Genkit di sini
Contoh /client/.env:

VITE_API_BASE_URL="http://localhost:3000/api/v1"
🤝 Kontribusi
Kontribusi Anda sangat kami hargai! Jika Anda ingin berkontribusi, silakan ikuti langkah-langkah berikut:

Fork repositori ini.

Buat Branch baru (git checkout -b fitur/NamaFiturAnda).

Lakukan perubahan dan Commit (git commit -m 'feat: Menambahkan fitur X').

Push ke Branch Anda (git push origin fitur/NamaFiturAnda).

Buka Pull Request.

📜 Lisensi
Proyek ini dilisensikan di bawah Lisensi MIT. Lihat file LICENSE untuk detail lebih lanjut.