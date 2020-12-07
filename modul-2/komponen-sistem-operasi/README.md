# Komponen Sistem Operasi

Sistem Operasi menangani perangkat keras, perangkat lunak, sampai menangani pengguna. Hal tersebut menyebabkan sebuah sistem operasi memiliki banyak sekali komponen-komponen tersendiri yang memiliki fungsinya masing-masing sering disebut juga modular karena dapat dikembangkan secara terpisah. Seluruh komponen yang menyusun sistem operasi tersebut saling bekerja sama untuk satu tujuan, yaitu efisiensi kerja seluruh perangkat komputer dan kenyamanan dalam penggunaan sistem operasi. Dari berbagai macam sistem operasi yang ada, tidak semua memiliki komponen-komponen penyusun yang sama (Masyarakat Digital Gorong Royong, 2008). Pada umumnya sebuah sistem operasi modern akan terdiri dari komponen sebagai berikut.

## MANAJEMEN PROSES

Proses merupakan program yang sedang dieksekusi. Sedangkan program adalah kumpulan instruksi yang ditulis ke dalam bahasa yang dimengerti sistem operasi. Sebuah proses membutuhkan sejumlah sumber daya untuk menyelesaikan tugasnya. Sumber daya tersebut dapat berupa CPU time, alamat memori, berkas-berkas, dan perangkat-perangkat Masukan/Keluaran (Input/Output, dalam Modul 1).
Sistem Operasi mengalokasikan sumber daya tersebut ketika proses sedang dijalankan. Ketika proses tersebut berhenti dijalankan, sistem operasi akan mengambil alih semua sumber daya agar bisa digunakan kembali oleh proses lainnya. Sistem operasi bertanggung jawab atas aktivitas yang berkaitan dengan manajemen proses seperti:

### Pembuatan atau Penghapusan Proses yang Dibuat oleh Pengguna atau Sistem

Sistem operasi bertugas mengalokasikan sumber daya yang dibutuhkan oleh sebuah proses yang dibuat oleh pengguna atau sistem. Sistem operasi mengambil sumber daya itu kembali setelah proses tersebut selesai agar dapat digunakan oleh proses lainnya.

### Menunda dan Melanjutkan Proses

Sistem operasi akan mengatur proses apa yang harus dijalankan terlebih dahulu berdasarkan prioritas dari proses-proses yang ada. Apabila terdapat dua proses atau lebih yang mengantri untuk dijalankan, sistem operasi akan mendahulukan proses yang memiliki prioritas yang paling besar.

### Kelengkapan Mekanisme untuk Sinkronisasi Proses

Sistem operasi mengatur jalannya beberapa proses yang dieksekusi bersamaan. Tujuannya adalah menghindarkan terjadinya inkonsistensi data karena pengabsisan data yang sama, juga untuk mengatur urutan jalannya proses agar setiap proses berjalan dengan lancar.

### Kelengkapan Mekanisme untuk Komunikasi Proses

Sistem operasi menyediakan mekanisme agar beberapa proses dapat saling berinteraksi dan berkomunikasi satu sama lain tanpa menyebabkan terganggunya proses lainnya.

### Kelengkapan Mekanisme untuk Pengendalian Deadlock

Deadlock adalah keadaan dimana sistem seperti terhenti karena setiap proses memiliki sumber daya yang tidak bisa dibagi dan menunggu untuk mendapatkan sumber daya yang sedang dimiliki oleh proses lain. Saling menunggu inilah yang disebut deadlock (kebuntuan). Sistem operasi harus bisa mencegah, menghindari, dan mendeteksi adanya deadlock. Jika deadlock terjadi, sistem operasi juga harus dapat memulihkan kondisi sistemnya.

## MANAJEMEN MEMORI UTAMA

Sistem operasi memiliki tugas untuk mengatur bagian memori yang sedang digunakan dan mengalokasikan jumlah dan alamat memori yang diperlukan, baik untuk program yang akan berjalan maupun untuk sistem operasi itu sendiri. Tujuan manajemen memori utama adalah agar utilitas CPU meningkat dan untuk meningkatkan efisiensi pemakaian memori.

