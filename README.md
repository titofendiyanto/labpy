#latihan 1
# Cara penggunaan git
# Apa Itu Git ?
* Git adalah salah satu sistem pengontrol versi(Version Control System) pada proyek perangkat lunak yang diciptakan Linus Torvalds.
* Pengontrol versi bertugas memcatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.
* Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja.
# Instalasi Git
* Download Git, Buka website resminya [git-scm.com.](https://git-scm.com)
* Kemudian unduh Git sesuai dengan arsitektur komputer kita, Kalau menggunakan 64bit, unduh yang 64bit. Begitu juga kalau menggunakan 32bit.

  ![downloadgit](https://user-images.githubusercontent.com/57053160/68082721-94e01e80-fe52-11e9-84cf-3ecc7967002a.png)

* Selamat, Git sudah terinstal di Windows. Untuk mencobanya, silahkan buka CMD atau PowerShell, kemudian ketik perintah ``git --version``

  ![gitversion](https://user-images.githubusercontent.com/57053160/68082747-e2f52200-fe52-11e9-8fe7-0747980d232f.png)

# Menambahkan Global Config
* Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email
* konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.
* apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah ``git commit``
* Config Global Repository

  ![git config 1](https://user-images.githubusercontent.com/57053160/68082766-22bc0980-fe53-11e9-95d5-6acf2177943c.png)
  
# Perintah Dasar Git
* ``git init`` , perintah untuk membuat repository local.
* ``git add`` , perintah untuk menambahkan file baru, atau perubahan pada file pada staging sebelum proses commit.
* ``git commit`` , perintah untuk menyimpan perubahan kedalam database git.
* ``git push -u origin master`` , perintah untuk mengirim perubahan pada repository local menuju server repository.
* ``git clone [url]``, perintah untuk membuat working directory yang diambil dari repositry sever.
* ``git remote add origin [url]`` , perintah untuk menambahkan remote server/reopsitory server pada local repositry (working directory)
* ``git pull`` , perintah untuk mengambil/mendownload perubahan terbaru dari server repository ke local repository.
# Membuat Reposiory Local
* Buka direktory aktif, misal: ``d:\labs_pemrograman1`` (bukamenggunakan Windows Explorer)
* klik kanan pada direktory aktif tersebut, dan pilih menu ``Git Bash`` ,sehingga muncul git bash commad
* Buat direktory project praktikum pertama dengan nama latihan1

  ![config2](https://user-images.githubusercontent.com/57053160/68082829-1d12f380-fe54-11e9-9708-a62b52da75af.png)

* Sehingga terbentuk satu direktori baru dibawahnya, selanjutnyamasuk kedalam direktori tersebut dengan perintah cd (changedirectory)
* direktory aktif menjadi: ``d:\labs_pemrograman1\latihan1``
# Membuat Reposiory Local
* Jalankan perintah git init, untuk membuat repository local.
* Repository baru berhasil di inisialisasi, dengan terbentuknya satudirektori hidden dengan nama .git
* Pada direktori tersebut, semua perubahan pada working directory akan disimpan.

  ![git init](https://user-images.githubusercontent.com/57053160/68082998-2b620f00-fe56-11e9-8289-51ba1737d7a3.png)

# Menambahkan File baru pada repository
* Untuk membuat file dapat menggunakan text editor, lalu menyimpafilenya pada direktori aktif (repository)
* disini kita akan coba buat satu file bernama README.md (text file) ``$ echo “#Latihan 1” >> README.md``
  
  ![echo](https://user-images.githubusercontent.com/57053160/68083012-5e0c0780-fe56-11e9-9867-e1fbd39fc450.png)

* File ``README.md`` berhasil dibuat.
# Menambahkan File baru pada repository
* Untuk menambahkan file yang baru saja dibuat tersebut gunakanperintah git add.
* File README.md berhasil ditambahkan. ``$ git add README.md``
  
  ![git add](https://user-images.githubusercontent.com/57053160/68083073-12a62900-fe57-11e9-87f7-5ebe1e4b74e7.png)

# Commit (Menyimpan perubahan ke database)
* Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah ``$ git commit -m``  ``“komentar commit”``

  ![git commit](https://user-images.githubusercontent.com/57053160/68083091-54cf6a80-fe57-11e9-9f07-655faa702b2b.png)
  
* Perubahan berhasil disimpan
# Membuat repository server
* Server reopsitory yang akan kita gunakan adalah [github.com](https://gitthub.com)
* Anda harus membuat akun terlebih dahulu.
* Pada laman github, klik tombol start a project, atau Dari menu (icon +) klik New Repositor

  ![repository server](https://user-images.githubusercontent.com/57053160/68083101-821c1880-fe57-11e9-8370-3883e32ed354.png)

# Membuat repository server
* Isi nama repositorynya, **misal: labpy1.**
* lalu klik tombol **Create repository**

 ![new repository](https://user-images.githubusercontent.com/57053160/68083116-a5df5e80-fe57-11e9-8532-58b464ad5ba0.png)
 
# Menambahkan Remote Repository
* Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga   dapat diakses oleh banyak user.
* Untuk menambahkan remote repository server, gunakan perintah ``git remote add origin [url]``

  ![git remote](https://user-images.githubusercontent.com/57053160/68083140-f8b91600-fe57-11e9-880c-1244bedd9b0a.png)
  
# Melihat hasilnya pada server repository
* Buka laman ``github.com``,arahkan pada repositori- nya.
* Maka perubahan akan terlihat pada laman tersebut.
![tito](https://user-images.githubusercontent.com/57053160/68083190-ccea6000-fe58-11e9-8ab2-338338cf060f.png)
# Clone Repository
* Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).
* Untuk melakukan cloning, gunakan perintah git clone [url]  
![clone](https://user-images.githubusercontent.com/57053160/68083242-0b801a80-fe59-11e9-8520-95bfd56daa3d.png)
**selesai**
