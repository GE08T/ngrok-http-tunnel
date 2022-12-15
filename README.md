## Pengertian Ngrok :

- Ngrok adalah penyedia layanan untuk Http Tunneling.
- Http Tunneling teknik untuk meneruskan request HTTP yang kita lakukan ke target yang dituju / ke Web Server.
- Simplenya, Ngrok dapat melakukan request via internet ke web server yang berjalan dalam local pc. Jadi tanpa perlu menggunakan cloud, hosting, private server, kita bisa mendapatkan request tersebut.
- Dengan demikian kita bisa mengakses web server yang ada di local via internet dengan menggunakan layanan Ngrok.

## Alur Ngrok :

- Start: Browser-> Menuju: Ngrok Server -> Meminta: computer yang menjalankan website dan Ngrok / daemon.
- Jadi ketika Ngrok / daemon dijalankan maka akan terkoneksi ke server Ngrok, dengan demikian di server itu membuatkan istilah kata Public Domain sehingga dapat diakses melalui Browser.
- Kemudian request didapatkan dari web di local lewat Ngrok diteruskan ke Ngrok server dan diteruskan lagi ke Browser.

## Download : 

- Download di situs ngrok.
- Kemudian ekstrak.

## Authentication :

- Sign up di situs ngrok
- Copy authenticate key nya
- Buka file exe di dalam file yang di ekstrak tadi
- Tambakan authenticate key kedalam nya / command nya

## Mendaftarkan Server Local :
- Buka file : ``` C:\Users\nama_user\AppData\Local/ngrok/ngrok.yml ```
- Untuk mendaftarkan local tambahkan di ngrok.yml :

```
tunnels:
  nama tunnels / test :
    proto: http / https dsb
    addr: 127.0.0.1:8000 / 8080 dsb
```

## Running : 

- Buka file exe tadi lalu tambahkan perintah :

```
$ ngrok start nama tunnels / test
```

## Inspecting Traffic : 

- Ketika menjalankan HTTP Tunnel, kadang kita melakukan proses debugging 
- Seperti untuk melihat request yang masuk / response yang keluar  yang berjalan di laptop kita 
- Untuk menggunakan fitur ini buka : http://localhost:4040

## Source Belajar : 

Link Youtube : https://www.youtube.com/watch?v=g9Ore5ZTw1M
