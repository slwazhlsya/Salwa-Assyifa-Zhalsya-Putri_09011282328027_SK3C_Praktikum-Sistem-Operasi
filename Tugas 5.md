# TUGAS 5 PRAKTIKUM SISTEM OPERASI

 **1. Lihat daftar secara lengkap pada direktori aktif, belokkan tampilan standard output ke file baru.**
 
 Untuk melihat daftar direktori aktif, gunakan perintah $ ls, sedangkan untuk membelokkan tampilan standard output ke file baru, gunakan ">"

 ![image](https://github.com/user-attachments/assets/cb5db572-bd2b-4188-b5cc-58422bc61080)

**2. Lihat daftar secara lengkap pada direktori /etc/passwd, belokkan tampilan standard output ke file baru tanpa menghapus file baru sebelumnya.**

Untuk melihat daftar lengkap dari direktori /etc/passwd, gunakan perntah $ ls, sedangkan untuk membelokkan tampilan standard output ke file baru 
tanpa menghapus file baru sebelumnya, gunakan ">>"

![image](https://github.com/user-attachments/assets/2adbcb32-13cc-4861-8991-363dc61a6c09)

**3. Urutkan file baru dengan cara membelokkan standard input.**

Untuk mengurutkan file, gunakan perintah $ sort, sedangkan untuk membelokkan standard input, gunakan "<"

![image](https://github.com/user-attachments/assets/cbf4e146-d55e-4690-9431-5632871c0d82)

**4. Urutkan file baru dengan cara membelokkan standard input dan standard output ke file baru.urut.**

Untuk mengurutkan file, gunakan perintah $ sort, sedangkan untuk membelokkan standard input, gunakan "<", sedangkan untuk membelokkan standard output ke file, gunakan ">". 
Pembelokan standart input dan standart output dapat dikombinasikan asalkan tidak boleh menggunakan nama file yang sama sebagai standart input dan output.

![image](https://github.com/user-attachments/assets/6934efc0-09ed-4d7f-8024-d6f59840e7c2)

**5. Buatlah direktori latihan6 sebanyak 2 kali dan belokkan standard error ke file rmdirerror.txt.**

Gunakan perintah $ mkdir untuk membuat direktori baru. Saat membuat direktori yang sama sebanyak dua kali, akan muncul pesan error. 
Pesan error itu kemudian dibelokkan ke file dengan menggunakan "2>".

![image](https://github.com/user-attachments/assets/2ae7e2bd-606d-406f-a0c0-2cb1de22ed42)

**6. Urutkan kalimat berikut dengan menggunakan notasi here document :**

**sort <<@@@**

**Jakarta**

**Bandung**

**Surabaya**

**Padang**

**Palembang**

**Lampung**

**@@@**

Pertama, buat notasi here document yang akan dibelokkan ke sebuah file kemudian isi document tersebut. Setelah diisi dan diakhiri, isi dokumen akan tersimpan ke file yang dibelokkan. 
File tersebut kemudian diurutkan menggunakan perintah $ sort. 

![image](https://github.com/user-attachments/assets/5bb03e81-3062-4ce9-95ee-bafb97b684a2)

**7. Hitung jumlah baris, kata, dan karakter dari file baru.urut dengan menggunakan filter dan tambahkan data tersebut ke file baru.**

Untuk mendapatkan jumlah baris, kata, dan karakter (secara berurutan) dari sebuah file, gunakan perintah wc yang dipipakan dengan perintah cat. 
Hasilnya kemudian bisa ditambahkan ke file menggunakan ">>" 

![image](https://github.com/user-attachments/assets/ce348ecd-7774-411f-a768-54b88b4d6632)

**8. Gunakan perintah di bawah ini dan perhatikan hasilnya:**

**cat /etc/passwd | sort | pr -n | grep tty03**

Menampilkan isi /etc/passwd, mengurutkannya, menomori barisnya, dan mencari baris yang mengandung tty03.

**find /etc –print | head**

Menampilkan 10 baris pertama dari daftar file dan direktori di dalam /etc.

**head /etc/passwd | tail -5 | sort**

Menampilkan 5 baris terakhir dari 10 baris pertama file /etc/passwd, kemudian mengurutkannya.

![image](https://github.com/user-attachments/assets/ba868190-20fc-4583-829d-601bfd491ae0)
![image](https://github.com/user-attachments/assets/acc20a7b-a5d3-4bc1-92fa-607ec304e407)

**9. Gunakan perintah berikut dan perhatikan hasilnya:**

**who | cat | cat | sort | pr | head | cat | tail**

Menampilkan pengguna yang sedang login (who), mengurutkan hasilnya, memformat output, menampilkan baris pertama dan terakhir dari hasil tersebut.

![image](https://github.com/user-attachments/assets/ac893a9d-00f5-4a19-88a6-bdcf443b87d9)

