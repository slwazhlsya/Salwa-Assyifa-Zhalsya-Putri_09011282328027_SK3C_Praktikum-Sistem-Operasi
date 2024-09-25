# PRAKTIKUM 5 - JOB CONTROL

### 1. Eksekusi seluruh profile yang ada
   - Edit file profile /etc/profile dan tampilkan pesan sebagai berikut:

      *__echo "Profile dari /etc/profile"__*

     ![image](https://github.com/user-attachments/assets/b07e3df5-f37d-4b41-ae4d-9762c189f0e4)
     
     ![image](https://github.com/user-attachments/assets/3196fba4-55fb-48e0-9a42-9e50600e69f3)


   - Asumsikan nama Anda stD02001, maka edit semua profile yang ada, yaitu:

     *__- /home/mahasiswa/.bash_profile__*

      *__- /home/mahasiswa/.bash_login__*

      *__- /home/mahasiswa/.profile__*
     
     *__- /home/mahasiswa/.bashrc__*
     
![image](https://github.com/user-attachments/assets/a02ea42e-7af0-43cb-8159-7c79559c77b8)

   - Ganti nama /home/mahasiswa/ dengan nama Anda sendiri. Pada setiap file tersebut, tambahkan instruksi berikut:
    
     *__echo "Profile dari .bash_profile"__*

     Lakukan hal yang sama pada file yang lain

     ![image](https://github.com/user-attachments/assets/93eaba07-198a-4c20-9be1-362aabeaddf5)

     ![image](https://github.com/user-attachments/assets/9e43bd0c-6342-44aa-8001-5faa01ccbec7)

     ![image](https://github.com/user-attachments/assets/2391652c-6b63-4b38-9957-2d3bfccd97dc)

     ![image](https://github.com/user-attachments/assets/da530c29-b559-484f-a518-bdaca4c81945)

   - Jalankan instruksi substitute user, kemudian keluar dengan perintah exit sebagai berikut:

     ![image](https://github.com/user-attachments/assets/b1378822-3dc7-41ce-8f06-a82bd6a9452c)

     Perbedaan kedua utilitas tersebut:
     
     __1. su mahasiswa:__

        Perintah ini menjalankan su untuk beralih ke user mahasiswa. Saat menggunakan perintah ini tanpa opsi -, lingkungan (environment) dari user saat ini tetap dipertahankan.
        Artinya, hanya identitas pengguna yang berubah, tetapi variabel lingkungan seperti PATH tidak akan berubah.
        Jadi, variabel lingkungan dan direktori kerja yang sedang aktif tetap sama seperti sebelumnya.
        
     __2. su - mahasiswa:__

        Perintah ini menggunakan opsi - yang dikenal sebagai login shell. Opsi ini melakukan login penuh sebagai user mahasiswa,
        sehingga environment yang dimuat adalah environment milik mahasiswa secara lengkap.
        Ini termasuk mengubah direktori kerja ke home directory user mahasiswa dan memuat variabel lingkungan seperti yang didefinisikan dalam shell milik mahasiswa.
        Jadi, ini seperti memulai sesi baru sebagai user mahasiswa.

### 2. Prompt String (PS1)
   - Edit file .bash_profile, ganti prompt PS1 dengan > sebagai prompt. Instruksi export diperlukan dengan parameter nama variable tersebut,
     agar perubahan variable PS1 dikenali oleh semua shell yang berjalan.

     ![image](https://github.com/user-attachments/assets/d170fe02-cfc5-4d33-8b09-9b55b72395a0)

     ![image](https://github.com/user-attachments/assets/45443533-a315-4e18-bcf8-1a27c44373b4)

   - Eksperimen hasil PS1.
     
     ![image](https://github.com/user-attachments/assets/28f02fba-b062-4c5a-badb-c1620e77ce12)


### 3. Logout
   - Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout:

     ![image](https://github.com/user-attachments/assets/94f30bac-c732-425b-9e61-638dc9222d58)

     ![image](https://github.com/user-attachments/assets/9a1c36d5-5923-4a32-8290-3ed1f01aecaa)

### 4. Bash Script
   - Buat 3 buah script (p1.sh, p2.sh, p3.sh) dengan isi masing-masing:
     #### p1.sh
     
     *__#!/bin/bash__*
     
     *__echo "Program p2"__*
    
     *__ls -l__*
     
     #### p2.sh
     
     *__#!/bin/bash__*
     
     *__echo "Program p2"__*
     
     *__who__*

     #### p3.sh

     *__#!/bin/bash__*
     
     *__echo "Program p3"__*
     
     *__ps x__*

     ![image](https://github.com/user-attachments/assets/157a2989-b268-4404-b0db-b70b2b3df0e3)

     ![image](https://github.com/user-attachments/assets/a12bf226-d803-4af8-a80d-2dbcaa736feb)

     ![image](https://github.com/user-attachments/assets/43f12d9d-1455-47c0-8760-976ccb6ccfa0)

     ![image](https://github.com/user-attachments/assets/a8ac5083-67c6-4a3b-9c63-67ba5207724b)

   - Jalankan script tersebut
   
     ![image](https://github.com/user-attachments/assets/45ac9cf6-b1cf-4343-9a37-6b7648af6e24)

     ![image](https://github.com/user-attachments/assets/5b61fa29-0e22-4236-9d2a-ff97e22db31c)
     
     ![image](https://github.com/user-attachments/assets/add846f2-eb84-4804-b083-c3c5354034c2)

     ![image](https://github.com/user-attachments/assets/dc248c6d-8cf7-4721-8fd5-1b0e6971ae32)

     ![image](https://github.com/user-attachments/assets/4948c33b-2549-4cbf-9823-b0e9d88708e7)

     ![image](https://github.com/user-attachments/assets/4265a115-664d-4e40-9177-b520519f9adc)

### 5. Jobs
   - Buat sebuah script looping melakukan loop dengan nama pwaktu.sh.  
     Setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil:

     ![image](https://github.com/user-attachments/assets/99668492-ef1d-4750-9b46-0ec0cad0dd9b)

     ![image](https://github.com/user-attachments/assets/5fa3c762-ed21-4836-8c3f-46c5a652be99)
  
   - Jalankan sebagai background, kemudian jalankan satu program (misalnya find) di background sebagai berikut:

     ![image](https://github.com/user-attachments/assets/d41891c8-c038-4d52-93da-54f75fbce0f2)

   - Jadikan program find sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background:

     ![Screenshot 2024-09-25 183926](https://github.com/user-attachments/assets/76cbaba3-d307-4931-8009-027ac090dfcf)

   - Stop program background dengan utilitas kill:

     ![image](https://github.com/user-attachments/assets/d2aec2f8-efae-48ae-9663-c3dfe985f9b6)

     ![image](https://github.com/user-attachments/assets/093fee53-8aa9-4d5e-b792-c331dc84ecd1)


### 6. *History*:
   - Ganti nilai HISTSIZE dari 1000 menjadi 20:

     ![image](https://github.com/user-attachments/assets/a908b9f5-6863-4b43-bbcd-31b0759cbb59)

   - Gunakan fasilitas history dengan mengoreksi instruksi baris ke-5 dari instruksi yang terakhir dilakukan:

     ![image](https://github.com/user-attachments/assets/e8ef0796-1775-487b-a0ba-fd11dfce7ffd)  
     
   - Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk beberapa perintah pada history buffer.

     ![image](https://github.com/user-attachments/assets/7fc3a846-c653-408b-a282-3467481ffa7d)

   - Edit nilai HISTFILESIZE agar history buffer nomor 150.

     ![image](https://github.com/user-attachments/assets/edebaf04-bc95-49a8-bdfe-040187e48bd7)

     karena history nomor 150 tidak ada jadi diganti dengan history nomor 272

   - Ulangi instruksi dengan grep "ls":

     ![image](https://github.com/user-attachments/assets/44ea1aab-cd9a-4a74-ab34-f9536e9d6cc2)

    
     

    
