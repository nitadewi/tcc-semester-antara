## Pertemuan 9 Clustering menggunakan Docker Swarm  

Docker swarm adalah *container orchestration tool* atau alat orkestrasi kontainer, yang berarti memungkinkan pengguna untuk mengelola banyak kontainer yang ditempatkan di beberapa mesin host. 

orkestrator (orchestrators) adalah alat untuk mengelola, menskalakan, dan memelihara aplikasi dalam container dan contoh paling umum adalah Kubernetes dan Docker Swarm.  

Swarm menyediakan banyak alat untuk penskalaan, jaringan, mengamankan dan memelihara aplikasi dalam container, di atas dan di luar kemampuan container itu sendiri.

Untuk memvalidasi bahwa aplikasi dalam container berfungsi dengan baik di Swarm, menggunakan lingkungan Swarm bawaan Docker Desktop tepat di mesin pengembangan untuk menerapkan aplikasi, sebelum dijalankan di cluster Swarm penuh dalam produksi. Lingkungan Swarm yang dibuat oleh Docker Desktop berfitur lengkap, yang berarti ia memiliki semua fitur Swarm yang akan dinikmati aplikasi di *real cluster* atau kluster nyata.

Swarm tidak pernah membuat wadah individual. Sebagai gantinya, semua beban kerja Swarm dijadwalkan sebagai layanan, yang merupakan grup kontainer yang dapat diskalakan dengan fitur jaringan tambahan yang dikelola secara otomatis oleh Swarm. Selanjutnya, semua objek Swarm dapat dan harus dijelaskan dalam manifes yang disebut file tumpukan(stack).   

[sumber](https://docs.docker.com/get-started/swarm-deploy/)  
