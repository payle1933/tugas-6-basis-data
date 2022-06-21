# TUGAS-6-SISTEM-BASIS-DATA
```
Nama	Maulana Hasanudin
NIM	312010106
Kelas	TI.20.D.1
```
# LANGKAH - LANGKAH TUGAS 6 SISTEM BASIS DATA TI.20.D1
# 1. Masuk Ke Database Nama_nim
<img width="430" alt="msk database tugas 6" src="https://user-images.githubusercontent.com/101716660/174850656-8329fbf6-11ce-4e9f-8f1f-8c3fbf291120.png">


# 2. Lakukan proses Backup Dengan Sql Dari Database Tugas Sebelumnya !
<img width="465" alt="bck up database tugas 6" src="https://user-images.githubusercontent.com/101716660/174850723-e4f6d5b6-1d2f-4fe4-8532-f06f5fcaef49.png">

# 3. Jika Proses Berhasil Maka Akan Muncul File Backup Pada Direktori C:\xampp\mysql\data\nama database
<img width="1070" alt="hasil_backup" src="https://user-images.githubusercontent.com/101716660/174850782-a85f4ce2-c234-439b-bd74-7ed7c171058e.png">


# 4. Recovery
Data Yang Telah Di-Backup Dapat Dikembalikan Kapan Saja Bila Diperlukan. Sintaks SQL Yang Digunakan Adalah LOAD DATA INFILE. Perintah Yang Dijalankan Adalah :

# LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ;
<img width="407" alt="load data tugas 6" src="https://user-images.githubusercontent.com/101716660/174850840-c552daa8-05fa-4c15-83da-ef93c75203a7.png">


# 5. Lakukan Proses Backup dan Recovery Dengan Sqldump Dari Database Tugas Sebelumnya !
![back up 5 tugas 6](https://user-images.githubusercontent.com/101716660/174851095-0b97b200-15ac-4b1d-a6d1-4e0a917c4266.png)

# 6. Tulisakan Script Cron Job Untuk Melakukan Backup Otomatis Setiap Hari Minggu Jam 12 Malam !
Crontab –e

00**7myqldump -u Adminklinik1 -p klinnik_312010106>backuptugaske6.sql
