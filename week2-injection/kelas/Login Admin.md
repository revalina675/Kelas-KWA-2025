## LOGIN ADMIN

Revalina Fairuzy Azhari Putri / 5027231001

Source: 

**Langkah-langkah:**

1. Masuk ke section login pada web OWASP Juice Shop. Disini kita diminta untuk masuk ke sistem sebagai admin.
![alt text](images/image.png)

2. Pada *case* ini kita akan menggunakan pola SQL Injection. Kita coba dengan menggunakan "OR true--".
![alt text](images/image-1.png)

3. Kita masukkan password bebas dengan kombinasi yang tidak ditentukan.
![alt text](images/image-2.png)

4. Kita telah berhasil masuk sebagai admin ke dalam sistem, terbukti saat kita klik *login button*, akan tertampil email admin sebagai *default* kita (admin@juice-sh.op)
![alt text](images/image-3.png)