Memori utama atau dikenal sebagai memori adalah sebuah array yang besar dari word atau byte yang ukurannya mencapai ratusan, ribuan, atau bahkan jutaan. Setiap word atau byte mempunyai alamat tersendiri. Memori utama berfungsi sebagai tempat penyimpanan instruksi/data yang akses datanya digunakan oleh CPU dan perangkat I/O. Memori utama termasuk tempat penyimpanan data yang bersifat volatile (tidak permanen), yaitu data akan hilang kalau komputer dimatikan.
Sistem operasi memberikan tanggapan terhadap manajemen memori utama untuk aktivitas-aktivitas sebagai berikut.

1. Menjaga dan memelihara bagian-bagian memori yang sedang digunakan dari yang menggunakan.
2. Memutuskan proses-proses mana saja yang harus dipanggil ke memori jika masih ada ruang di memori.
3. Mengalokasikan dan mendealokasikan ruang memori jika diperlukan.

## MANAJEMEN MEMORI SEKUNDER

Memori sekunder/penyimpanan sekunder adalah sarana penyimpanan yang berada satu tingkat di bawah memori utama sebuah komputer. Memori sekunder tidak memiliki hubungan langsung dengan prosesor melalui bus, sehingga harus melewati perangkat I/O.

Sarana penyimpanan sekunder memiliki fungsi-fungsi sebagai berikut:

1. Menyimpan Berkas secara Permanen
   Data atau berkas diletakkan secara fisik pada piringan magnet dari disk, yang tidak hilang walaupun komputer dimatikan (non volatile).

2. Menyimpan Program yang Belum Dieksekusi Prosesor
   Jika sebuah program ingin dieksekusi oleh prosesor, program tersebut dibaca dari disk, lalu diletakkan di memori utama komputer untuk selanjutnya dieksekusi oleh prosesor menjadi proses.

3. Memori Virtual
   Mekanisme sistem operasi untuk menjadikan beberapa ruang kosong dari disk menjadi alamat-alamat memori virtual, sehingga prosesor bisa menggunakan memori virtual ini seolah-olah sebagai memori utama. Akses prosesor ke memori virtual menjadi jauh lebih lambat dan menghambat kinerja komputer karena letaknya di penyimpanan sekunder.

Sistem operasi memiliki peran penting dalam manajemen penyimpanan sekunder karena bertujuan untuk keamanan, efisiensi, dan optimalisasi penggunaan sarana penyimpanan sekunder. Sistem operasi memberikan tanggapan terhadap manajemen penyimpanan sekunder untuk aktivitas-aktivitas sebagai berikut:

_a. Pengaturan ruang kosong._
Sistem operasi mengatur ruangan pada disk yang belum terpakai atau ruang yang kosong akibat penghapusan data. Sistem operasi membuat daftar ruang-ruang kosong apabila ada berkas baru yang ingin disimpan, maka ruang bebas dicari pada daftar ini. Untuk membuat berkas baru, sistem mencari ke daftar tersebut untuk mencarikan ruang kosong yang dibutuhkan.

_b. Alokasi penyimpanan_
Sistem operasi mengalokasikan penyimpanan ke dalam memori sekunder misalnya magnetic disk, harddisk, floppy disk, optical disk dan flash memory.

_c. Penjadwalan disk._
Sistem operasi melakukan penjadwalan disk dalam proses membaca, mengubah, dan menghapus data di penyimpanan sekunder. Proses pelayanan I/O dari atau menuju disk dengan urutan yang tepat membawa informasi-informasi operasi input atau output, alamat disk/memori untuk proses tersebut, dan jumlah bytes yang akan ditransfer.

## MANAJEMEN I/O (INPUT/OUTPUT)

Sistem operasi juga sering disebut device manager, karena sistem operasi mengatur berbagai macam perangkat (device). Fungsi -fungsi sistem operasi untuk sistem I/O:

