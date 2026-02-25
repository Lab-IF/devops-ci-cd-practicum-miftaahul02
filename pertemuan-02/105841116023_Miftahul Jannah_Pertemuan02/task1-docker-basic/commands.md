# Daftar commands yang dijalankan

**1. Pull Image Nginx**
docker pull nginx:alpine

Mengunduh image nginx versi alpine dari Docker Hub ke sistem lokal.

**2. Menjalankan Container**
docker run -d --name web-praktikum -p 8080:80 nginx:alpine

Keterangan:

-d → Menjalankan container di background

--name web-praktikum → Memberikan nama container

-p 8080:80 → Mapping port 8080 (host) ke 80 (container)

**3. Melihat Container yang Berjalan**
docker ps

Menampilkan daftar container yang sedang aktif.

**4. Mengakses Nginx Melalui Browser**
https://localhost:8080

Jika berhasil, akan tampil halaman default nginx.

**5. Melihat Logs Container**
docker logs web-praktikum

Menampilkan log aktivitas container nginx.

**6. Masuk ke Dalam Container**
docker exec -it web-praktikum sh

Perintah yang dijalankan di dalam container:

**7. Menghentikan Container**
docker stop web-praktikum

Menghentikan container yang sedang berjalan.

**8. Menghapus Container**
docker rm web-praktikum

Menghapus container dari sistem.
