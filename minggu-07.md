## PERTEMUAN MINGGU KE-6 Teknologi Virtualisasi dan Container - Docker 

### OS-level virtualization 
OS-level virtualization atau Virtualisasi tingkat OS mengacu pada paradigma sistem operasi di mana kernel memungkinkan adanya beberapa instance ruang *solated user*.  Contoh instance tersebut, disebut wadah (container) LXC, Solaris containers, Docker), Zones (Solaris containers), virtual private servers (OpenVZ), partitions, virtual environments(VEs), virtual kernels (DragonFly BSD), or jails (FreeBSD jail or chroot jail). 

mungkin terlihat seperti komputer sungguhan dari sudut pandang program yang berjalan di dalamnya. Program komputer yang berjalan pada sistem operasi biasa dapat melihat semua sumber daya (perangkat yang terhubung, file dan folder, pembagian jaringan, daya CPU, kemampuan perangkat keras yang dapat diukur) dari komputer tersebut. Namun, program yang berjalan di dalam wadah (container) hanya dapat melihat konten dan perangkat kontainer yang ditugaskan ke wadah.

#### Operation
Pada sistem operasi pada PC umumnya sebuah program komputer dapat melihat (meskipun mungkin tidak dapat mengakses) semua sumber daya sistem mereka termasuk:

* Kemampuan perangkat keras yang dapat digunakan, seperti CPU dan koneksi jaringan
* Data yang dapat dibaca atau ditulis, seperti file, folder, dan berbagi jaringan
* Periferal yang terhubung dapat berinteraksi dengannya, seperti webcam, printer, scanner, atau fax. 

Dengan sistem operasi-virtualisasi, atau *containerization* memungkinkan untuk menjalankan program di dalam wadah, yang hanya dialokasikan sebagian sumber daya. 

*containerization* memiliki kemiripan dengan virtualisasi aplikasi: Pada yang terakhir, hanya satu program komputer yang ditempatkan dalam container yang terisolasi dan isolasi hanya berlaku untuk sistem file. 

### Docker
setelah memahami tentang apa itu OS-level virtualization berikutnya akan dipelajari tentang docker. menurut [dokumentasi docker](https://docs.docker.com/get-started/overview/) Docker adalah platform terbuka untuk mengembangkan, mengirim, dan menjalankan aplikasi. Docker memungkinkan untuk memisahkan aplikasi dari infrastruktur sehingga dapat mengirimkan perangkat lunak dengan cepat. 

#### Docker Platform  
Docker menyediakan kemampuan untuk mengemas (package) dan menjalankan aplikasi dalam lingkungan yang terisolasi yang disebut kontainer. Isolasi dan keamanan memungkinkan Anda menjalankan banyak kontainer secara bersamaan pada host tertentu.  

Docker menyediakan alat dan platform untuk mengelola siklus hidup dari kontainer:

* mengembangkan aplikasi dan komponen pendukungnya menggunakan kontainer.
* kontainer menjadi unit untuk mendistribusikan dan menguji aplikasi.
* men-*deploy* aplikasi ke lingkungan produksi, sebagai kontainer atau layanan yang dirancang. Ini berfungsi sama apakah lingkungan produksi adalah pusat data lokal, penyedia cloud, atau gabungan keduanya. 


#### Docker Engine 
Docker Engine adalah aplikasi client-server dengan komponen utama sebagai berikut:
* Server yang merupakan jenis long-running program yang disebut proses daemon (perintah dockerd).

* REST API yang menentukan antarmuka yang dapat digunakan program untuk berkomunikasi dengan daemon dan memerintahkannya apa yang harus dilakukan.

* Sebuah antarmuka baris perintah (CLI) client (perintah docker).