1. Penyanggahan (buffering) yaitu menampung data sementara dari/ke perangkat I/O.
2. Penjadwalan (scheduling) yaitu melakukan penjadwalan pemakaian I/O sistem supaya lebih efisien.
3. Spooling Meletakkan suatu pekerjaan program pada penyangga, agar setiap perangkat dapat mengaksesnya saat perangkat tersebut siap.
4. Menyediakan driver perangkat yang umum. Driver digunakan agar sistem operasi dapat memberi perintah untuk melakukan operasi pada perangkat keras I/O yang umum, seperti optical drive, media penyimpanan sekunder dan layar monitor.
5. Menyediakan driver perangkat yang khusus. Driver digunakan agar sistem operasi dapat memberi perintah untuk melakukan operasi pada perangkat keras I/O tertentu, seperti kartu suara, kartu grafis dan mainboard.

## MANAJEMEN FILE

File atau berkas adalah representasi program dan data yang berupa kumpulan informasi yang saling berhubungan dan disimpan di perangkat penyimpanan. Sistem operasi harus dapat melakukan operasi-operasi pada berkas, seperti membuka, membaca, menulis, dan menyimpan berkas tersebut pada sarana penyimpanan sekunder.
Sistem operasi memberikan tanggapan terhadap manajemen file untuk aktivitas-aktivitas sebagai berikut:

1. Pembuatan dan Penghapusan File atau Direktori
   Sistem operasi menunjukkan tempat lokasi berkas atau direktori tersebut diletakkan. Kemudian sistem operasi akan membuat entri yang berisi nama berkas dan lokasi pada sistem berkas. Sistem operasi mencari letak berkas atau direktori yang akan dihapus dari sistem berkas kemudian menghapus seluruh entry berkas tersebut, agar tempat dari berkas tersebut dapat digunakan oleh berkas lainnya.

2. Pemetaan File ke Memori Sekunder
   Sistem operasi mengatur lokasi fisik tempat penyimpanan berkas pada sarana penyimpanan sekunder.

3. Backup File ke Media Penyimpanan yang Stabil (Non Volatile)
   Sistem operasi menyimpan file ke media penyimpanan yang stabil dimana file tersebut tidak akan pernah hilang walaupun tidak mendapatkan daya listrik.

## PROTEKSI DAN KEAMANAN

Ketika seseorang tidak memiliki wewenang mencoba menggunakan atau memodifikasi file/berkas, orang tersebut dapat mencoba mengganggu penggunaan berkas dengan beberapa peran sebagai pengguna yang berwenang dengan program mereka.
Sistem operasi harus menggagalkan upaya tersebut. Fungsi proteksi didesain untuk melawan ancaman penggunaan yang tidak sah atau gangguan yang diakibatkan oleh pengguna sistem komputer; sedangkan fungsi keamanan didesain untuk melawan ancaman serupa yang dilakukan oleh orang-orang di luar kendali sistem operasi.

Pada saat fungsi sistem komputer dalam keadaan terisolasi, permasalahan keamanan dan proteksi dapat dengan mudahnya terpisahkan. Sistem operasi memverifikasi identitas seseorang melalui pemeriksaan kode sandi pada saat pengguna login. Prosedur ini disebut Authentication atau Otentifikasi. Oleh karena itu, ancaman sekuriti tidak akan muncul di dalam sistem apabila prosedur otentifikasi akurat. Sebuah file akan dapat dieksekusi oleh sebuah program yang memiliki perlindungan dari ancaman apabila ada seorang pengguna yang memprakarsai suatu program dan tidak berhak untuk mengakses suatu file. Sistem file melawan ancaman ini dengan cara menggagalkan program.

