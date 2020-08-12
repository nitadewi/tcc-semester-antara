## Pertemuan 10 Clustering menggunakan Kubernetes  


Kubernetes adalah mesin orkestrasi container open source untuk mengotomatiskan penerapan, scaling (penskalaan), dan pengelolaan aplikasi dalam container. Proyek open source diselenggarakan oleh Cloud Native Computing Foundation (CNCF).

Layanan Kubernetes dan Layanan Swarm sangat berbeda! Meski memiliki nama yang mirip, kedua orkestra ini memiliki arti yang sangat berbeda dengan istilah 'layanan'. Di Swarm, layanan menyediakan fasilitas penjadwalan dan jaringan, membuat wadah dan menyediakan alat untuk merutekan lalu lintas ke sana. Di Kubernetes, penjadwalan dan jaringan ditangani secara terpisah: penerapan (atau pengontrol lain) menangani penjadwalan container sebagai pod, sementara layanan hanya bertanggung jawab untuk menambahkan fitur jaringan ke pod tersebut. 

Cluster Kubernetes adalah sekumpulan mesin node untuk menjalankan aplikasi dalam container. Jika Anda menjalankan Kubernetes, Anda menjalankan cluster.

Minimal, cluster berisi Control plane dan satu atau beberapa mesin komputasi, atau node. Control plane bertanggung jawab untuk mempertahankan status cluster yang diinginkan, seperti aplikasi mana yang sedang berjalan dan gambar container mana yang mereka gunakan. Node benar-benar menjalankan aplikasi dan beban kerja.

Kluster adalah keunggulan utama Kubernetes: kemampuan untuk menjadwalkan dan menjalankan container di sekumpulan mesin, baik itu fisik maupun virtual, di tempat atau di cloud. Kontainer Kubernetes tidak terikat dengan mesin individu. Sebaliknya, mereka disarikan di seluruh cluster. 

Mari kita lihat beberapa istilah Kubernetes lainnya yang berguna untuk memahami apa yang dilakukan cluster.

* Control plane: Kumpulan proses yang mengontrol node Kubernetes. Di sinilah semua tugas berasal.

* Node: Mesin ini melakukan tugas yang diminta yang diberikan oleh bidang kontrol.

* Pod: Kumpulan 1 atau lebih container yang di-deploy ke satu node. Pod adalah objek Kubernetes terkecil dan paling sederhana.

* Service: Cara untuk mengekspos aplikasi yang berjalan pada sekumpulan pod sebagai layanan jaringan. Ini memisahkan definisi kerja dari pod.

* Volume: Direktori yang berisi data, dapat diakses oleh container di dalam pod. Volume Kubernetes memiliki masa hidup yang sama dengan pod yang membungkusnya. Volume hidup lebih lama dari semua penampung yang berjalan di dalam pod, dan data dipertahankan saat penampung dimulai ulang.

* Namespace: Kluster virtual. Namespaces memungkinkan Kubernetes untuk mengelola beberapa cluster (untuk beberapa tim atau project) dalam cluster fisik yang sama.