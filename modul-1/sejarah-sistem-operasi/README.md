# Sejarah Sistem Operasi

Perkembangan Sistem Operasi sangat dipengaruhi oleh perkembangan hardware. Fasilitasi penggunaan hardware adalah sebuah alasan mengapa sistem operasi dikembangkan. Dengan kata lain, ketika hardware berkembang dan bertambah maju, maka harus diikuti oleh kemajuan pengembangan sistem operasi.

## Evolusi Sistem Operasi

Evolusi sistem operasi dari waktu ke waktu adalah sebagai berikut.

1. Generasi ke-nol (1940)
   a. Komponen utama tabung hampa udara
   b. Sistem komputer belum menggunakan sistem operasi
   c. Semua operasi komputer dilakukan secara manual melalui plugboards, dan hanya bisa digunakan untuk menghitung (+,- dan \*)
2. Generasi ke-satu/pertama (1950)
   a. Komponen utama transistor
   b. Sistem operasi berfungsi terutama sebagai pengatur pergantian antar job berikutnya lebih efisien. Dalam masa ini muncul konsep batch system (semua job sejenis dikumpulkan jadi satu).
   c. Input memakai punch card.
3. Generasi ke-dua (1960)
   a. Komponen utama IC.
   b. Berkembang konsep-konsep:
   (1) Multiprogramming, satu prosesor mengerjakan banyak program yang ada di memori utama.
   (2) Multiprocessing, satu job dikerjakan oleh banyak prosesor untuk meningkatkan utilitas.
   (3) Spooling (Simultaneous Peripheral Operation On Line), bertindak sebagai buffer saja, dan mampu menerima pesanan meskipun belum akan dikerjakan.
   (4) Device Independence, masing-masing komponen memiliki sifat yang saling berbeda (misal: tiap-tiap printer memiliki driver).
   (5) Time sharing atau multitasking.
   (6) Real time system, berguna sebagai kontrol bagi mesin-mesin.
4. Generasi ketiga (1970)
   a. Komponen utama VLSI (Very Large Scale Integrated Circuit).
   b. Menggunakan konsep general purpose system, sehingga sistem operasi menjadi sangat kompleks, mahal dan sulit untuk dipelajari.
5. Generasi keempat (pertengahan 1970-1an hingga sekarang)
   a. PC (Personal Computer) makin populer.
   b. Sistem Operasi sudah dengan jaringan komputer dengan tujuan: data sharing, hardware sharing dan program sharing.
   c. User interface semakin mudah digunakan (user friendly) tanpa mengurangi kinerja komputer.

## SISTEM AWAL (SERIAL PROCESSING)

Komputer-komputer awal secara fisik berukuran besar dan dijalankan dari suatu console. Console terdiri dari lampu-lampu, tombol-tombol, perangkat masukan (card reader), dan printer. Seorang programmer yang juga merangkap sebagai operator, menulis program dan menjalankan program tersebut langsung dari console-nya. Program tersebut dimuatkan dalam memori untuk menjalankan setiap instruksi, biasanya per instruksi dari kartu plong. Kemudian ada suatu tombol di console yang harus ditekan untuk menjalankan keseluruhan program tersebut. Jika terjadi error pada program tersebut, yang diketahui dengan menyalanya lampu indikator tertentu maka programmer dapat menghentikan program tersebut dan memeriksa isi memori dan register-registernya serta men-debug program tersebut secara langsung dari console. Jika tidak terjadi error pada waktu menjalankan program tersebut, maka keluaran program tersebut dapat dicetak atau dibuatkan kartu plong-nya untuk pencetakan di kemudian hari.

Karena kebutuhan yang beragam, software dan hardware tambahan banyak dikembangkan, Card reader, line printer dan magnetic tape menjadi hal yang biasa pada waktu itu. Assembler, linker, dan loader didesain untuk memudahkan pemrograman. Fungsi-fungsi yang sering digunakan dalam pemrograman kemudian disatukan dan disimpan tersendiri sebagai library sehingga programmer tidak perlu menulis ulang fungsi-fungsi tersebut (Binanto, 2005)

## SISTEM BATCH SEDERHANA

Dengan sistem awal (Serial Processing) ternyata banyak waktu CPU yang terbuang. Sering CPU tidak terpakai (idle) karena programmer atau operator sedang mengganti atau memasang tape. Padahal pada saat itu harga komputer serta biaya perawatan dan operasionalnya sangat mahal. Karena hal tersebut kemudian ditemukan sebuah cara, yaitu mengumpulkan job-job yang sejenis untuk dieksekusi oleh CPU sebagai suatu group atau kumpulan job. Dengan sistem batch sederhana ini maka pemakai tidak punya akses langsung ke mesin komputer.

**[Rangkuman](./rangkuman.md)**