Pada saat sistem komputer yang terhubung Internet, dan seorang pengguna mengunduh suatu program melalui Internet, terdapat hal berbahaya yaitu sebuah program yang kemungkinan disusupi dengan program lain yang mempengaruhi sumber daya komputer dalam sistem. Ancaman keamanan ini nyata karena adanya campur tangan yang disebabkan oleh seseorang dari luar sistem yang disebut Intruder atau penyelundup. Siapa pun yang hendak menulis atau memodifikasi program yang telah diunduh akan mendapatkan risiko ancaman keamanan melalui Trojan horse.

Trojan adalah suatu program yang dirancang untuk melakukan suatu serangan namun terselubung dengan baik dan merupakan jenis lain dari malware (malicious code). Malware adalah kumpulan kode untuk merusak, mengganggu, mencuri, atau menimbulkan dampak “buruk” pada data, host, atau jaringan. Trojan horse adalah kuda kayu Yunani yang digunakan untuk menyusup ke dalam Troy. Pengguna biasanya tidak sadar telah terjangkit Trojan, karena semua program dapat berjalan dengan baik. Tujuan Trojan sendiri bukanlah merusak data atau mencuri informasi melainkan untuk menjadi pintu celah keamanan agar malware dapat masuk ke dalam sebuah sistem.

Ancaman keamanan lainnya yaitu virus komputer yang menyebar dengan menyisipkan salinan dirinya ke dalam program lain dan menjadi bagian dari program tersebut. Virus dapat menyebar dari satu komputer ke komputer lain, dari program yang sudah terinfeksi. Virus dapat menyebabkan kerusakan data atau program. Hampir semua virus melekat pada sebuah file executable, yang berarti virus mungkin ada pada sebuah sistem tetapi tidak akan aktif atau dapat menyebar sampai pengguna menjalankan atau membuka file host berbahaya atau membuka program tersebut.

Adapun tingkatan lain dari ancaman keamanan komputer adalah Worm. Worm adalah sebuah program komputer yang dapat menggandakan dirinya secara sendiri dalam sistem komputer. Worm merupakan evolusi dari virus komputer. Worm tidak membutuhkan sebuah program atau file yang terinfeksi dalam proses penyebaran. Teknik yang digunakan oleh worm yaitu mencari celah keamanan pada sistem target atau juga menggunakan trik kecil agar kita menjalankan worm, seperti link download yang menginstall program tertentu.

Sistem operasi memastikan bahwa suatu program tidak bisa dimodifikasi pada saat program sedang disalin melalui Internet dengan cara mengisi celah keamanan pada saat ancaman itu ditemukan. Para pengguna diharapkan berkontribusi untuk mengamankan komputernya dengan cara penggunaan notifikasi peringatan pada saat mengunduh program melalui Internet.

## MANAJEMEN JARINGAN

Dukungan terhadap komunikasi data antar perangkat komputer mutlak diperlukan. Pada model sistem terdistribusi dan jaringan komputer peer to peer ataupun client server, sistem operasi berfungsi untuk mengatur model komunikasi antar komputer dan komunikasi antar perangkat jaringan.

Jaringan komputer menyediakan akses bagi pengguna ke bermacam sumber daya sistem pada jaringan. Akses tersebut menyebabkan proses komputasi semakin cepat, peningkatan ketersediaan data dan peningkatan kemampuan.

Sistem terdistribusi adalah sekumpulan prosesor yang tidak berbagi memori atau clock. Setiap prosesor memiliki memori dan clock sendiri. Prosesor tersebut terhubung melalui jaringan komunikasi dan menyediakan akses ke pengguna ke berbagai sumber daya sistem. Suatu sistem operasi terdistribusi yang sejati adalah yang berjalan pada beberapa buah mesin, yang tidak melakukan sharing memori, tetapi terlihat oleh pengguna sebagai satu buah komputer.

Perbedaan sistem operasi jaringan dan sistem operasi terdistribusi adalah setiap komputer memiliki sistem operasi sendiri, memiliki file sendiri dimana data disimpan. Sistem operasi masing-masing komputer dapat berbeda, pada file system dapat digunakan dengan dukungan NFS. NFS atau Network File System adalah sekumpulan protokol yang digunakan untuk mengakses beberapa sistem berkas melalui jaringan. NFS merupakan sebuah implementasi dan spesifikasi dari sebuah perangkat lunak untuk mengakses remote file melalui jaringan Local Area Network (LAN) atau Wide Area Network (WAN).

