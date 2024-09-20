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

