# PWeb_PHP
## Membuat Website Sederhana Dengan Integrasi Ke Database Menggunakan PHP

## Ini adalah tugas untuk membuat dan mengimplementasikan website CRUD  untuk melakukan pengisian biodata diri siswa dengan menggunakan bahasa PHP dan XAMPP. User dapat menambahkan, menghapus, mengedit biodata siswa dalam tampilan website yang terkoneksi dengan database phpMyAdmin dengan http://localhost/pendaftaran_siswa/

## Langkah - Langkah Yang Dilakukan :
## 1. Buat sebuah sistem database dalam localhost/phpmyadmin dengan nama pendaftaran_siswa. Masukkan query dalam phpmyadmin sebagai berikut 

```R
  CREATE DATABASE `pendaftaran_siswa`;
``` 

## 2. Lalu buat tabel dalam database pendaftaran_siswa dengan memasukkan table dengan nama calon_siswa dengan query sebagai berikut

```R
  CREATE TABLE `pendaftaran_siswa`.`calon_siswa` (
    `id` INT NOT NULL AUTO_INCREMENT ,  
    `nama` VARCHAR(64) NOT NULL ,  
    `alamat` VARCHAR(255) NOT NULL ,  
    `jenis_kelamin` VARCHAR(16) NOT NULL ,  
    `agama` VARCHAR(16) NOT NULL ,  
    `sekolah_asal` VARCHAR(64) NOT NULL ,    
    PRIMARY KEY  (`id`)
) ENGINE = InnoDB;
``` 

## 3. Masukkan data siswa untuk mengetahui apakah data sudah masuk ke dalam database atau belum pada tabel calon_siswa dengan query sebagai berikut

```R
  INSERT INTO `calon_siswa` (`id`, `nama`, `alamat`, `jenis_kelamin`, `agama`, `sekolah_asal`) VALUES (NULL, 'Tio', 'Jl. Mulyosari Mas No.C8', 'laki-laki', 'Islam', 'SMPN Al-Ummah Jombang');
``` 

## 4. Buatlah folder baru dalam direktory C:\xampp\htdocs dengan nama pendaftaran_siswa dan jalankan pada localhost/pendaftaran_siswa

## Hasil dari program akan seperti berikut 

### 1. Hasil Utama Program
![First](images/halaman_utama.png)

### 2. Melakukan Pendaftaran Baru
![Second](images/daftar.png)

### 3. Tampilan Data Siswa Beserta Data Yang Baru Saja Dimasukkan
![Third](images/database.png)

### 3. Melakukan Proses Edit Data
![Four](images/edit.png)

### 3. Melakukan Proses Hapus Data
![Five](images/hapus.png)