## COMMAND-INTERPRETER SYSTEM

Command Interpreter System adalah sistem penerjemah perintah tekstual dari pengguna untuk dijalankan di sistem operasi. Program yang dapat membaca instruksi dan mengartikan control statements berdasarkan masukan dari pengguna umumnya disebut : control card interpreter atau command line interpreter pada sistem UNIX sering disebut juga shell atau console. Command Interpreter System sangat bervariasi dari suatu sistem operasi ke sistem operasi yang lain dan disesuaikan dengan tujuan dan teknologi masukkan/keluaran perangkat yang ada. Contohnya: command line interpreter (CLI), Windows (GUI dengan click, drag n drop), pen-based (touch) dan lain-lain.

### Shell

Jika kita ingin berkomunikasi secara interaktif dengan sistem operasi melalui terminal (layar monitor) dan berkomunikasi secara interaktif dengan sistem operasi melalui system call, maka yang dibutuhkan adalah shell.

Dapat dikatakan juga bahwa shell adalah suatu antarmuka pemakai komputer ke sistem operasi, yang merupakan tampilan utama antara pemakai yang duduk di depan terminal (layar monitor) dengan sistem operasi.

Ketika pemakai mulai berinteraksi dengan komputer, maka shell dimulai. Shell mempunyai terminal sebagai standar masukkan dan standar keluaran. Shell dimulai dengan menampilkan prompt, sebuah karakter dollar ($) atau karakter pagar (#) ketika sebagai root di Linux atau UNIX; jika di DOS/Windows dimulai dengan A:\>, C:\>, atau drive letter yang lain. Hal ini sebenarnya memberitahu kepada pemakai bahwa shell sudah menunggu masukan perintah.

### Date

Maka shell akan membuat proses dan menjalankan program date sebagai proses berjalan, shell menunggu program tersebut sampai berhenti. Ketika proses selesai, shell menampilkan prompt lagi dan siap membaca baris masukan berikutnya.

### System Call

Pada dasarnya system call dapat dikelompokkan dalam 5 kategori sebagai berikut.
\*>TODO : Add

### Kontrol Proses

Hal-hal yang dilakukan adalah sebagai berikut.
a. Mengakhiri (end) dan membatalkan (abort).
b. Mengambil (load) dan eksekusi (execute).
c. Membuat dan mengakhiri proses.
d. Menentukan dan mengeset atribut proses.
e. Wait for time.
f. Wait event, signal event.
g. Mengalokasikan dan membebaskan memori.

Contoh: Sistem operasi pada MS-DOS menggunakan sistem single-tasking yang memiliki command interpreter yang akan bekerja pada saat start. Karena single-tasking, maka akan menggunakan metode yang sederhana untuk menjalankan program dan tidak akan membuat proses baru.

### Manipulasi File

Hal-hal yang dilakukan:
a. Membuat dan menghapus file;
b. Membuka dan menutup file
c. Membaca, menulis, dan mereposisi file;
d. Menentukan dan mengeset atribut file;

### Manipulasi Device

Hal-hal yang dilakukan:
a. Meminta dan membebaskan device;
b. Membaca, menulis, dan mereposisi file;
c. Menentukan dan mengeset atribut device;

### Informasi Lingkungan

a. Mengambil atau mengeset waktu atau tanggal;
b. Mengambil atau mengeset sistem data;
c. Mengambil atau mengeset proses, file, atau atribut-atribut device;

### Komunikasi

Hal-hal yang dilakukan
a. Membuat dan menghapus sambungan komunikasi;
b. Mengirim dan menerima pesan;
c. Mentransfer satu informasi;

**[Rangkuman](./rangkuman.md)**
