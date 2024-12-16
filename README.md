# Final-Project-Os-Server-23TK02-23.83.1036
**Nama:** Ariiq Hafizh  
**NIM:** 23.83.1036  
**Kelas:** 23TK02  
**Mata Kuliah:** OS SERVER dan SISTEM ADMIN 
Progres 1 : Minggu 1 Des 2024 Penentuan judul website Coffe Shop

## Daftar Isi
1. [Instalasi OPEN SSH SERVER](#1-instalasi-open-ssh-server)
2. [Instalasi MYSQL SERVER](#2-instalasi-mysql-server)
3. [Instalasi APACHE2](#3-instalasi-apache2)
4. [Instalasi DATABASE SERVER](#4-instalasi-database-server)
5. [Instalasi FAIL2BAN](#5-instalasi-fail2ban)


## 1.Instalasi OPEN SSH SERVER
**Langkah 1:** Lakukan Instalasi Paket SSH Server
```bash
sudo apt install openssh-server -y
```
**Langkah 2:** Mengaktifkan Layanan ssh server
```bash
sudo systemctl enable ssh
```
**Langkah 3:** Memulai Layanan SSH SERVER
```bash
sudo systemctl start ssh
```
**Langkah 4:** Cek ip ubuntu server
```bash
ip a
```
**Langkah 5:** Cek status ubuntu server
```bash
sudo systemctl status ssh
```
**Langkah 6:** config ssh server
```bash
Buka CMD pada windows,lakukan konfigurasi pada ubuntu dengan cara <ssh username ubuntu@ip address ubuntu server> contoh:ssh hilmiserver@192.168.1.3
setelah itu ketik manual "yes" dan masukkan password ubuntu server
```
![Screenshot 2024-12-01 162253](https://github.com/user-attachments/assets/6c07cc9e-b9a9-42cc-ac4d-c2944f85a11e)


## 2.Installasi MY-SQL SERVER
**Langkah 1:** Install mysql server dengan perintah
```bash
sudo apt install mysql-server -y
```
**Langkah 2:** Install tumpukan LAMP (Linux, Apache, MySQL, PHP) pada sistem operasi dengan perintah
```bash
sudo apt install php libapache2-mod-php phpmysql
```
**Langkah 3:** Membuka File Konfigurasi Direktori Apache dengan perintah
```bash
sudo nano /etc/apache2/mods-enabled/dir.conf
```
**Langkah 4:** Membuka file bernama “info.php” pada direktori var/www/html
```bash
sudo nano /var/www/html/info.php
```
-isikan dengan code dibawah
```bash
<?php

phpinfo ();

?>
```
**Langkah 5:** cek configurasi

contoh :192.168.1.13/info.php
![Screenshot 2024-12-01 162919](https://github.com/user-attachments/assets/0bfbfc72-f180-4414-90bf-4aad8b833412)

## 3.Installasi APACHE2
**Langkah 1:** Perbarui daftar paket dengan perintah
```bash
sudo apt update
```
**Langkah 2:** Installasi apache 2 dengan perintah
```bash
sudo apt install apache2 -y
```
**Langkah 3:** Memulai layanan server apahe2 dengan perintah
```bash
sudo systemctl start apache2
```
**Langkah 4:** Lakukan pengecekan ip addres ubuntu server dengan perintah
```bash
ip a
```
**Langkah 5:** Buka pada browser google chrome pada windows dan ketikkan ip addres tadi “192.168.1.13”


contoh ip saya : 192.168.1.13
![Screenshot 2024-12-01 163131](https://github.com/user-attachments/assets/aeeb7b73-f217-466d-aeef-7102390b68f6)

## 4.Installasi DATABASE SERVER
**Langkah 1:** Installasi paket mariadb
```bash
sudo apt update
```
**Langkah 2:** Untuk mengamankan installasi pilihan
```bash
sudo apt install apache2 -y
```
**Langkah 3:** Lakukan instalasi paket
![Screenshot 2024-12-01 163243](https://github.com/user-attachments/assets/b76c67db-137c-496f-a956-bfea6eef03cb)
![Screenshot 2024-12-01 163503](https://github.com/user-attachments/assets/5d17d87f-fb12-4e77-a1ba-ac711a32b41a)
![Screenshot 2024-12-01 163541](https://github.com/user-attachments/assets/4cb885c4-d2b8-4ada-ad8d-a383d59a13f4)
![Screenshot 2024-12-01 163557](https://github.com/user-attachments/assets/fe008325-bab0-4584-b228-5378e09bec08)

```bash
sudo systemctl start apache2
```
**Langkah 4:** Restart ulang layanan
```bash
ip a
```
**Langkah 5:** CEK KONFIGURASI Buka pada browser windows gogole chrome dan ketikkan <ip address ubuntu server/phpmyadmin/> cth:192.168.1.13/phpmyadmin/
![Screenshot 2024-12-01 171808](https://github.com/user-attachments/assets/6e3ae4ed-e01b-480e-8393-77a8f9e8b7cd)

## 5.Installasi fail2bn
**Langkah 1:** Instalasi fail2ban
```bash
sudo apt install fail2ban -y
```
**Langkah 2:** nyalakan 
```bash
sudo systemctl enable fail2ban
```
**Langkah 3:** jalankan
```bash
sudo systemctl start fail2ban
```
**Langkah 4:** check status
```bash
sudo systecmtl status fail2ban
```
![Screenshot 2024-12-15 205603](https://github.com/user-attachments/assets/b034640c-b2fe-45f3-a5aa-adf3cd050a50)


