# Aplikasi Web "Mahara"
<h1 align = "center"><img src = "https://mahara.org/theme/mahara-org/images/site-logo.svg?v=3775"></h1>

[Sekilas Tentang](#sekilas-tentang) | [Instalasi](#instalasi) | [Konfigurasi](#konfigurasi) | [Otomatisasi](#otomatisasi) | [Cara Pemakaian](#cara-pemakaian) | [Pembahasan](#pembahasan) | [Referensi](#referensi)
:---:|:---:|:---:|:---:|:---:|:---:|:---:

## Sekilas Tentang
[`^Back to top^`](#)<br>
**Mahara** adalah salah satu *electronic portfolio management system*, aplikasi web ini bersifat gratis dan *open source*. Berdasarkan *website* resminya pada Mahara ini pengguna dapat mengunggah file, membuat jurnal, menyematkan sumber daya media sosial dari web serta berkolaborasi dengan pengguna lain dalam kelompok. Mahara mengabungkan antara dua hal yaitu *ePortfolio* dan sistem *social networking*. Mahara dikembangkan sejak 2006 sebagai suatu proyek kolaborasi antara *Massey University, Auckland University of Technology, The Open Polytechnic of New Zealand* dan *Victoria University of Wellington*, yang didanai oleh komisi pendidikan Selandia Baru.

## Instalasi
[`^Back to top^`](#)

#### Kebutuhan Sistem :
- Server OS: Debian GNU/ Linux Debian GNU/Linux (semua versi mulai dar 6/"Squeeze"), Ubuntu GNU/Linux, semua versi mulai dari 12.04/"Lucid Lynx".
- Web Server : Apache, semua versi mulai dari versi 2.
- Database Server : PostgreSQL (semua versi mulai dari 9.1), MySQL (semua versi mulai dari 5.1)
- PHP : minimal versi 7
- Memory : minimal 256 MB, direkomendasikan 1 GB.

#### Proses Instalasi :
1. 

## Konfigurasi (opsional)
[`^Back to top^`](#)

- 
- batas memori
- dll


## Otomatisasi
[`^Back to top^`](#)<br>
Selain dapat diinstall melalui server ubuntu, mahara juga dapat diinstall di windows menggunakan XAMPP. Berikut cara install nya.
1. Kunjungi website https://mahara.org/
2. Pada halaman home, klik download mahara
3. Download file .zip 
4. Extract file mahara-19.10.2.zip
5. Setelah diextract, di dalam folder tersebut terdapat folder htdocs. Masuk ke dalam folder tersebut, copy semua file yang ada di sana.
6. Masuk ke directory di mana XAMPP di install, biasanya ada di **C:\xampp\htdocs**
7. Di dalam folder htdocs xampp tersebut, buatlah folder baru dengan nama mahara, kemudian paste (CTRL + V) semua file ke folder ini.
8. Buka XAMPP, start Apache dan MySQL
9. Buka http://localhost/phpmyadmin/ di browser
10. Pada phpmyadmin, buat database baru dengan nama db_mahara, penyortiran utf8_bin
11. Cari file config-dist.php di folder mahara yang dibuat tadi
12. Duplikat file ini dengan nama config.php
13. Edit file config.php, sehingga menjadi seperti berikut :
```
      $cfg->dbtype   = 'mysql5';
      $cfg->dbhost   = 'localhost';
      $cfg->dbport   = null; 
      $cfg->dbname   = 'db_mahara';
      $cfg->dbuser   = 'root';
      $cfg->dbpass   = '';
```
14. Setelah itu buka http://localhost/mahara/ di browser
15. Akan muncul perintah install, lakukan instalasi sampai selesai
16. Setelah itu, masukkan password baru dan alamat email
    Catatan : password harus kombinasi huruf, angka, dan simbol dengan panjang minimal 8 karakter
17. Setelah sub,it, maka aplikasi mahara telah terinstal
    

Skrip shell untuk otomatisasi instalasi, konfigurasi, dan maintenance.


## Cara Pemakaian
[`^Back to top^`](#)
Berikut ini cara pemakaian web server Mahara:
1. 

- Tampilan aplikasi web
- Fungsi-fungsi utama
- Isi dengan data real/dummy (jangan kosongan) dan sertakan beberapa screenshot


## Pembahasan
[`^Back to top^`](#)

- Pendapat anda tentang aplikasi web ini

**Kelebihan**
- Mendukung integrasi dengan web server lain, contohnya moodle
- Mudah untuk melakukan sharing dan kolaborasi dengan orang lain

**Kekurangan**
- Bahasa yang tersedia masih belum terlalu banyak, termasuk bahasa Indoneia.


## Referensi
[`Back to top`](#)
1. [About Mahara](https://mahara.org/) - Mahara
2. [System Administrator's Guide/Upgrading Mahara](https://wiki.mahara.org/wiki/System_Administrator%27s_Guide/Upgrading_Mahara) - Upgrading Mahara
3. [System Administrator's Guide/Installing Mahara](https://wiki.mahara.org/wiki/System_Administrator%27s_Guide/Installing_Mahara) - Installing Mahara
4. [Mahara online user manual](https://manual.mahara.org) - Mahara
5. [Install mahara menggunakan XAMPP](https://ilmukomputer.org/wp-content/uploads/2010/05/Mudafiq-InstalasiMaharaDiWindows.pdf)
