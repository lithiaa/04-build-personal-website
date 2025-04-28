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

## 3. Membuat Layout dan Navigasi

1. Buat direktori src/components jika belum ada. 
2. Buat file src/components/Layout.tsx 
![alt text](image-10.png)
3. Buat file src/components/Navbar.tsx
![alt text](image-11.png)
4. Buat file src/components/Footer.tsx
![alt text](image-12.png)
5. Update file app/layout.tsx untuk menggunakan layout
![alt text](image-13.png)
6. Update setiap halaman menambahkan metadata dengan generateMetadata
![alt text](image-14.png)
![alt text](image-19.png)
Lakukan hal yang sama untuk halaman projects/page.tsx dan essays/page.tsx. 
![alt text](image-15.png)
![alt text](image-17.png)

![alt text](image-16.png)
![alt text](image-18.png)

## 4. Membuat Halaman Proyek dengan Grid Responsif 

1. Buat folder di public/images. Kemudian tambahkan dua image, lalu rename dengan nama 
project1.png dan project2.png 
![alt text](image-20.png)

2. Modifikasi file app/projects/page.tsx: 
Tambahkan import next/image dan beberapa image yang telah ditambahkan sebelumnya 
![alt text](image-21.png)
Buat card project item sebagai berikut: 
![alt text](image-22.png)

Modifikasi komponen project sebagai berikut: 
![alt text](image-23.png)

3. Simpan file dan buka http://localhost:3000/projects di browser. Anda akan melihat daftar proyek 
dalam grid yang responsif.
![alt text](image-24.png)