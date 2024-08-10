Tutorial Cara Buka Projek KP Invoice

1. Download XAMPP
2. Donwload Composer: https://getcomposer.org/download/
"Download and run Composer-Setup.exe - it will install the latest composer version whenever it is executed."
Jika sudah cek versi Composer "composer --version" di CMD
3. Cara masuk CMD Win -> Tulis "CMD" / Ctrl + R -> Tulis "CMD" ketik "composer --version" di CMD
4. Buka Projek Laravel -> Agar cepat yang tidak perlu Zip Download file Repository ini: https://github.com/percivalyan/laravel-invoice-print 
Masuk ke "<> Code" yang warna hijau lalu "Download Zip"
5. Masuk ke CMD lagi (Cara masuk CMD Win -> Tulis "CMD" / Ctrl + R -> Tulis "CMD") -> ketika composer install (jika tidak bisa composer update, tapi coba install dulu)
6. Lalu klik cd laravel-invoice-print di CMD
7. Jika pakai Visual Code Studio, klik "code ." nanti langsung masuk ke VSC
8. Kembali ke CMD atau pakai Terminal VSC (opsional), lalu ketika
   a. copy .env.example .env (kalo tidak bisa pakai "cp .env.example .env")
   b. php artisan key:generate
9. Masuk ke ".env", lihat di projek laravel-invoice-print
10. Ubah bagian ini menjadi seperti ini:
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=laravel_invoice_excel_td
    DB_USERNAME=root
    DB_PASSWORD=

    "Biasanya dikomentari, buka komentar lalu ketik atau replace"
11. Masuk ke localhost di browser
12. Lalu buat nama database "laravel_invoice_excel_td"
13. Kembali ke CMD atau Terminal Visual Code Studio, ketik "php artisan migrate"
14. Lalu jika tidak ada error, ketik "php artisan serve"
15. Buka "http://127.0.0.1:8000/" di browser, jika bisa berarti berhasil

