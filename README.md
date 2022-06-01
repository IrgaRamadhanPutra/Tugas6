# Tugas6
Nama  : Irga Ramadhan putra

Kelas : 312010067

NIM   : 312010067

Matkul: Sistem Basis Data

- Masuk ke databse nama_nim


![image](https://user-images.githubusercontent.com/101645216/170992801-6075e5f5-54f9-4663-a8a1-ab378d350320.png)


- Lakukan proses backup dan recovery dengan sql dari database tugas seblumnya !

Backup

![image](https://user-images.githubusercontent.com/101645216/170992962-0ca0b726-7c4f-41ae-a84b-8f4bab08e25c.png)


Jika proses backup berhasil maka akan muncul file backuppada direktori C:\xampp\mysql\data\nama database


![image](https://user-images.githubusercontent.com/101645216/170993067-fa33a8c9-4247-409e-b863-852bcc5ff874.png)


Recovery

Data yang telah di-backup dapat dikembalikan kapan saja bila diperlukan. Sintaks SQL yang digunakan adalah LOAD DATA INFILE. Perintah yang dijalankan adalah 

LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ; 


![image](https://user-images.githubusercontent.com/101645216/170994707-ed5bde88-54cc-4b02-8ccb-5eea7ae3a0b4.png)


![image](https://user-images.githubusercontent.com/101645216/171398353-2744b7de-96f2-4890-8da1-d950f88955a5.png)


![image](https://user-images.githubusercontent.com/101645216/170995424-842b12cb-3cd1-434f-9bb9-85e01895f55a.png)

-  Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnya !

![image](https://user-images.githubusercontent.com/101645216/170997325-319b3249-850e-4055-b679-a9d247d8ee7e.png)


![image](https://user-images.githubusercontent.com/101645216/170997419-0ecd89c0-a660-46ac-b719-1b8dba430afb.png)


- Tulisakan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !

crontab –e

00**7myqldump -u root -p irga_312010067>irga_312010067_backup.sql
