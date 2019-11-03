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
# Menambahkan File baru pada repository
* Untuk membuat file dapat menggunakan text editor, lalu menyimpafilenya pada direktori aktif (repository)
* disini kita akan coba buat satu file bernama README.md (text file) ``$ echo “#Latihan 1” >> README.md``
* File ``README.md`` berhasil dibuat.
# Menambahkan File baru pada repository
* Untuk menambahkan file yang baru saja dibuat tersebut gunakanperintah git add.
* File README.md berhasil ditambahkan. ``$ git add README.md``
# Commit (Menyimpan perubahan ke database)
* Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah ``$ git commit -m``  ``“komentar commit”``
* Perubahan berhasil disimpan
# Membuat repository server
* Server reopsitory yang akan kita gunakan adalah [github.com](https://gitthub.com)
* Anda harus membuat akun terlebih dahulu.
* Pada laman github, klik tombol start a project, atau Dari menu (icon +) klik New Repositor
# Membuat repository server
* Isi nama repositorynya, **misal: labpy1.**
* lalu klik tombol **Create repository**
# Menambahkan Remote Repository
* Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga   dapat diakses oleh banyak user.
* Untuk menambahkan remote repository server, gunakan perintah ``git remote add origin [url]``
# Melihat hasilnya pada server repository
* Buka laman ``github.com``,arahkan pada repositori- nya.
* Maka perubahan akan terlihat pada laman tersebut.
**selesai**
