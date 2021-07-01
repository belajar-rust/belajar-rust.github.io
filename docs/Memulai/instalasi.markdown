---
layout: default
title: Instalasi 
nav_order: 1
parent: Memulai
---

## Instalasi

Langkah pertama adalah menginstal **Rust**. Kita akan mengunduh **Rust** melalui **rustup**, alat baris perintah (Command Line Interface) untuk mengelola versi **Rust** dan alat terkait. Kita memerlukan koneksi internet untuk mengunduh.

<div class="code-example">
Catatan : Jika Anda memilih untuk tidak menggunakan rustup karena alasan tertentu, silahkan lihat <a href="https://www.rust-lang.org/tools/install">halaman instalasi Rust</a> untuk opsi lainnya.
</div>

Langkah-langkah berikut menginstal versi stabil terbaru dari kompiler Rust. Jaminan stabilitas Rust memastikan bahwa semua contoh dalam dokumentasi yang dikompilasi akan terus dikompilasi dengan versi Rust yang lebih baru. Output mungkin sedikit berbeda antar versi, karena Rust sering mengupdate pesan kesalahan atau error dan peringatan. Dengan kata lain, setiap versi Rust yang lebih baru dan stabil yang Anda instal menggunakan langkah-langkah ini akan berfungsi seperti yang diharapkan dengan konten dokumentasi ini.

Notasi Baris Perintah
Dalam bab ini dan di seluruh dokumen ini, kami akan menunjukkan beberapa perintah yang digunakan di terminal. Baris yang harus Anda masukkan di terminal semuanya dimulai dengan **$**. Anda tidak perlu mengetikkan karakter **$**; ini menunjukkan awal dari setiap perintah. Baris yang tidak dimulai dengan **$** biasanya menunjukkan output dari perintah sebelumnya. Selain itu, contoh khusus PowerShell akan menggunakan **>** daripada **$**.

### Menginstal rustup di Linux atau macOS (Varian *Nix OS)
Jika Anda menggunakan Linux atau macOS, buka terminal dan masukkan perintah berikut:

```
curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
```

Perintah ini akan mengunduh skrip dan memulai instalasi alat ```rustup```, yang menginstal versi stabil terbaru dari Rust. Anda mungkin dimintai kata sandi. Jika instalasi berhasil, baris berikut akan muncul:

```
Rust is installed now. Great!
```

Selain itu, kamu memerlukan semacam tautan. Kemungkinan sudah diinstal, tetapi ketika kamu akan mencoba untuk mengkompilasi program Rust dan mendapatkan kesalahan yang menunjukkan bahwa linker tidak bisa dijalankan, itu berarti linker tidak diinstal pada sistem dan kamu harus menginstalnya secara manual. Kompiler C biasanya datang dengan tautan yang benar. Periksa dokumentasi platform kamu untuk mengetahui cara menginstal compiler C. Juga, beberapa paket Rust umum bergantung pada kode C dan akan membutuhkan kompiler C. Oleh karena itu, mungkin bisa untuk menginstalnya sekarang.

### Menginstal rustup di Windows
Di Windows, buka https://www.rust-lang.org/tools/install dan ikuti petunjuk untuk menginstal Rust. Pada titik tertentu dalam penginstalan, Anda akan menerima pesan yang menjelaskan bahwa Anda juga memerlukan build tools C++ untuk Visual Studio 2013 atau yang lebih baru. Cara termudah untuk mendapatkan alat pembangunan adalah dengan memasang Alat Build untuk Visual Studio 2019. Ketika ditanya workloads mana yang harus dipasang, pastikan "C++ build tools" dipilih dan bahwa Windows 10 SDK dan komponen paket bahasa Inggris disertakan.

Sisa dokumentasi ini menggunakan perintah yang berfungsi di cmd.exe dan PowerShell. Jika ada perbedaan spesifik, kami akan menjelaskan mana yang akan digunakan.