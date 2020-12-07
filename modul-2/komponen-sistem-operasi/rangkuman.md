# Rangkuman Komponen Sistem Operasi

Dari berbagai macam sistem operasi yang ada, tidak semua memiliki komponen-komponen penyusun yang sama. Pada umumnya sebuah sistem operasi modern akan terdiri dari komponen sebagai berikut :

1. Manajemen proses
   Sistem operasi bertanggung jawab atas aktivitas yang berkaitan
   dengan manajemen proses seperti:  
   a. Pembuatan atau penghapusan proses yang dibuat oleh pengguna atau sistem.
   b. Menunda dan melanjutkan proses
   c. Kelengkapan mekanisme untuk sinkronisasi proses
   d. Kelengkapan mekanisme untuk komunikasi proses
   e. Kelengkapan mekanisme untuk pengendalian deadlock

2. Manajemen memori utama
   Sistem operasi memberikan tanggapan terhadap manajemen memori utama untuk aktivitas-aktivitas sebagai berikut:
   a. Menjaga dan memelihara bagian-bagian memori yang sedang digunakan dari yang menggunakan.
   b. Memutuskan proses-proses mana saja yang harus dipanggil ke memori jika masih ada ruang di memori
   c. Mengalokasikan dan mendealokasikan ruang memori jika diperlukan.

3. Manajemen memori sekunder
   Sistem operasi memberikan tanggapan terhadap manajemen penyimpanan sekunder untuk aktivitas-aktivitas sebagai berikut:
   a. Pengaturan ruang kosong.
   b. Alokasi penyimpanan
   c. Penjadwalan disk

4. Manajemen I/O (Input/Output)
   Sistem operasi juga sering disebut device manager, karena sistem operasi mengatur berbagai macam perangkat (device). Fungsi-fungsi sistem operasi untuk sistem I/O:
   a. Penyanggahan (buffering). Menampung data sementara dari/ke perangkat I/O.
   b. Penjadwalan (scheduling). Melakukan penjadwalan pemakaian I/O sistem supaya lebih efisien.
   c. Spooling Meletakkan suatu pekerjaan program pada penyangga, agar setiap perangkat dapat mengaksesnya saat perangkat tersebut siap.
   d. Menyediakan driver perangkat yang umum. Driver digunakan agar sistem operasi dapat memberi perintah untuk melakukan operasi pada perangkat keras I/O yang umum, seperti optical drive, media penyimpanan sekunder dan layar monitor.
   e. Menyediakan driver perangkat yang khusus. Driver digunakan agar sistem operasi dapat memberi perintah untuk melakukan operasi pada perangkat keras I/O tertentu, seperti kartu suara, kartu grafis dan mainboard.

5. Manajemen file
   Sistem operasi memberikan tanggapan terhadap manajemen file untuk aktivitas-aktivitas sebagai berikut:
   a. Pembuatan dan penghapusan file atau direktori
   b. Pemetaan file ke memori sekunder
   c. Backup file ke media penyimpanan yang stabil (non volatile)

6. Proteksi dan keamanan
   Sistem operasi memastikan bahwa suatu program tidak bisa dimodifikasi pada saat program sedang disalin melalui Internet, dengan cara mengisi celah keamanan, pada saat ancaman itu ditemukan. Para pengguna diharapkan untuk berkontribusi untuk mengamankan dengan cara penggunaan notifikasi peringatan pada saat mengunduh program melalui Internet.

7. Manajemen jaringan
   Dukungan terhadap komunikasi data antar perangkat komputer mutlak diperlukan. Pada model sistem terdistribusi, jaringan komputer peer to peer ataupun client server, sistem operasi berfungsi untuk mengatur model komunikasi antar komputer dan komunikasi antar perangkat jaringan.

8. Command Interpreter System
   Command Interpreter System adalah sistem operasi menunggu instruksi dari pengguna (command driven). Program yang dapat membaca instruksi dan mengartikan control statements berdasarkan masukan dari pengguna umumnya disebut : control card interpreter atau command line interpreter pada sistem UNIX sering disebut juga shell atau console. Command Interpreter System sangat bervariasi dari suatu sistem operasi ke sistem operasi yang lain dan disesuaikan dengan tujuan dan teknologi masukkan/keluaran perangkat yang ada. Contohnya: Command Line Interpreter (CLI), Windows (GUI dengan click, drag n drop), pen-based (touch) dan lain-lain.
