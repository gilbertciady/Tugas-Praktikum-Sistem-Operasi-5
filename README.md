# Tugas-Praktikum-Sistem-Operasi-5
- Nama: Gilbert Ciady
- NIM: 09011182328005
- Kelas: SK3B
## Tugas Praktikum 5 Job Control
1. Eksekusi seluruh profile yang ada :  
a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :  
echo “Profile dari /etc/profile”  
![Screenshot 2024-09-19 122110](https://github.com/user-attachments/assets/63b6fc5f-1bb4-4a39-8c54-d384646a1bdd)  
![Screenshot 2024-09-19 122144](https://github.com/user-attachments/assets/5969be1b-fb3f-48e5-b5b1-14c88e2af511)  
![Screenshot 2024-09-19 122623](https://github.com/user-attachments/assets/69efe8d2-1703-4528-9fc9-a6d0cf233344)  
![Screenshot 2024-09-19 122717](https://github.com/user-attachments/assets/127a0c2a-393e-4f1d-a4c1-59b79708ebbc)  
b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :  
/home/stD02001/.bash_profile  
/home/. stD02001/.bash_login  
/home/mahasiswa/.profile  
/home/mahasiswa/.bashrc  
Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo,  
misalnya pada /home/ mahasiswa/.bash_profile :  
echo “Profile dari .bash_profile”  
Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.  
![Screenshot 2024-09-20 083757](https://github.com/user-attachments/assets/9dddf295-ae01-4047-93a3-1054afaf7999)  
![Screenshot 2024-09-20 084036](https://github.com/user-attachments/assets/7653cc00-4c2b-42c4-91ae-94e1d41cf10e)  
![Screenshot 2024-09-20 084244](https://github.com/user-attachments/assets/8dc671ba-9551-4a94-802d-e3c3c104ee91)  
![Screenshot 2024-09-20 084230](https://github.com/user-attachments/assets/651b8b87-cbf7-4c8f-bb25-817a84df2552)  
![Screenshot 2024-09-20 084401](https://github.com/user-attachments/assets/25a467f0-c7d2-478f-b6a4-0c4027ceb025)  
![Screenshot 2024-09-20 084340](https://github.com/user-attachments/assets/9fe7269d-68b3-4816-afb5-c945a1f5e254)  
![Screenshot 2024-09-20 084458](https://github.com/user-attachments/assets/90102b94-dfc7-4743-96e0-571275ef0cfb)  
![Screenshot 2024-09-20 084711](https://github.com/user-attachments/assets/45e4a897-f378-426a-8187-ad793338c634)  
c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:  
$ su mahasiswa  
$ exit  
kemudian gunakan opsi – sebagai berikut :  
$ su – mahasiswa  
$ exit  
![Screenshot 2024-09-20 084806](https://github.com/user-attachments/assets/e3e3bc8a-d226-4d02-ad99-861dc9ec20d1)  
![Screenshot 2024-09-20 084837](https://github.com/user-attachments/assets/804454e3-82b5-4826-bd3a-ad315ef7d3c0)  
Jelaskan perbedaan kedua utilitas tersebut.  
su hanya menampilkan profile / file dari .bashrc karena hanya hak akses dan identitas pengguna yang berubah dan tidak merubah enviorment shell  
su - menampilkan dan menjalankan profile / file dari pengguna seperti /etc/profile dan .bash_profile di enviorment shell baru  
2. Prompt String (PS)  
a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan  
parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell  
PS1=‟> „  
export PS1  
![Screenshot 2024-09-20 090915](https://github.com/user-attachments/assets/7e84b1cb-3e01-4bde-916a-b0debcf3834c)  
![Screenshot 2024-09-20 091024](https://github.com/user-attachments/assets/a32b129d-ed47-4314-aa76-255829b46b22)  
![Screenshot 2024-09-20 091248](https://github.com/user-attachments/assets/dd001fc6-0687-4fcc-938c-2dc345b5324a)  
b. Eksperimen hasil PS1 :  
$ PS1=“\! > “  
69 > PS1=”\d > “  
Mon Sep 23 > PS1=”\t > “  
10:10:20 > PS1=”Saya=\u > “  
Saya=mahasiswa > PS1=”\w >”  
~ > PS1=\h >”  
![Screenshot 2024-09-20 100908](https://github.com/user-attachments/assets/d6a24c50-199e-4191-a68a-245c26204a71)  
3. Logout  
Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout  
Echo “Terima kasih atas sesi yang diberikan”  
Sleep 5  
clear  
![Screenshot 2024-09-20 101046](https://github.com/user-attachments/assets/a5a30aa5-cdf1-4355-8cdc-e8dca345caa0)  
![Screenshot 2024-09-20 101207](https://github.com/user-attachments/assets/b5501e03-4144-44d0-aff5-f08bd41ec9a0)  
4. Bash script  
a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :  
p1.sh  
#! /bin/bash  
echo “Program p1”  
ls –l  
p2.sh  
#! /bin/bash  
echo “Program p2”  
who  
p3.sh  
#! /bin/bash  
echo “Program p3”  
ps x  
![Screenshot 2024-09-20 102640](https://github.com/user-attachments/assets/470fad6d-4cb9-418a-8bf5-eb204a158135)  
![Screenshot 2024-09-20 102738](https://github.com/user-attachments/assets/772ac0eb-1e5e-46da-90c4-8c5c7a5094d2)  
![Screenshot 2024-09-20 103009](https://github.com/user-attachments/assets/75fe4e33-4d50-48d9-82df-b83b04315836)  
![Screenshot 2024-09-20 102845](https://github.com/user-attachments/assets/7646063e-9ae3-4818-b0ea-46b29be0929c)  
![Screenshot 2024-09-20 103019](https://github.com/user-attachments/assets/1f20058c-0a0a-41ed-9c2f-a58719afd4ca)  
![Screenshot 2024-09-20 102950](https://github.com/user-attachments/assets/ff4b392d-32a0-4367-83b2-55b185fa9970)  
b. Jalankan script tersebut sebagai berikut :  
$ ./p1.sh ; ./p3.sh ; ./p2.sh  
$ ./p1.sh &  
$ ./p1.sh $ ./p2.sh & ./p3.sh &  
$ ( ./p1.sh ; ./p3.sh ) &  
![Screenshot 2024-09-20 103337](https://github.com/user-attachments/assets/131a4397-e592-4ddf-81f7-9a59edcdd8b1)  
![Screenshot 2024-09-20 103353](https://github.com/user-attachments/assets/57f6e62b-6c8a-4ba6-bc3c-4aa28bfd63c1)  
![Screenshot 2024-09-20 103413](https://github.com/user-attachments/assets/7bf05091-3f7b-4f09-a3e1-4ba4c6b96a6c)  
![Screenshot 2024-09-20 104040](https://github.com/user-attachments/assets/7d09af14-8b0d-45fc-927a-5d9190a6fa7b)  
![Screenshot 2024-09-20 104104](https://github.com/user-attachments/assets/9b7fbcd4-1f31-4895-b838-d14fad049adf)  
![Screenshot 2024-09-20 104119](https://github.com/user-attachments/assets/8002be90-8b20-4d64-b0f1-bb7d5c82cfcc)  
5. Jobs  
a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik,  
kemudian menyimpan tanggal dan jam pada file hasil.  
#!/bin/bash 
while [ true ] 
do 
  date >> hasil 
  sleep 10 
done 
![Screenshot 2024-09-20 105659](https://github.com/user-attachments/assets/ad5ca104-64b3-41e5-997d-c9f746276e22)  
![Screenshot 2024-09-20 105858](https://github.com/user-attachments/assets/430e6238-ec14-40b7-a322-6b39936aecaf)  
b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :  
$ jobs  
$ find / -print > files 2>/dev/null &  
$ jobs  
![Screenshot 2024-09-20 110832](https://github.com/user-attachments/assets/9850ae66-db84-4f65-ac91-4d95c98907eb)  
![Screenshot 2024-09-20 110850 (1)](https://github.com/user-attachments/assets/ec03d988-0165-4e13-b146-38f99cc499e0)  
c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background  
$ fg %1  
$ bg  
![Screenshot 2024-09-20 110850](https://github.com/user-attachments/assets/de0deb73-3923-4fb2-bddd-86de28ec0c73)  

d. Stop program background dengan utilitas kill   
$ ps x  
$ kill [Nomor PID]  
![Screenshot 2024-09-20 111006](https://github.com/user-attachments/assets/8138d6cd-a8b6-482a-aa91-be18798be628)  
![Screenshot 2024-09-20 111109](https://github.com/user-attachments/assets/cf7f296d-f179-4ca0-a74a-94cd8f11dcd5)  
![Screenshot 2024-09-20 111123](https://github.com/user-attachments/assets/9e7da7fb-9414-4f8f-8554-1a0c56073ffe)  
6. History  
a. Ganti nilai HISTSIZE dari 1000 menjadi 20  
$ HISTSIZE=20  
$ h  
![Screenshot 2024-09-20 111403](https://github.com/user-attachments/assets/cfdd5340-bd6c-4c41-8762-f8f3971edc32)  
b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan  
$ !-5  
c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer  
$ !!  
d. Ulangi instruksi pada history bufer nomor 150  
$ !150  
e. Ulangi instruksi dengan prefix “ls”  
$ !ls  
![Screenshot 2024-09-20 111603](https://github.com/user-attachments/assets/dcd12021-4627-4e97-8bd1-e7f5d9da9f2a)  
