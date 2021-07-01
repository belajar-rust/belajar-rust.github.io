---
layout: home
title: Perkenalan
nav_order: 1
---

# Perkenalan

Berkenalan dengan bahasa pemrograman **Rust** (dibaca "rast"). Bahasa pemrograman ini pertama kali didesign oleh [Graydon Hoare](https://everipedia.org/wiki/lang_en/graydon-hoare) , yang notabene masih dalam perusahaan Mozilla yakni [Mozilla Research](https://research.mozilla.org/). dengan kontribusi dari beberapa orang teman dan koleganya yakni [Dave Herman](https://engineering.linkedin.com/blog/2017/11/getting-to-know-dave-herman) , [Brendan Eich](https://en.wikipedia.org/wiki/Brendan_Eich) dan lainnya. Para designer (baca : designer system) ini memperhalus dan membentuk bahasa pemrograman rust ini dengan mengimplementasikannya pada saat membuat [Servo](https://en.wikipedia.org/wiki/Servo_(software)) yakni engine peramban (baca : browser engine). dan dari sanalah bahasa pemrograman ini meningkat jumlah pemakaiannya di industri ini. dan perusahaan terkemuka seperti [Microsoft](https://en.wikipedia.org/wiki/Microsoft) bereksperimen dengan bahasa dan compiler satu ini, karena dengan fitur aman dan komponen perangkat lunak yang kritis terhadap keselamatan akan terjadinya kesalahan. 

## Untuk Siapa Saja Rust ini ?

**Rust** sangat ideal bagi banyak orang karena berbagai alasan. Mari kita lihat beberapa grup yang paling penting.

### Tim Pengembang (Developer)
**Rust** terbukti menjadi alat yang produktif untuk berkolaborasi di antara tim besar pengembang dengan berbagai tingkat pengetahuan pemrograman sistem. Kode tingkat rendah (*low level programming*) rentan terhadap berbagai kesalahan atau bug halus, yang dalam sebagian besar bahasa lain hanya dapat ditangkap melalui pengujian ekstensif dan tinjauan kode yang cermat oleh pengembang berpengalaman. Di **Rust**, kompiler memainkan peran penjaga gerbang dengan menolak untuk mengkompilasi kode dengan bug yang sulit dipahami ini, termasuk bug konkurensi. Dengan bekerja bersama kompiler, tim dapat menghabiskan waktu mereka dengan fokus pada logika program daripada mengejar bug.

**Rust** juga membawa alat pengembang kontemporer ke dunia pemrograman sistem:

**Cargo**, alat manajemen dan alat pembangunan yang disertakan, membuat penambahan, kompilasi, dan pengelolaan dependensi tidak menyulitkan dan konsisten di seluruh ekosistem **Rust**.
**Rustfmt** memastikan gaya pengkodean yang konsisten di seluruh pengembang atau developer yang memakai format yang sama.
Rust Language Server mendukung integrasi Integrated Development Environment (IDE) untuk penyelesaian kode dan pesan kesalahan sebaris.
Dengan menggunakan ini dan alat lainnya di ekosistem Rust, pengembang dapat menjadi produktif saat menulis kode tingkat sistem.

### Siswa
**Rust** adalah untuk siswa dan mereka yang tertarik untuk belajar tentang konsep sistem. Menggunakan **Rust**, banyak orang telah belajar tentang topik seperti pengembangan sistem operasi. Masyarakat sangat ramah dan senang menjawab pertanyaan siswa. Melalui upaya seperti buku ini, tim **Rust** ingin membuat konsep sistem lebih mudah diakses oleh lebih banyak orang, terutama mereka yang baru mengenal pemrograman.

### Perusahaan
Ratusan perusahaan, besar dan kecil, menggunakan Rust dalam produksi untuk berbagai tugas. Tugas-tugas itu termasuk alat baris perintah, layanan web, alat DevOps, perangkat tertanam, analisis dan transcoding audio dan video, cryptocurrency, bioinformatika, mesin pencari, aplikasi Internet of Things, pembelajaran mesin, dan bahkan bagian utama dari browser web Firefox.

### Pengembang Sumber Terbuka (Open Source Developer)
**Rust** adalah untuk orang yang ingin membangun bahasa pemrograman Rust, komunitas, alat pengembang, dan perpustakaan. Kami ingin Anda berkontribusi pada bahasa Rust.

### Orang yang Menyukai dan Menghargai Kecepatan dan Stabilitas
**Rust** adalah untuk orang-orang yang mendambakan kecepatan dan stabilitas dalam suatu bahasa. Dengan kecepatan, yang kami maksud adalah kecepatan program yang dapat Anda buat dengan Rust dan kecepatan di mana Rust memungkinkan Anda menulisnya. Pemeriksaan kompiler Rust memastikan stabilitas melalui penambahan fitur dan refactoring. Ini berbeda dengan kode lama yang rapuh dalam bahasa tanpa pemeriksaan ini, yang sering kali takut dimodifikasi oleh pengembang. Dengan berjuang untuk abstraksi tanpa biaya, fitur tingkat tinggi yang dikompilasi ke kode tingkat yang lebih rendah secepat kode yang ditulis secara manual, Rust berupaya membuat kode aman menjadi kode cepat juga.

Bahasa **Rust** berharap dapat mendukung banyak pengguna lain juga; yang disebutkan di sini hanyalah beberapa pemangku kepentingan terbesar. Secara keseluruhan, ambisi Rata-Rata Rust adalah untuk menghilangkan kompromi yang telah diterima oleh programmer selama beberapa dekade dengan memberikan keamanan dan produktivitas, kecepatan dan ergonomi. Cobalah Rust dan lihat apakah pilihannya cocok untuk Anda.