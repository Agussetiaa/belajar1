# latihan1 
# LATIHAN VCS

## TUGAS BAHASA PEMROGRAMAN

## Instalali Git

 - Buka wabsite resmi Git (https://git-scm.com/)
 - Kemudian unduh Git sesuai OS
 - Selamat, Git sudah terinstal di windows. untuk mencobanya silahkan buka **CMD** atau **powershell**, kemudian ketik perintah.
```
git --version
```
 ![Gambar1](Gambar/1.png)
 

 ## Menambahkan Global Config
 
 - Pada saat pertama kali, perlu di perhatikan konfigurasi *user.name* dan *user.email*
 - Konfigurasi ini bisa di lakukan untuk global repository atau individual repository.
 - Apabila belum di lakukan konfigurasi, akan mengakitbatkan terjadi kegagalan saat menjalankan perintah git commit

 - Config Global Repository
 ```
 $ git config --global user.name "nama_user"
 ```
 ```
 $ git config --global user.email "nama_user"
 ```


 ## Perintah Dasar Git

 - **git init**, perintah untuk membuat repository local
 - **git add**, perintah untuk menambahkan file baru, atau perubahan pada file pada staging sebelum proses commit.
 - **git commit**, perintah untuk menyimpan perubahan kedalam database git.
 - **git push -u origin master**, perintah untuk mengirim perubahan pada repository local menuju server repository.
 - **git clone [url]**, perintah untuk membuat working directory yang di ambil dari repository server.
 - **git remote add origin [url]**, perintah untuk menambahkan remote server/repository server pada local repository (*working direktory*)
 - **git pull**, perintah untuk mengambil/mendwonload perubahan terbaru dari server repositoy ke local repository


 ## Membuat Repository Lokal

 - Buka direktory aktif: **d:\labs_pemrograman1** (buka menggunakan Widows Explore)
 - klik kanan pada direktory aktif tersebut, dan pilih menu **Git Bash**, sehingga muncul *git bash command*
 - Buat direktory project praktikum pertama dengan nama **latihan1**
  ```
  $ mkdir latihan1
  ```
  ```
  $ cd latihan1
  ```
 - Sehingga terbentuk satu direktory baru dibawahnya, selanjutnya masuk kedalam direktory tersebut dengan perintah **cd** (*change direktory*)
 - direktory aktif menjadi: **d:\lab_pemrograman1\latihan1**
 
 
 ## Membuat Repository Local
 
 - Jalan **git init**, untuk mebuat repository local
 ```
 $ git init
 ```
 - Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktory hidden dengan nama **.git**
 - Pada direktory tersebut, semua perubahan pada *working direktory* akan di simpan.
 
 
  ## Menambahkan File Baru Pada Repository
  
  - Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktory aktif (repository)
  - Disinni kita akan coba buat satu file bernama README.md (text file)
  ```
  $ echo "# latihan1 " >> README.md
  ```
  - File **README.md** berhasil dibuat.
  ![Gambar1](Gambar/2.png)


  ## Menambah File Repository
  - Untuk menambah file baru saja dibuat tersebut gunakan perintah **git add**.
  ```
  $ git add README.md
  ```
  - file **README.md** berhasil ditambahkan.
  ![Gambar](Gambar/3.png)
  
  
  ## Commit (Menyimpan perubahan ke database)
  - Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah **git commit -m "komentar commit"**
  ```
  $ git commit -m "file pertama saya"
  ```
  - Perubahan berhasil disimpan.
  ![Gambar](Gambar/4.png)
  
  
  ## Membuat repository server
  -
