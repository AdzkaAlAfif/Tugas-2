# Tugas-2

PERINTAH – PERINTAH DASAR SISTEM OPERASI LINUX


I.	Tujuan Praktikum


•	Mengenal format intruksi arsitektur sistem pada sistem operasi Linux


	Mempelajari Utilitas dasar pada sistem operasi Linux


	Menggunakan perintah – perintah dasar pada sistem operasi Linux


II.	Alat dan Bahan / Perangkat Lunak


•	Laptop dengan sistem operasi Windows.


•	Virtual Machine (VirtualBox.)


•	Ubuntu 14.04.6 LTS Desktop 64-bit (ISO).


III.	Dasar Teori

Linux yang pada dasarnya untuk menjalankan setiap service dengan menjalankan Command line atau baris perintah dalam lingkungan shell. Keuntungan menggunakan perintah di baris perintah adalah efektifitas dan maksimalitas kerja. Prompt dari shell bash pada linux menggunakan “$”. username@linux-PC:~$


Untuk sebuah sesi linux terdiri dari :


1.	Login


2.	Bekerja dengan shell atau menjalankan aplikasi

  
3.	Logout
Seperti halnya mengetik perintah di DOS, baris perintah di linux juga diketik di prompt yang ada di lingkungan shell dan diakhiri dengan enter untuk mengeksekusi perintah tersebut.

A.	Perintah – Perintah Dasar


<img width="446" height="143" alt="image" src="https://github.com/user-attachments/assets/b3343b32-1211-4a1c-a24d-1a8f7e87f3ef" />



  <img width="449" height="304" alt="image" src="https://github.com/user-attachments/assets/37755188-746d-4d25-94fd-69b7ca77994b" />
 
 


B.	Format Intruksi Linux


Intruksi linux standar mempunyai format sebagai berikut :


$ NamaInteruksi [Pilihan] [argument]


Pilihan adalah opsi yang dimulai dengan tanda – (minus). Argumen dapat kosong, satu atau beberapa argument (parameter). Contoh :

<img width="598" height="286" alt="image" src="https://github.com/user-attachments/assets/2bf0bc61-76a2-484f-8680-8d461765cc2c" />


Sistem operasi merupakan perangkat lunak yang mengelola sumber daya perangkat keras dan menyediakan layanan bagi aplikasi. Linux merupakan sistem operasi yang dapat digunakan melalui Command Line Interface (CLI) maupun Graphical User Interface (GUI). Ubuntu merupakan salah satu distribusi Linux yang menyediakan lingkungan desktop.


IV.	Langkah - Langkah Praktikum

1.	Hidupkan komputer


2.	Masuk ke sistem operasi linux

Tunggu sampai ada perintah login untuk mengisi nama user dan perintah password untuk mengisi password dari user.
 
•	Tampilan login dengan tampilan GUI,kemudian bukalah terminal

•	Tampilan login berupa command line tanpa GUI


3.	Untuk keluar dari system gunakan perintah Logout atau Exit


4.	Gunakan perintah – perintah untuk informasi user : Id, hostname, uname, w, who, whoami, chfn.


5.	Gunakan – perintah dasar (basic command): date, cal, man, clear, apropos, whatis

  
6.	Gunakan perintah – perintah dasar untuk manipulasi file : ls, file, cat, more, pg, cp, mv, rm, grep


V.	Latihan


Percobaan 1 : Melihat identitas diri (nomor id dan group id)
$ id
<img width="650" height="210" alt="image" src="https://github.com/user-attachments/assets/0c9f9095-a128-4a29-9481-2607ab1f370c" />


Percobaan 2 : Melihat tanggal dan kalender dari system
•	Melihat tanggal saat iniho
$ date
•	Melihat kalender
$ cal 10 2015
<img width="649" height="196" alt="image" src="https://github.com/user-attachments/assets/c25fb504-e68f-4cdf-958c-97446f5413ff" />


Percobaan 3 : Melihat identitas mesin
$ hostname
$ uname
$ uname -a
 <img width="751" height="161" alt="image" src="https://github.com/user-attachments/assets/1028755e-ec35-4f85-8861-80037de524f1" />

 

Percobaan 4 : Melihat siapa yang sedang aktif
•	Mengetahui siapa saja yang sedang aktif
$ w
$ who
$ whoami
•	Mengubah informasi finger
$ chfn mahasiswa
<img width="657" height="234" alt="image" src="https://github.com/user-attachments/assets/5cc4dcfb-9a8d-491a-b858-b2fb2886ac5c" />



Percobaan 5 : Menggunakan Manual
$ man ls
$ man man
$ man –k file
$ man 5 passwd
<img width="536" height="347" alt="image" src="https://github.com/user-attachments/assets/004a873a-729e-457a-9658-b89540c892d8" />

 
Percobaan 6 : Menghapus layar
$ clear


