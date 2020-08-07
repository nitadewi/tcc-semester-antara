## Pertemuan 8 Docker, Docker Compose, dan Docker Network  

### Docker
untuk penjelasan docker ada di rangkuman [minggu-ke 7](https://github.com/nitadewi/tcc-semester-antara/blob/master/minggu-06.md)  

### Docker Compose  
Compose merupakan alat untuk mendefinisikan dan menjalankan aplikasi multi-container Docker. Dengan Compose, file YAML digunakan untuk mengonfigurasi layanan aplikasi. Kemudian, dengan satu perintah dapat membuat dan memulai semua layanan dari konfigurasi YAML.

Menggunakan Compose pada dasarnya memiliki 3 langkah proses: 
1. menetapkan lingkungan aplikasi dengan Dockerfile sehingga dapat direproduksi di mana saja
2. menentukan layanan yang membentuk aplikasi di docker-compose.yml sehingga aplikasi tersebut dapat dijalankan bersama di lingkungan yang terisolasi.
3. Jalankan *docker-compose up* dan Compose dimulai dan jalankan seluruh aplikasi.  

contoh kode dengan YAML

```
version: '2.0'
services:
  web:
    build: .
    ports:
    - "5000:5000"
    volumes:
    - .:/code
    - logvolume01:/var/log
    links:
    - redis
  redis:
    image: redis
volumes:
  logvolume01: {}
```


### Docker Network  
perintah Docker network digunakan untuk mengelola jaringan. dapat menggunakan sub perintah untuk membuat(create), memeriksa(inspect), mendaftar(list), menghapus(remove), memangkas(prune), menghubungkan(connect), dan memutuskan jaringan(disconnect networks).  

```
docker network COMMAND
```

Docker Network memiliki beberapa child commands antara lain:
| Command     | Keteranangan |
| ----------- | ----------- |
| docker network connect     | menghubungkan kontainer ke network     |
| docker network create   | membuat network       |
|docker network disconnect|memutuskan kontainer dari network|
|docker network inspect| menampilkan detail informasi dari satu atau banyak network |
|docker network ls| daftar network |
|docker network prune| menghapus semua network yang tidak digunakan |
|docker network rm| menghapus satu atau banyak network|  


