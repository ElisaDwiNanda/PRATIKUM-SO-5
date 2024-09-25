# PRATIKUM-SO-5
## 1. Eksekusi seluruh profile yang ada : 
### a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut : 
echo “Profile dari /etc/profile” 
### b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu : 
/home/stD02001/.bash_profile </br>
/home/. stD02001/.bash_login </br>
/home/mahasiswa/.profile </br>
/home/mahasiswa/.bashrc 
### c. Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile : 
echo “Profile dari .bash_profile” 

Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan. </br>
$ su mahasiswa </br>
$ exit </br>

kemudian gunakan opsi – sebagai berikut : </br>
$ su – mahasiswa </br>
$ exit </br>

Jelaskan perbedaan kedua utilitas tersebut. 

1. $ sudo nano/etc/profile
 ![image](https://github.com/user-attachments/assets/5aaf6041-0d85-4eb5-a2a4-5b6a2410c463)
![image](https://github.com/user-attachments/assets/ee9d65fe-8202-441e-8da0-b652dcf757f6)

Analisis
-	Perintah diatas kita disuruh mengedit file di etc/profile. Maka langkah- langkahnya adalah
-	Membuka file /etc/profile dengan perintah

$ sudo nano /etc/profile
-	Menambahkan echo “profile dari /etc/profile” pada file tersebut
-	Menyimpannya dengan cara ctrl + X, tekan Y, enter
-	Kemudian kita cek dengan menggunakan su - <user>, dan terlihat profile dari /etc/profile sudah terlihat. Artinya kita sukses menambahkannya.

2. $ sudo nano /home/elisa/.bash_login
$ sudo nano /home/elisa/.bash.profile
$ sudo nano /home/elisa/.profile
$ sudo nano /home/elisa/.bashrc

Analisis :
-	Semua perintah diatas kita mengubah semua profile yang ada. Yaitu .bash_profile , .bash_login, .profile, .bashrc
-	Kita mengubah dengan cara yang sama dengan latihan 1a
 
![image](https://github.com/user-attachments/assets/f9384cb4-6c30-4286-b1a9-241b4ee40f17)

![image](https://github.com/user-attachments/assets/9c9ef9b9-4597-4e80-9d93-eed20b9499b1)

![image](https://github.com/user-attachments/assets/4cd9dc15-c53c-4017-a568-b7fa5a253704)

![image](https://github.com/user-attachments/assets/52306251-f137-42e7-a9e1-f54afd98913e)

![image](https://github.com/user-attachments/assets/8abe0028-6aa9-46bf-96ca-d8b81d1bca70)

![image](https://github.com/user-attachments/assets/ef3f567d-3304-4a1f-8ded-967b1a5cb529)

![image](https://github.com/user-attachments/assets/d1eb43ef-c980-4b56-8184-aa273c8033e7)

![image](https://github.com/user-attachments/assets/06bad8c4-ffa2-4693-a1fc-1c9ff3c45bdf)

![image](https://github.com/user-attachments/assets/58dd4b01-1f9f-408c-a721-f5cb3a7b1913)

![image](https://github.com/user-attachments/assets/7d4aa8ef-fddf-4c31-97df-17d32094c032)

Analisis :
-	Fungsi dari setiap file yang kita edit akan muncul pada waktu tertentu.

### c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:
$ su mahasiswa </br> 
$ exit </br>
![image](https://github.com/user-attachments/assets/c508d871-4bd8-4e5f-be69-16719c037d33)

kemudian gunakan opsi – sebagai berikut : </br>
$ su – mahasiswa </br>
$ exit </br>
![image](https://github.com/user-attachments/assets/91ac69f0-1521-45aa-8acf-fe2b8c5deae5)

Jelaskan perbedaan kedua utilitas tersebut.

Analisa :
-	Perbedaan dari 2 utilitas tersebut adalah Jika - (atau -l) ditentukan, su mensimulasikan login nyata. Lingkungan dibersihkan kecuali untuk beberapa variabel pilih (terutama, DISPLAY dan XAUTHORITY pada beberapa sistem). Jika tidak, lingkungan dibiarkan seperti itu kecuali untuk PATH yang direset.


## 2. Prompt String (PS) 
### a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell 
PS1=‟> „ </br>
export PS1 </br>
![image](https://github.com/user-attachments/assets/b7278bc6-11bd-4e3d-88bb-147d1fb54812)

![image](https://github.com/user-attachments/assets/971c2b19-27a1-4c7a-8695-d0e3572976ed)


### b. Eksperimen hasil PS1 :
$ PS1=“\! > “</br>
69 > PS1=”\d > “ </br>
Mon Sep 23 > PS1=”\t > “ </br>
10:10:20 > PS1=”Saya=\u > “ </br>
Saya=stD02001 > PS1=”\w >” </br>
~ > PS1=\h >” </br>
![image](https://github.com/user-attachments/assets/6d9e62fe-e78b-4572-93e4-1bb54d8f1211)


## 3. Logout 
Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout </br>
Echo “Terima kasih atas sesi yang diberikan” </br>
Sleep 5 </br>
clear</br>
![image](https://github.com/user-attachments/assets/7c15cb70-d15b-4fcc-aba0-06973fcf0e50)

![image](https://github.com/user-attachments/assets/2bfa4741-727d-4bd6-b249-64322983eac3)

Hasil dari edit file .bash_logout :
![image](https://github.com/user-attachments/assets/e19d2b10-a9a4-4b09-a904-452ddf24ae1c)


Analisis :
-	Kita menuliskan echo “terimakasih atas sesi yang diberikan” dan menulis program diatas dengan maksud akan memberikan waktu 5 detik kemudian logout.
-	Setelah kita cek dengan login dan kemudian exit. Ternyata hasilnya seperti gambar yaitu terimakasih atas sesi yang diberikan dan kemudian exit setelah 5 detik

## 4. Bash script 
### a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing : 
p1.sh </br>
#! /bin/bash </br>
echo “Program p1” </br>
ls –l </br>
![image](https://github.com/user-attachments/assets/6982e7d7-9fb5-4abe-b89a-dedb9fe02d4f)

![image](https://github.com/user-attachments/assets/f68845b8-718c-4412-b645-7b3d06945f3a)

p2.sh </br>
#! /bin/bash </br>
echo “Program p2” </br>
who </br>
![image](https://github.com/user-attachments/assets/a70498a2-d8a9-43d5-9930-fa5760915d13)

![image](https://github.com/user-attachments/assets/4ec272c7-9952-4f1c-bfd0-216dfb90a356)

p3.sh </br>
#! /bin/bash </br>
echo “Program p3” </br>
ps x </br>
![image](https://github.com/user-attachments/assets/43f91b37-52c5-4d24-96bf-53ebd670945f)

![image](https://github.com/user-attachments/assets/d63c9f57-e056-4974-b2ee-c3d3636da721)

### b. Jalankan script tersebut sebagai berikut :
$ ./p1.sh ; ./p3.sh ; ./p2.sh 
![image](https://github.com/user-attachments/assets/516e9aba-5280-4b72-b08c-b2b8dde441d2)
![image](https://github.com/user-attachments/assets/cdc443f1-a881-42f6-8c82-2575d2b6ad45)
![image](https://github.com/user-attachments/assets/9e47d359-6aa8-4d42-b2cc-5c897e9752fd)
 
Analisis
-	Perintah diatas berfungsi untuk menjalankan program p1 kemudian dilanjutkan program p3 dan dilanjutkan program p2

$ ./p1.sh & 
![image](https://github.com/user-attachments/assets/7b083574-f293-4acc-b81b-d6e1bf1f798d)

Analisis
-	Perintah diatas untuk menjalankan program p1 dan menjalankan di background

$ ./p1.sh $ ./p2.sh & ./p3.sh & 
![image](https://github.com/user-attachments/assets/a495f694-af8a-4f8a-a391-31a88ba90fe2)

Analisis
-	Menjalankan p1 jika berhasil maka akan menjalankan p2 dan p3 di background

$ ( ./p1.sh ; ./p3.sh ) &
![image](https://github.com/user-attachments/assets/07c1c515-2b4d-4fac-a15e-762a100421ba)

Analisis
-	Perintah diatas akan menjalankan program p2 dalam background dan jika berhasil maka akan menjalankan program p3 didalam background $ ( ./p1.sh ; ./p3.sh ) &

## 5. Jobs 
### a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.
#!/bin/bash </br>
while [ true ] </br>
do </br>
        date >> hasil </br>
        sleep 10 </br>
done </br>
![image](https://github.com/user-attachments/assets/3585a164-8254-4982-a866-8769e7338e40)

![image](https://github.com/user-attachments/assets/e6ca75f9-f05f-4867-879c-2765d87c60fe)

 
### b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut : 
$ jobs </br>
$ find / -print > files 2>/dev/null & </br>
$ jobs </br>
![image](https://github.com/user-attachments/assets/8944f51b-df86-47cd-bb15-c6ca08429d11)

Analisis :
-	Melihat apakah masih berjalan atau tidak

### c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background 
$ fg %1 </br>
$ bg </br>
![image](https://github.com/user-attachments/assets/682e6ec1-4ad7-4fbc-b72b-d9cf430853d4)

Analisis
-	Perintah fg %1 maksudnya memindahkan program 1 yang ada di background menjadi berada di foreground. Dan untuk memindahkan kembali ke background, di hentikan dulu dengan Ctrl+Z

### d. Stop program background dengan utilitas kil 
$ ps x </br>
$ kill [Nomor PID] </br>
![image](https://github.com/user-attachments/assets/68c751ed-9ea3-48c7-94c6-f0ef717ec7ba)

![image](https://github.com/user-attachments/assets/4b70716d-a5aa-433c-ab70-b1ffbbe3caca)

Analisis
-	Perintah kill digunakan untuk menghentikan proses sesuai pid. Dan untuk memastikan proses telah dihentikan maka kita gunakan perintah jobs. Dan terlihat proses usdah ter terminated

## 6. History 
### a. Ganti nilai HISTSIZE dari 1000 menjadi 20 
$ HISTSIZE=20 </br>
$ h </br>
![image](https://github.com/user-attachments/assets/2a09248a-783e-40fd-8975-28486fd722e3)

### b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan 
$ !-5 
![image](https://github.com/user-attachments/assets/680f67c4-2714-4115-87c2-baf56e80a231)

Analisis :
-	Megerjakan perintah dari 5 baris yang terakhir dilakukan

### c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer 
$ !! 
![image](https://github.com/user-attachments/assets/f8615be8-bd8e-4bfd-a74b-6f863c772253)

Analisis
-	Mengulangi instruksi yang terakhir

### d. Ulangi instruksi pada history bufer nomor 150 
$ !150 
![image](https://github.com/user-attachments/assets/541f4bf6-74b5-4699-87b6-953db109a064)

Analisis
-	Mengulangi instruksi tertentu berdasarkan nomer tertentu

### e. Ulangi instruksi dengan prefix “ls” 
$ !ls
![image](https://github.com/user-attachments/assets/fc5fc45f-94e5-459a-a091-a075db475a86)

