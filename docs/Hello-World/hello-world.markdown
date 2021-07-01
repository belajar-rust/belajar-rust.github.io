---
layout: default
title: Hello World! 
nav_order: 3
---

# Hello, World!
Sekarang setelah Anda menginstal Rust, tulis program Rust pertama Anda. Sudah menjadi tradisi ketika mempelajari bahasa baru untuk menulis program kecil yang menampilkan teks Hello, World! ke layar, jadi kita akan melakukan hal yang sama di sini!

<div class="code-example">
Catatan: Dokumentasi ini berasumsi perintah dasar setiap lingkungan atau environment sama. Rust tidak membuat tuntutan khusus untuk pengeditan atau alat yang Anda pakai atau di mana kode Anda berada, jadi jika Anda lebih suka menggunakan lingkungan pengembangan terintegrasi (IDE) daripada baris perintah, jangan ragu untuk menggunakan IDE favorit Anda. Banyak IDE sekarang memiliki pengembangan dan dukungan Rust; periksa dokumentasi IDE untuk detailnya. Baru-baru ini, tim Rust telah berfokus untuk mengaktifkan dukungan IDE di berbagai editor, dan kemajuan telah dibuat dengan cepat. terima kasih untuk team developer Rust.
</div>

### Membuat Folder untuk Rust Project
Anda akan mulai dengan membuat direktori atau folder untuk menyimpan kode Rust Anda. Tidak masalah bagi Rust di mana kode Anda berada, tetapi untuk latihan dan project dalam buku ini, kami sarankan untuk membuat direktori project di direktori home Anda dan menyimpan semua project Anda di sana.

Buka terminal dan masukkan perintah berikut untuk membuat direktori proyek dan direktori untuk "Hello, world!" project dalam direktori project.

Untuk Linux, macOS, dan PowerShell di Windows, masukkan ini:

```
mkdir ~/projects
```

```
cd ~/projects
```

```
mkdir hello_world
```

```
cd hello_world
```

Untuk CMD Windows, masukkan ini:

```
mkdir "%USERPROFILE%\projects"
```

```
cd /d "%USERPROFILE%\projects"
```

```
mkdir hello_world
```

```
cd hello_world
```

### Menulis dan Menjalankan Program Rust
Selanjutnya, buat file sumber baru dan beri nama main.rs. File Rust selalu diakhiri dengan ekstensi .rs. Jika Anda menggunakan lebih dari satu kata dalam nama file Anda, gunakan garis bawah untuk memisahkannya. Misalnya, gunakan hello_world.rs daripada helloworld.rs.

Sekarang buka file main.rs yang baru saja Anda buat dan masukkan kode di Listing 1-1.

Nama file: main.rs

```
fn main() {
    println!("Hello, world!");
}
```
Listing 1-1: Program yang menampilkan Hello, world!

Simpan file dan kembali ke jendela terminal Anda. Di Linux atau macOS, masukkan perintah berikut untuk mengompilasi dan menjalankan file:

```
rustc main.rs
```

```
./main
```

maka program akan menampilkan : 
```
Hello, world!
```

Di Windows, masukkan perintah .\main.exe bukan ./main:

```
rustc main.rs
```

```
.\main.exe
```
maka program juga akan menampilkan

```
Hello, world!
```

Terlepas dari sistem operasi Anda, string Hello, world! harus tampil di terminal. Jika Anda tidak melihat output ini, lihat kembali bagian [Check Versi]({{ site.baseurl }}{% link docs/Memulai/check-versi.markdown %}) atau di [Updating]({{ site.baseurl }}{% link docs/Memulai/updating.markdown %}) ataupun di bagian [Instalasi]({{ site.baseurl }}{% link docs/Memulai/instalasi.markdown %}) untuk mengetahui cara mendapatkan bantuan.

Jika ```Hello, world!``` berhasil mencetak, selamat! Anda telah secara resmi menulis program Rust. Itu membuat Anda menjadi programmer Rust—selamat datang!

### Anatomi Program Rust
Mari kita tinjau secara rinci apa yang baru saja terjadi di “Hello, world!”. Inilah bagian pertama dari teka-teki:

```
fn main() {

}
```

Garis-garis ini mendefinisikan fungsi di Rust. Fungsi utamanya adalah khusus: selalu kode pertama yang berjalan di setiap program Rust yang dapat dieksekusi. Baris pertama mendeklarasikan fungsi bernama main yang tidak memiliki parameter dan tidak mengembalikan apa pun. Jika ada parameter, mereka akan masuk ke dalam tanda kurung, ().

Perhatikan juga bahwa badan fungsi dibungkus dalam tanda kurung kurawal, {}. Karat membutuhkan ini di sekitar semua badan fungsi. Ini adalah gaya yang baik untuk menempatkan kurung kurawal pembuka pada baris yang sama dengan deklarasi fungsi, dengan menambahkan satu spasi di antaranya.

Jika Anda ingin tetap menggunakan gaya standar di seluruh proyek Rust, Anda dapat menggunakan alat pemformat otomatis yang disebut rustfmt untuk memformat kode Anda dalam gaya tertentu. Tim Rust telah menyertakan alat ini dengan distribusi Rust standar, seperti rustc, jadi seharusnya sudah diinstal di komputer Anda! Periksa dokumentasi online untuk lebih jelasnya.

Di dalam fungsi utama adalah kode berikut:

```
println!("Halo dunia!");
```
Baris ini melakukan semua pekerjaan dalam program kecil ini: ia mencetak teks ke layar. Ada empat detail penting yang perlu diperhatikan di sini.

Pertama, gaya Rust adalah indentasi dengan empat spasi, bukan tab.

Kedua, println! memanggil makro Rust. Jika memanggil fungsi, itu akan dimasukkan sebagai println (tanpa !). Kami akan membahas makro Rust secara lebih rinci di Bab 19. Untuk saat ini, Anda hanya perlu mengetahui bahwa menggunakan ! berarti Anda memanggil makro alih-alih fungsi normal.

Ketiga, Anda melihat pesan "Hello, world!". Kami meneruskan string ini sebagai argumen ke println!, dan string tersebut dicetak ke layar.

Keempat, kita akhiri baris dengan titik koma (;), yang menunjukkan bahwa ekspresi ini telah berakhir dan ekspresi berikutnya siap untuk dimulai. Sebagian besar baris kode Rust diakhiri dengan titik koma.

Kompilasi dan Menjalankan Adalah Langkah Terpisah
Anda baru saja menjalankan program yang baru dibuat, jadi mari kita periksa setiap langkah dalam prosesnya.

Sebelum menjalankan program Rust, Anda harus mengompilasinya menggunakan kompiler Rust dengan memasukkan perintah rustc dan memberikannya nama file sumber Anda, seperti ini:

```
rustc main.rs
```
Jika Anda memiliki latar belakang C atau C++, Anda akan melihat bahwa ini mirip dengan gcc atau dentang. Setelah kompilasi berhasil, Rust mengeluarkan biner yang dapat dieksekusi.

Di Linux, macOS, dan PowerShell di Windows, Anda dapat melihat executable dengan memasukkan perintah ls di s