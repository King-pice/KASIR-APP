Kasir Kafe - Aplikasi Kasir Modern untuk Kafe
Aplikasi kasir berbasis web yang dibangun dengan Next.js 15 dan TypeScript, dirancang khusus untuk kebutuhan kasir kafe dengan fitur lengkap dan responsif.

🚀 Fitur Utama
🔐 Sistem Keamanan Berlapis
Token Akses Ganda: Token khusus untuk owner dan pengguna
Sistem Login: Register dan login akun kasir
Role Management: Owner dapat mengubah token pengguna
💳 Kasir Lengkap
Menu Management: Pencarian dan filter menu berdasarkan kategori
Keranjang Belanja: Tambah, kurangi, dan custom pesanan
Catatan Pesanan: Tambahkan catatan khusus (pedas, asin, dll)
Nomor Meja: Opsional untuk dine-in atau take-away
Variasi Produk: Support variasi seperti Hot/Ice
📋 Manajemen Pesanan
Simpan Pesanan: Simpan pesanan untuk diproses nanti
Riwayat Transaksi: Lihat semua transaksi yang telah selesai
Refund: Proses refund untuk pesanan yang bermasalah
Cetak Struk: Cetak struk untuk setiap transaksi
📊 Laporan Penjualan
Laporan Harian: Ringkasan penjualan hari ini
Laporan Bulanan: Statistik penjualan per bulan
Laporan Tahunan: Overview penjualan tahunan
Auto Standby: Update otomatis sesuai periode
🛍️ Kelola Produk
CRUD Produk: Tambah, edit, dan hapus produk
Kategori: Organisir produk berdasarkan kategori
Variasi Produk: Tambahkan variasi dengan harga berbeda
Harga Dinamis: Atur harga untuk setiap variasi
⚙️ Pengaturan Lengkap
Custom Struk: Atur header, footer, dan tampilan struk
Ukuran Kertas: Support 58mm dan 80mm thermal print
Pengaturan PPN: Atur tarif pajak dan aktifkan PPN
Manajemen Akun: Ubah password dan informasi akun
📱 Responsif & Multi-Device
Mobile-First: Desain optimal untuk smartphone
Tablet Friendly: Tampilan sempurna di tablet
Desktop Mode: Interface lengkap untuk desktop
Touch-Friendly: Interface yang mudah digunakan dengan sentuhan
🛠️ Teknologi
Frontend
Next.js 15: Framework React dengan App Router
TypeScript 5: Type safety dan better DX
Tailwind CSS 4: Styling modern dan responsif
shadcn/ui: Component library yang konsisten
Lucide Icons: Icon set yang modern
Backend & Database
Prisma ORM: Database management yang modern
SQLite: Database lokal yang ringan
API Routes: RESTful API dengan Next.js
Development Tools
ESLint: Code quality dan consistency
TypeScript: Static type checking
Hot Reload: Development experience yang cepat
🚀 Quick Start
Prerequisites
Node.js 18+
npm atau yarn
Installation
Clone repository
bash

Line Wrapping

Collapse
Copy
1
2
git clone <repository-url>
cd kasir-kafe
Install dependencies
bash

Line Wrapping

Collapse
Copy
1
npm install
Setup database
bash

Line Wrapping

Collapse
Copy
1
npm run db:push
Run development server
bash

Line Wrapping

Collapse
Copy
1
npm run dev
Buka browser
Navigate ke http://localhost:3000
📖 Cara Penggunaan
1. Setup Awal
Buka halaman utama untuk generate token
Generate Token Owner untuk akses penuh
Generate Token Pengguna untuk akses kasir
Owner dapat mengubah token pengguna kapan saja
2. Login Akun
Masukkan token akses yang telah dibuat
Register akun kasir baru atau login dengan akun existing
Setelah login, Anda akan diarahkan ke dashboard
3. Menggunakan Kasir
Pilih Menu: Cari atau filter menu yang diinginkan
Tambah ke Keranjang: Klik tombol tambah pada menu
Custom Pesanan: Tambahkan catatan khusus jika needed
Nomor Meja: Opsional, isi untuk pesanan dine-in
Proses: Klik "Proses Pesanan" untuk menyelesaikan transaksi
4. Kelola Produk
Buka menu "Kelola Produk"
Tambah kategori baru jika needed
Tambah produk dengan nama, harga, dan kategori
Tambahkan variasi (Hot/Ice) jika diperlukan
5. Pengaturan Struk
Buka menu "Pengaturan" → "Struk"
Custom header dan footer struk
Pilih ukuran kertas (58mm/80mm)
Atur PPN jika diperlukan
Cetak test struk untuk preview
📁 Struktur Proyek

Line Wrapping

Collapse
Copy
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
kasir-kafe/
├── src/
│   ├── app/                 # Next.js App Router
│   │   ├── api/            # API Routes
│   │   ├── dashboard/      # Main Dashboard
│   │   ├── login/          # Login Page
│   │   └── page.tsx        # Token Page
│   ├── components/         # React Components
│   │   ├── ui/            # shadcn/ui Components
│   │   ├── ProductManager.tsx
│   │   └── Settings.tsx
│   └── lib/               # Utilities
│       └── db.ts          # Prisma Client
├── prisma/
│   └── schema.prisma      # Database Schema
├── public/                # Static Assets
└── README.md
🔧 Environment Variables
Buat file .env.local di root directory:

env

Line Wrapping

Collapse
Copy
1
DATABASE_URL="file:./dev.db"
📝 Database Schema
Aplikasi menggunakan database SQLite dengan schema berikut:

Users: Manajemen akun pengguna
Categories: Kategori produk
Products: Data produk dan harga
Variations: Variasi produk (Hot/Ice)
Orders: Data transaksi
OrderItems: Detail item pesanan
Settings: Pengaturan sistem
🚀 Deployment
Vercel (Recommended)
Push ke GitHub
Connect repository ke Vercel
Setup environment variables
Deploy
Self-Hosted
Build aplikasi: npm run build
Start production: npm start
Setup reverse proxy (nginx/apache)
🤝 Contributing
Fork repository
Create feature branch: git checkout -b feature/amazing-feature
Commit changes: git commit -m 'Add amazing feature'
Push ke branch: git push origin feature/amazing-feature
Open Pull Request
📄 License
MIT License - lihat file LICENSE untuk detail

🆘 Support
Jika mengalami masalah atau memiliki pertanyaan:

Cek Issues untuk masalah yang sudah dilaporkan
Buat issue baru dengan detail yang lengkap
Sertakan screenshot dan error message jika ada
🔄 Update & Maintenance
Regular Updates: Update dependencies secara berkala
Database Backup: Backup database SQLite secara rutin
Security Review: Review keamanan secara berkala
🌟 Features yang Akan Datang
 Payment Gateway Integration
 SMS/WhatsApp Notifications
 Advanced Analytics
 Multi-Location Support
 Inventory Management
 Customer Loyalty Program
Dibuat dengan ❤️ menggunakan Next.js 15 dan TypeScript
