# UJIAN TENGAH SEMESTER Teknologi Cloud Computing
-------------------------------------------------------------------------------------
##### 1. Membuat Akun Dockerhub
Membuat akun Dockerhub dapat dilakukan dengan cara [Docker Hub](https://hub.docker.com/), apabila sudah mempunyai akun DockerHub maka dapat  [Login](https://id.docker.com/login/?next=%2Fid%2Foauth%2Fauthorize%2F%3Fclient_id%3D43f17c5f-9ba4-4f13-853d-9d0074e349a7%26next%3D%252F%253Fref%253Dlogin%26nonce%3DeyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiI0M2YxN2M1Zi05YmE0LTRmMTMtODUzZC05ZDAwNzRlMzQ5YTciLCJleHAiOjE1ODU1MTQ1NzUsImlhdCI6MTU4NTUxNDI3NSwicmZwIjoidVd2UDNXQ04taEJCYzBfYy1wRUVYZz09IiwidGFyZ2V0X2xpbmtfdXJpIjoiLz9yZWY9bG9naW4ifQ.7xqSCH9ncCNtvK2U-1wlRBvCxeLmViw9rpQ6w6mglLo%26redirect_uri%3Dhttps%253A%252F%252Fhub.docker.com%252Fsso%252Fcallback%26response_type%3Dcode%26scope%3Dopenid%26state%3DeyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiI0M2YxN2M1Zi05YmE0LTRmMTMtODUzZC05ZDAwNzRlMzQ5YTciLCJleHAiOjE1ODU1MTQ1NzUsImlhdCI6MTU4NTUxNDI3NSwicmZwIjoidVd2UDNXQ04taEJCYzBfYy1wRUVYZz09IiwidGFyZ2V0X2xpbmtfdXJpIjoiLz9yZWY9bG9naW4ifQ.7xqSCH9ncCNtvK2U-1wlRBvCxeLmViw9rpQ6w6mglLo) secara langsung, gambar dibawah adalah akun yang sudah mendaftarkan didalam dockerHub
![Gambar Akun Dockerhub](https://github.com/yusufandy/UTS-teknologi-cloud-computing/blob/master/tcc/soal%201.png)

##### 2. Menjalankan pull image
* Pertama mengclone image dari doodle, doodle yang digunakan adalah `chrees2019` dengan melakukan perpindahan direktori pada CMD dengan perintah `cd doodle/chrees2019`. 

* Kedua menginstall build cheers2019 `docker build -t yusufandy/cheers2019`dan menentukan bahwa semua file dalam direktori lokal  mendapatkan tard dan dikirim ke daemon Docker. PATH menentukan dimana untuk menemukan file untuk “konteks” dari membangun di daemon Docker, dibutuhkan beberapa menit untuk mendapatkan file secara sukses.
![Proses build image](https://github.com/yusufandy/UTS-teknologi-cloud-computing/blob/master/tcc/soal%202-1.png)

* Ketiga menjalankan container dengan image yang sudah di download dengan mengetikkan perintah `docker run -t yusufandy/cheers2019`, untuk melihat image yang telah dibuat.
![Hasil](https://github.com/yusufandy/UTS-teknologi-cloud-computing/blob/master/tcc/soal%202-2.png) 
![Hasil](https://github.com/yusufandy/UTS-teknologi-cloud-computing/blob/master/tcc/soal%202-3.png)

* Keempat melakukan cek cek container pada docker dengan perintah`docker -ps a`, akan menampilkan rincian docker. 
![Cek Image](https://github.com/yusufandy/UTS-teknologi-cloud-computing/blob/master/tcc/soal%202-4.png)

* Kelima menghentikan container dengan menggunakan perintah `docker stop 3d027c5b5e40`, maka secara otomatis docker akan berhenti.
![Stop Image](https://github.com/yusufandy/UTS-teknologi-cloud-computing/blob/master/tcc/soal%202-5.png)

* Keenam mengecek kembali apakah container sudah diberhentikan dengan perintah `docker -ps a`, apabila muncul exited maka container berhasil berhenti.
![Cek Image Ulang]https://github.com/yusufandy/UTS-teknologi-cloud-computing/blob/master/tcc/soal%202-6.png)
##### 3. Dockerfile dan Push ke Repository DockerHub
* Membuat image  file Dockerfile dapat menggunakan cara seperti berikut :
![Hasil](https://github.com/yusufandy/UTS-Teori-TEKN-CLOUD/blob/master/tcc/soal%204-2.png)