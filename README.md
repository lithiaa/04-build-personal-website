## Laporan Praktikum

|  | Pemrograman Berbasis Framework 2025 |
|--|--|
| NIM |  2241720217|
| Nama |  Muhammad Bagus Indrawan |
| Kelas | TI - 3A |

## Langkah-langkah Praktikum 
### 1. Persiapan Lingkungan 
1. Pastikan Node.js dan npm sudah terinstal di komputer Anda. Anda dapat memeriksanya dengan 
menjalankan perintah berikut di terminal atau command prompt: 
node -v 
npm -v 

2. Buat direktori baru untuk proyek Next.js Anda: 
mkdir website-pribadi 
cd website-pribadi 

3. Inisialisasi proyek Next.js dengan TypeScript dan App Router: 
npx create-next-app@latest . --typescript –app 

4. Cek konfigurasi postcss.config.mjs: 
![alt text](image-3.png)

5. Cek di app/globals.css, sudah ada import untuk tailwindcss: 
![alt text](image-2.png)

6. Buka app/layout.tsx, tambahkan import './globals.css', dan modifikasi menjadi sebagai berikut: 
![alt text](image-1.png)

7. Jalankan aplikasi Next.js: 
npm run dev 
Aplikasi akan terbuka di browser pada alamat http://localhost:3000.

![alt text](image.png)

## 2. Membuat Halaman Website 

1. Buat file app/page.tsx sebagai halaman "Tentang Saya": 
![alt text](image-7.png)
2. Buat file app/projects/page.tsx sebagai halaman "Proyek": 
![alt text](image-8.png)
3. Buat file app/essays/page.tsx sebagai halaman "Esai": 
![alt text](image-9.png)
4. Buka browser dan akses: 
- http://localhost:3000/ untuk halaman "Tentang Saya". 
![alt text](image-4.png)
- http://localhost:3000/projects untuk halaman "Proyek". 
![alt text](image-5.png)
- http://localhost:3000/essays untuk halaman "Esai".
![alt text](image-6.png)
