Logistics Management Service

 Proyek ini adalah API Layanan Manajemen Logistik yang dibangun menggunakan Express.js dan PostgreSQL. Layanan ini mengintegrasikan autentikasi dari Authentication & User Management Service menggunakan JWT. API ini menyediakan endpoint untuk mengelola pengiriman barang, termasuk membuat, memperbarui, melacak pengiriman, dan mengambil data pengiriman yang terkait dengan pengguna yang sedang masuk.

Fitur
Layanan Autentikasi & Manajemen Pengguna
1.	Registrasi: Memungkinkan pengguna baru (admin dan pengguna reguler) untuk mendaftar.
2.	Login: Memungkinkan pengguna untuk masuk dan menerima token JWT.
3.	Profil Pengguna: Memungkinkan pengguna yang telah masuk untuk mengambil informasi profil mereka.
Layanan Manajemen Logistik
1.	Membuat Pengiriman: Memungkinkan admin untuk membuat pengiriman baru.
2.	Memperbarui Status Pengiriman: Memungkinkan admin memperbarui status pengiriman (contoh: dari "Dikirim" menjadi "Terkirim").
3.	Menghapus data pengiriman: Menghapus data pengiriman dari data yang di pilih
4.	Mengambil Data Pengiriman: Mengambil semua data pengiriman yang terkait dengan pengguna yang sedang masuk (baik sebagai pengirim atau penerima).
Prasyarat
1.	Node.js (versi 15 atau lebih baru)
2.	MongoDB (Pastikan Anda memiliki instance Mongodb/MongoDBCompass yang berjalan)
3.	NPM (Sudah termasuk dalam Node.js)
4.	Axios (Untuk integrasi API antara layanan)
Instalation
1. Clone both repositories: - **Authentication & User Management Service** - **Logistics Management Service** 
bash
   git clone https://github.com/yourusername/auth-service.git
   git clone https://github.com/yourusername/logistics-service.git

2.  Install dependencies for each service:

    - cd auth-service
    - npm install

    - cd ../logistics-service
    - npm install
## Pengujian dengan Postman
1.	Gunakan Postman untuk mengirim permintaan ke layanan ini.
2.	Untuk permintaan yang memerlukan autentikasi, sertakan token JWT di header Authorization dengan format:
Bearer <token>.
3.	Uji berbagai endpoint berikut:
o	Registrasi pengguna baru
o	Login dan dapatkan token JWT
o	Membuat pengiriman baru (hanya untuk admin)
o	Mengupdate pengiriman
o	Mengambil semua data pengiriman yang terkait dengan pengguna yang masuk
Penjelasan:
1.	Features menjelaskan fitur-fitur yang tersedia dalam kedua layanan, yaitu Authentication & User Management Service dan Logistics Management Service.
2.	Installation memberikan panduan langkah demi langkah untuk mengkloning repositori, menginstal dependensi yang dibutuhkan, dan menjalankan proyek.
3.	Testing with Postman memberikan panduan untuk menguji API menggunakan Postman, termasuk cara autentikasi dengan JWT token dan pengujian endpoint API.
4.	API Documentation menyediakan akses ke dokumentasi API melalui Swagger, sehingga memudahkan pengguna memahami dan menguji setiap endpoint.
