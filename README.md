# Aplikasi CRUD Data Buku Menggunakan Java Swing dan PostgreSQL

## Deskripsi tugas
Tugas ini merupakan simulasi Ujian Tengah Semester yaitu membuat aplikasi `CRUD` (Create, Read, Update, dan Delete) data buku dengan atribut `ISBN`, `Judul Buku`, `Tahun Terbit`, `Penerbit` menggunakan Java Swing dan Postgresql. 

## Langkah-langkah
1. Membuat koneksi baru di Java yang disambungkan dengan Postgresql. Klik kanan pada Database yang ada di menu service, lalu new connection dan memilih postgresql.
   
   ![Screenshot 2024-10-01 142934](https://github.com/user-attachments/assets/36fc07f9-18c5-422c-881e-f8b77a54f314)
   ![Screenshot 2024-10-01 142950](https://github.com/user-attachments/assets/42db1073-8984-4948-a9ef-9fd38acf5fcf)
   
2. Mengisi dan menyesuaikan dengan database yang telah dibuat. Kemudian pilih public dan finish.
   
   ![Screenshot 2024-10-01 143036](https://github.com/user-attachments/assets/69ad7830-f3ce-4ff4-9bf4-fbfb73410fcc)
   ![Screenshot 2024-10-01 143047](https://github.com/user-attachments/assets/415550da-5671-4824-85ad-acec73c09e74)
   ![Screenshot 2024-10-01 143100](https://github.com/user-attachments/assets/10fceb75-7fec-4d33-b873-ef69044c5af6)
   
3. Kemudian, membuat library baru untuk mengkoneksikan ke database kita dengan klik kanan pada Library, lalu Add Library dan pilih Postgresql JDBC Driver.
   
   ![Screenshot 2024-10-01 143129](https://github.com/user-attachments/assets/ff429b94-9655-4634-b2b5-89aaadd21c58)
   ![Screenshot 2024-10-01 143152](https://github.com/user-attachments/assets/4c353e70-2620-4390-9d2d-2ff3d41cf281)
   
4. Ini adalah tampilan ketika kita sudah add library kita dengan JDBC Driver Postgresql.

   ![Screenshot 2024-10-01 143202](https://github.com/user-attachments/assets/064d6cd3-8c04-4785-bce1-91bcb33377e7)
   
5. selanjutnya adalah membuat desain Java Swing dengan cara klik kanan pada package yang telah dibuat, lalu pilih Jframe From.

   ![Screenshot 2024-10-01 143245](https://github.com/user-attachments/assets/1fc6a5fc-0826-4a6e-af55-88e944973f1d)

6. Beri nama pada Jframe From nya, disini saya memberi nama yaitu simulasi_06.

   ![Screenshot 2024-10-01 143326](https://github.com/user-attachments/assets/3f2fa92a-bf7b-4323-929f-2278dbc77978)

7. Berikut adalah desain yang telah saya buat.

   ![Screenshot 2024-10-02 065107](https://github.com/user-attachments/assets/af8aa20b-0573-4afe-bf4d-ed152e403d98)

8. Kemudian, terlebih dahulu saya membuat class DbUtils pada package yang sama.
 
   ![Screenshot 2024-10-01 150154](https://github.com/user-attachments/assets/a308f993-8db5-48e6-a33a-da6c3455730b)

9. Sebelum lanjut ke tahap selanjutnya, kita harus membuat tabel yang ada di database kita. Berikut adalah query dari pembuatan tabel dalam database saya dengan beberapa atribut yang sudah ditentukan.

   ![Screenshot 2024-10-01 161924](https://github.com/user-attachments/assets/bcfbb18d-63bd-4a7d-b145-92bd8f5a05d1)

10. Berikut adalah source code dalam class DbUtils.

    ![Screenshot 2024-10-02 065544](https://github.com/user-attachments/assets/5d6acdbc-af77-4eb2-b7cc-0f5a05f0de1a)
    
11. Berikut adalah source code dari Connection to Database.

    ![Screenshot 2024-10-02 065835](https://github.com/user-attachments/assets/74479f53-dcbc-4b86-8cdb-5e93c2753ef3)
    
12. Berikut adalah source code dari Insert.

    ![Screenshot 2024-10-02 065851](https://github.com/user-attachments/assets/2f2ac1c7-66ec-4f66-b374-f4d092524bc3)
    dalam insert kita harus mengisi pertanyaan yang ada, kemudian akan bisa melakukan aksi insert. jika kita mengosongi salah satunya, maka program tidak akan berjalan dan ada pop up peringatannya.
    
13. Berikut adalah source code dari Update.

    ![Screenshot 2024-10-02 065859](https://github.com/user-attachments/assets/61716ab5-e986-45d2-82fa-ca10b1b3c143)
    dalam update kita bisa mengeklik data pada tabel saja, lalu data akan otomatis ke isi pada kolom jawaban. Kemudian kita akan dengan mudah mengganti apa yang perlu diganti, tapi tidak untuk PRIMARY KEY.
    
14. Berikut adalah source code dari Delete.

    ![Screenshot 2024-10-02 065908](https://github.com/user-attachments/assets/57e70bcb-4325-49bc-b26b-cfdd357358f6)
    dalam delete ini akan menghapus data yang kita inginkan dan memberikan konfirmasi saat akan menghapus data.
    
15. Berikut adalah source code dari Tampil/Select.

    ![Screenshot 2024-10-02 065937](https://github.com/user-attachments/assets/fbea1205-37d5-4cd8-94ed-1484c8bcd433)
    
16. Berikut adalah source code dari tbTabelMouseClicked.

    ![Screenshot 2024-10-02 065923](https://github.com/user-attachments/assets/097100b8-8131-4d48-9c3e-f33574af9bfb)
    
17. Berikut adalah source code dari Clear.

    ![Screenshot 2024-10-02 065917](https://github.com/user-attachments/assets/2e1d9a04-ce92-4653-a29e-1fee0c7f5bd2)
    
    dalam source code ini juga ada tambahan code untuk mengkosongkan semua kolom jawaban yaitu dengan Clear yang mengambil dari method bersih berikut ini.
    
    ![Screenshot 2024-10-02 070650](https://github.com/user-attachments/assets/40981cd2-794d-447f-9d81-953a435d58c3)
    
18. Berikut adalah hasil desain dari yang telah saya buat.
    ![Screenshot 2024-10-02 062759](https://github.com/user-attachments/assets/c8cb4994-0c6f-4ef4-9df2-46d9fe0d9df0)

## Uji Coba
1. Insert

   ![Screenshot 2024-10-02 062159](https://github.com/user-attachments/assets/9d2c027a-4a3e-4bc2-b3f1-f65a08a4e96a)
   ![Screenshot 2024-10-02 062217](https://github.com/user-attachments/assets/5d0357ef-c89e-46f3-a1e6-9e5f440a202a)
2. Update

   ![Screenshot 2024-10-02 062444](https://github.com/user-attachments/assets/c7932a52-90d7-41d4-b010-f57194d9d9de)
   ![Screenshot 2024-10-02 062521](https://github.com/user-attachments/assets/cc498198-a8ef-40b3-8922-c534cb0a408f)
   ![Screenshot 2024-10-02 062657](https://github.com/user-attachments/assets/a26fd261-a4b0-48d0-b9ea-431b02a91e6c)
   ![Screenshot 2024-10-02 062705](https://github.com/user-attachments/assets/8182948a-56a5-46c1-b26b-2b536ac9f6a6)
3. Delete

   ![Screenshot 2024-10-02 062724](https://github.com/user-attachments/assets/7493e424-c6f5-4956-a0f3-cdc7c41974db)
   ![Screenshot 2024-10-02 062731](https://github.com/user-attachments/assets/3f387c8d-80c4-40b3-b61a-8cca4a21955c)
   ![Screenshot 2024-10-02 062740](https://github.com/user-attachments/assets/18af3e4b-2575-4260-9d85-026fb6583933)
4. Clear

   ![Screenshot 2024-10-02 062750](https://github.com/user-attachments/assets/8f17906d-775f-4c9b-ac2e-7e6a2f87a4bb)
   ![Screenshot 2024-10-02 062759](https://github.com/user-attachments/assets/427ca8ed-e219-4d14-af76-7ccb3dbc428d)

Semoga penjelasan diatas dapat membantu memahami materi dalam tugas pertemuan 7 simulasi UTS mata kuliah Pemrograman Berorientasi Objek ini.









    







   






   



   

   

