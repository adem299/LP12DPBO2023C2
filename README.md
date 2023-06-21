# LP12DPBO2023C2
Saya Ade Mulyana NIM 2108799 mengerjakan LP12 dalam mata kuliah Desain dan Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

## Deskripsi Program
##### Preview Program
<img width="500" src="https://github.com/adem299/LP12DPBO2023C2/assets/100661834/b1cb96bd-6a99-4044-a7f7-80d42d3447ff" >

> 3 main Object game. Player bericon Ninja, Target bergambar pedang/katana, Leaf object bulat warna pink

Untuk program (TMD) kali ini saya menggunakan bahasa program Java dan Arsitektur MVVM (Model View ViewMode) dengan struktur program sebagai berikut:
1. Model
    - DB
    - GameObject
    - KeyController
    - User
    - TableUser
    - Player
    - Target
    - Leaf
2. View
    - Display
    - Menu
3. ViewModel
    - BGM
    - Game
    - Handler
    - ProcessUser

Ketika mulai menjalankan program, program akan menampilkan menu yang merupakan main class dari program ini, Menu ini menampilkan form input dan table isi dari data pemain / user beserta score dan standing nya, data maupun input data baru disini di proses melalui processUser yang mana akan terkoneksi ke database. Selain menampilkan menu juga akan memulai process play musik melalui BGM class dimana musik akan berhenti jika pemain/user memulai game. Untuk memulai game user dapat meninput field username baru, atau melanjutkan sebagai user yang tersedia dari data sebelumnya.
  
Game di mulai program akan menampilkan windows dengan menggunakan class Display dan merender seluruh objeck game yang tersedia disini terdapat 3 object game utama Player, Target / Tempat object player berpijak, dan leaf yang akan jatuh dari atas dengan random (asumsi daun bunga sakura). Dalam game ini terdapat KeyController untuk user dapat menggerakan object Player. Adapun sistem dari game ini yaitu ketika object player menyentuh target (pedang) score akan bertambah berdasarkan ukuran width dari target lebih kecil lebih besar score yang didapat. Ketika Player menyentuh batas atas atau batas bawah dari layar akan terjadi game over, dan seluruh data dari game tadi akan di simpan ke database. Tak hanya itu untuk menghentikan game juga dapat menggunakan tombol Space data akan tersimpan pada database juga.

### Alasan Penggunaan Arsitektur MVVM
Arsitekur MVVM membantu memisahkan dengan jelas logika bisnis dan presentasi aplikasi dari antarmuka pengguna (UI). Pemisahan yang jelas antara logika aplikasi dan antarmuka pengguna membantu menyelesaikan banyak masalah pengembangan dan memfasilitasi pengujian, pemeliharaan, dan pengembangan aplikasi. Itu juga dapat sangat meningkatkan penggunaan kembali kode dan memungkinkan pengembang dan desainer UI untuk berkolaborasi dengan lebih mudah saat mengembangkan suatu aplikasi. Oleh karena Arsitektur MVVM ini sangat cocok pada program kali ini.
