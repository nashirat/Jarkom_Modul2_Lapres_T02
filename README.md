
# Lapres Modul 2 Jarkom T02 2020

#### Oleh :
- Muhammad Sulthon Nashir (0511174000017)
- Bagas Immanuel Lodianto (05311840000026)


## No 1
### Membuat Website dengan alamat semeruyyy.pw

Membuat file dengan nama alamat di /etc/bind

![Nomor 1](img/1.PNG)

Membuat file di /etc/bind/named.conf.local

![Nomor 1](img/1B.PNG)

## No 2
### Membuat alias dengan www.semeruyyy.pw (CNAME Record)
mengedit file yang ada di /etc/bind
![Nomor 2](img/2.PNG)

## No 3
### Membuat Sub Domain penanjakan dan diarahkan ke Probolinggo 
mengedit file yang ada di /etc/bind
![Nomor 3](img/3.PNG)

## No 4
### Reverse Domain untuk Domain utama 
mengedit file yang ada di /etc/bind/named.local.conf
![Nomor 4](img/4.PNG)

## No 5
### Membuat Mojokerto menjadi DNS Slave dari Malang

Setting pada Malang Allow transfer

![Nomor 5](img/5.PNG)

Setting pada Mojokerto Sebagai slave 

![Nomor 5](img/5B.PNG)

## No 6
### Membuat Delegasi subdomain

Setting pada Malang untuk delegasi (NS1)
![Nomor 6](img/6.PNG)

Setting pada Malang untuk delegasi (Allow query any)
![Nomor 6](img/6B.PNG)

Allow Transfer
![Nomor 6](img/6C.PNG)

Setting di Mojokerto allow transfer any
![Nomor 6](img/6D.PNG)

Setting allow Query any
![Nomor 6](img/6E.PNG)

## No 7 
### Membuat Subdomain naik.gunung.semeruyyy.pw

Membuat file di /etc/bind
![Nomor 7](img/7.PNG)


## No 8

### Mengatur Web Server untuk semeruyyy.pw

Membuat file di /etc/apache2/sites-available
![Nomor 8](img/8.PNG)

Membuat Document root di /var/www/
![Nomor 8](img/8B.PNG)

Maka hasilnya
![Nomor 8](img/8C.PNG)


## No 9
### Aktifkan Mod Rewrite sehingga index.php hilang

Membuat file .htaccess pada root folder dari semeruyyy.pw
![Nomor 9](img/9.PNG)

Maka Hasilnya
![Nomor 9](img/9B.PNG)

## No 10
### Membuat Web lagi dengan nama penanjakan.semeruyyy.pw

Membuat Document root di /var/www
![Nomor 10](img/10.PNG)

Membuat file /etc/apache2/sites-available
![Nomor 10](img/10B.PNG)

## No 11
### Public boleh di akses, folder isinya public tidak boleh

Mengbubah file yang ada di /etc/apache2/sites-available agar mematikan option indexes

![Nomor 11](img/11.PNG)

## No 12
### Redirect url yang tidak valid ke 404.html

Membuat file .htaccess yang melakukan redirect
![Nomor 12](img/12.PNG)

## No 13
### Membuat Alias javascript jadi /js 

![Nomor 13](img/13.PNG)

## No 14
### Membuat web naik.gunung.semerut02.pw dengan port 8888

Tinggal buat di sites-available naik.gunung.semeru02.pw dengan port 8888. Lalu tambahkan lister 8888 di ports.conf.
![Nomor 14](img/14.PNG)

## No 15
### Set username dan password di naik.gunung.semerut02.pw

Pertama buat username dan password di file .htpasswd dengan htpasswd. Bisa dilihat kalau password terenkripsi.
![Nomor 15](img/15c.PNG)
Lalu cek ulang di naik.gunung.semerut02.pw
![Nomor 15](img/15.PNG)
![Nomor 15](img/15b.PNG)


## No 16
### Redirect IP Probolinggo ke semeruyyy.pw

Mengedit file yang ada di /etc/apache2/sites-available/default
![Nomor 16](img/16.PNG)


## No 17
### Jika URL mengandung Substring semeru redirect ke semeru.jpg

Membuat File .htaccess yang mengandung regex dan melakuakn redirect yang diletakkan di root
![Nomor 17](img/17.PNG)
