### Membuat Website Sederhana Dengan Integrasi Ke Database Menggunakan PHP

Ini adalah tugas untuk membuat dan mengimplementasikan website CRUD  untuk melakukan pengisian biodata diri siswa dengan menggunakan bahasa PHP dan XAMPP. User dapat menambahkan, menghapus, mengedit biodata siswa dalam tampilan website yang terkoneksi dengan database phpMyAdmin dengan http://localhost/pendaftaran_siswa/

### Langkah - Langkah Yang Dilakukan :
1. Buat sebuah sistem database dalam localhost/phpmyadmin dengan nama pendaftaran_siswa. Masukkan query dalam phpmyadmin sebagai berikut 

```R
  CREATE DATABASE `pendaftaran_siswa`;
``` 

2. Lalu buat tabel dalam database pendaftaran_siswa dengan memasukkan table dengan nama calon_siswa dengan query sebagai berikut

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

3. Masukkan data siswa untuk mengetahui apakah data sudah masuk ke dalam database atau belum pada tabel calon_siswa dengan query sebagai berikut

```R
  INSERT INTO `calon_siswa` (`id`, `nama`, `alamat`, `jenis_kelamin`, `agama`, `sekolah_asal`) VALUES (NULL, 'Tio', 'Jl. Mulyosari Mas No.C8', 'laki-laki', 'Islam', 'SMPN Al-Ummah Jombang');
``` 

4. Buatlah folder baru dalam direktory C:\xampp\htdocs dengan nama pendaftaran_siswa dan jalankan pada localhost/pendaftaran_siswa

### Hasil dari program akan seperti berikut 

1. Hasil Utama Program
![image](https://github.com/tiostwn/PWEB-CRUD-Siswa/assets/53292102/02f9379f-8fc2-41da-b66e-7462255de43b)

2. Melakukan Pendaftaran Baru
![image](https://github.com/tiostwn/PWEB-CRUD-Siswa/assets/53292102/2309e581-8361-4c21-81c9-5a5896e3630c)


3. Tampilan Data Siswa Beserta Data Yang Baru Saja Dimasukkan
![image](https://github.com/tiostwn/PWEB-CRUD-Siswa/assets/53292102/d870449c-9e89-4648-97dd-8bd8735c6ae2)

3. Melakukan Proses Edit Data
![image](https://github.com/tiostwn/PWEB-CRUD-Siswa/assets/53292102/6e0372c3-bf1f-4f52-a799-c2d17b8d164a)


