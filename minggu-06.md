## PERTEMUAN MINGGU KE-6 Data as a Service 

Dalam komputasi, data as a service, atau DaaS, diaktifkan oleh software as a service (SaaS). seperti pada semua layanan teknologi as a service (aaS), DaaS dibangun berdasarkan konsep bahwa produk datanya dapat diberikan kepada pengguna sesuai permintaan,terlepas dari pemisahan geografis atau organisasi antara penyedia dan konsumen. 


### Keunutungan dari DaaS 
* Agility pengguna dapat bergerak dengan cepat, karena akses data yang sederhana, ddan tidak membutuhkan pengetahuan luas tentang data yang mendasari. Struktur data dan persyaratan khusus lokasi dapat dimodifikasi sesuai kebutuhan pengguna. 
* Cost-effectiveness penyedia dapat membangun basis dengan para ahli data dan *outsourcing* pada lapisan presentasi (presentation layer), yang membuat antarmuka pengguna sangat hemat biaya dan membuat permintaan perubahan pada lapisan presentasi jauh lebih layak.
* Data Quality akses data dikendalikan melalui layanan data, yang cenderung meningkatkan kualitas data, karena ada satu titik untuk pembaruan.  


## CLOUD DATABASE
berbicara mengenai Data maka tidak jauh dengan database, pada teknologi cloud computing terdapat pula databasenya atau yang sering disebut *cloud database*. *cloud database* atau Basis data cloud adalah basis data yang biasanya berjalan pada platform komputasi awan, dan akses ke basis data disediakan sebagai layanan (as-a-service).  

### Arsitektur dan karakteristik umum 
* Sebagian besar layanan database menawarkan konsol berbasis web, yang dapat digunakan *end user* untuk menyediakan dan mengkonfigurasi instance database. 
* Layanan database terdiri dari komponen database-manager, yang mengontrol instance database yang mendasarinya menggunakan service API. service API yang terbuka ke pengguna akhir, dan memungkinkan pengguna untuk melakukan perintah pemeliharaan dan penskalaan pada instance basis data mereka. 
* software-stack yang mendasarinya biasanya stack mencakup sistem operasi, database, dan perangkat lunak pihak ketiga yang digunakan untuk mengelola database. Penyedia layanan bertanggung jawab untuk menginstal, patching (menambal), dan memperbarui software stack yang mendasarinya dan memastikan kesehatan dan kinerja keseluruhan basis data. 
* Fitur skalabilitas berbeda antara vendor - beberapa menawarkan penskalaan otomatis, yang lain memungkinkan pengguna untuk meningkatkan menggunakan API, tetapi tidak skala secara otomatis.  


### MODEL DATA  

Penting juga untuk membedakan antara basis data cloud yang bersifat relasional dan bukan non-relasional atau NoSQL.  
* SQL databases  
adalah salah satu jenis database yang dapat berjalan baik di cloud maupung di *virtual machine* atau *as a service*, tergantung pada vendor. 
* NoSQL databases  
adalah tipe lain dari basis data yang dapat berjalan di cloud. Database NoSQL dibangun untuk melayani read/write yang berat dan dapat meningkatkan dan menurunkan dengan mudah. Beberapa basis data SQL telah mengembangkan kemampuan NoSQL termasuk JSON, JSON biner (mis. BSON atau varian serupa), dan tipe data penyimpanan nilai kunci.