## LOGIN BENDER

Revalina Fairuzy Azhari Putri / 5027231001

Source: https://demo.owasp-juice.shop/#/score-board?categories=Injection

**Langkah-langkah:**

1. Dalam *case* ini kita diminta untuk masuk ke dalam sistem sebagai Bender. Dengan menggunakan teknik OSINT, kita bisa mencari nama email dari Bender, dan terbukti dapat ditemukan di kumpulan kolom *review*.

Setelah mendapatkan *email name* dari Bender, kita ketikkan pada section yang ada. Dengan menggunakan SQL Injection, kita akan memberikan command untuk mencoba melakukan *bypass* pada akun bender, dengan mengetikkan bender@juice-sh.op'--
![alt text](images/image-4.png)

2. Kita bisa masukkan *password* bebas pada *section* yang tersedia.
![alt text](images/image-5.png)

3. Kita berhasil masuk sebagai Bender disini, terbukti dari tampilan pada *login button* yang ada, tertampil *email* dari Bender.
![alt text](images/image-6.png)

Dari hasil di atas, maka diketahui 

- Hasil: Berhasil

- Alasan: Login sebagai Bender berhasil karena kombinasi teknik OSINT (mencari alamat email target dari kolom review) dan SQL Injection (bender@juice-sh.op'--) membuat query SQL yang dijalankan mengabaikan bagian password. Dengan begitu, sistem langsung menerima login menggunakan email Bender.

- Refleksi: Percobaan ini menegaskan bahwa serangan sering kali tidak hanya mengandalkan eksploitasi teknis, tetapi juga informasi yang tersedia secara publik (OSINT). Jika aplikasi tidak mengamankan input dengan baik, maka data yang sudah terekspos dapat dimanfaatkan untuk akses tidak sah.