Percobaan 7 : Mencari perintah yang deskripsinya mengandung kata kunci yang dicari.
$ apropos date
$ apropos mail
$ apropos telnet


Percobaan 8 : Mencari perintah yang tepat sama dengan kunci yang dicari.
$ whatis date


Percobaan 9 : Manipulasi berkas (file) dan direktori
•	Menampilkan curent working directory
$ ls
•	Melihat semua file lengkap
$ ls –l
•	Menampilkan semua file atau direktori yang tersembunyi
$ ls –a
•	Menampilkan semua file atau direktori tanpa proses sorting
$ ls –f
•	Menampilkan isi suatu direktori
$ ls /usr
•	Menampilkan isi direktori root
$ ls /
•	Menampilkan semua file atau direktori dengan menandai : tanda (/) untuk direktori, tanda asterik (*) untuk file yang bersifat executable, tanda (@) untuk file symbolic link, tanda (=) untuk socket, tanda (%) untuk whiteout dan tanda (|) untuk FIFO.
$ ls –F /etc
•	Menampilkan file atau direktori secara lengkap yaitu terdiri dari nama file, ukuran, tanggal dimodifikasi, pemilik, group dan mode atau atributnya.
$ ls –l /etc
 
•	Menampilkan semua file dan isi direktori. Argumen ini akan menyebabkan proses berjalan agak lama, apabila proses akan dihentikan dapat menggunakan ^c
$ ls –R /usr


Percobaan 10 : Melihat tipe file
$ file
$ file *
$ file /bin/ls


Percobaan 11 : Menyalin file
•	Mengkopi suatu file. Berikan opsi –i untuk pertanyaan interaktif bila file sudah ada.
$ cp /etc/group f1
$ ls –l
$ cp –i f1 f2
$ cp –i f1 f2
•	Mengkopi ke direktori
$ mkdir backup
$ cp f1 f3
$ cp f1 f2 f3 backup
$ ls backup
$ cd backup
$ ls


Percobaan 12 : Melihat isi file
•	Menggunakan instruksi cat
$ cat f1
•	Menampilkan file per satu layar penuh
$ more f1


Percobaan 13 : Mengubah nama file
•	Menggunakan instruksi mv
 
$ mv f1 prog.txt
$ ls
•	Memindahkan file ke direktori lain. Bila argumen terakhir adalah nama direktori, maka berkas-berkas akan dipindahkan ke direktori tersebut.
$ mkdir mydir
$ mv f1 f2 f3 mydir


Percobaan 14 : Menghapus file
$ rm f1
$ cp mydir/f1 f1
$ cp mydir/f2 f2
$ rm f1
$ rm –i f2


Percobaan 15 : Mencari kata/kalimat dalam file
$ grep root /etc/passwd
$ grep “:0:” /etc/passwd
$ grep mahasiswa /etc/password



VI.	Tugas
1.	Tugas Percobaan 1 Informasi finger
Ubahlah informasi finger pada komputer Anda dengan memperbarui nama lengkap, ruang, dan nomor telepon sesuai identitas Anda.
 <img width="527" height="212" alt="image" src="https://github.com/user-attachments/assets/2aa8481e-3856-4134-b77b-aa9e1df6b31a" />


2.	Tugas Percobaan 2 log user aktif
Lihatlah user-user yang sedang aktif pada komputer Anda menggunakan perintah who dan w.
 <img width="621" height="221" alt="image" src="https://github.com/user-attachments/assets/0a9c94dd-62cb-452c-b669-fe0390e24df8" />

 

3.	Tugas Percobaan 3 group
Buka file $cat /etc/group kemudian analisa untuk baris root:x:0: yang menunjukkan konfigurasi grup administrator utama.
<img width="551" height="440" alt="image" src="https://github.com/user-attachments/assets/fda9f403-f3b0-4cb8-aa4f-0a86e05373be" />


VII.	Kesimpulan


Berdasarkan praktikum Linux Modul 2 yang telah dilakukan, dapat disimpulkan bahwa manajemen pengguna dan eksplorasi perintah dasar merupakan fondasi penting dalam sistem operasi Linux. Perintah seperti w, who, dan whoami terbukti efektif untuk memantau serta mengidentifikasi pengguna yang sedang aktif di dalam sistem. Selain itu, perintah chfn digunakan untuk mengelola informasi finger atau biodata pengguna, sementara perintah man (manual) sangat membantu pengguna dalam memahami dokumentasi dan argumen dari setiap perintah terminal. Terakhir, pengecekan file konfigurasi sistem seperti /etc/group melalui perintah cat memberikan pemahaman mengenai struktur pengelolaan hak akses dan kelompok pengguna, di mana grup root menempati level tertinggi dengan ID 0.
