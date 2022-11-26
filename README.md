# Jarkom-Modul-4-ITB08-2022

## Anggota:
| Nama                      | NRP        |
|---------------------------|------------|
| Salsabila Briliana A. S.  | 5027201003 |
| Muhammad Rifqi Fernanda   | 5027201050 |
| Gilang Bayu Gumantara     | 5027201062 | 


## Topologi CPT
---
![topologiCPT](image/topologiCPT.png)

## VLSM
---
Pertama, kami membagi topologi kedalam beberapa bagian kecil.
![topologiVLSM](image/topologiVLSM.png)

Selanjutnya menghitung berapa jumlah host pada setiap subnet dan netmask yang akan digunakan.
![tabel](image/tabel.png)


Major network nya berada pada netmask /20. Prefix IP kelompok kami adalah 192.218.X.X. Selanjutnya kami membuat pohon perhitungan VLSM
![pohonVLSM](image/pohonVLSM.png)

Untuk table perhitungannya adalah sebagai berikut :
![tabelVLSM](image/tabelVLSM.png)

Selanjutnya yaitu, memasukkan ip pada setiap node cohtoh pada subnet A1

```
Subnet A1 : 
    NID : 192.218.8.0
    Netmask : 255.255.252.0
    IP range : 192.218.8.1 - 192.218.11.254
```

Selanjutnya yaitu mengatur router, contohnya pada The Minister terhubung dengan Guideau pada interface `Fa0/0`. maka ip pada `interface Fa0/0` diatur dengan IP range yang tersedia sebagai berikut:
![contoh1](image/contoh1.png)

Setelah mengatur IP pada The Minister, selanjutnya kita mengatur IP pada Guideau dengan IP range yang telah tersedia sebagai berikut:
![contoh2](image/contoh2.png)

Setelah berhasil mengatur IP pada subnet A1, selanjutnya mengatur IP setiap subnet sampai A18 sesuai dengan hasil perhitungan yang telah didapatkan sebelumnya. Karena terlalu banyak, kami hanya mencontohkan assign IP pada satu subnet saja. Untuk assign lengkap nya dapat di akses melalui <a href="https://github.com/SalsabilaB/Jarkom-Modul-4-ITB08-2022/blob/main/modul4.pkt"><b style="color:red">link berikut ini</b></a> 

Setelah semua Node sudah diatur IP nya, selanjutnya yaitu melakukan routing agar semua node saling terhubung. Cara melakukan konfigurasinya adalah dengan masuk pada config ROUTING. Disana dapat mengisikan Netrwork , Mask, dan Next Hop yang ditujukan. Sebagai contoh penjelasan, kita ambil Router The Order. The order terhubung dengan router The Minister, sehingga konfigurasi pada router The Order yaitu:

![static](image/static.png)

Selanjutnya yaitu memastikan semua node telah terhubung.
![hasilVLSM](image/hasil.png)

## Topologi GNS3
---
![image](https://user-images.githubusercontent.com/90242686/204094486-506c673f-b6ad-41eb-8db9-b9753b9c49ab.png)

## CIDR
---
- Selanjutnya menghitung berapa jumlah host pada setiap subnet dan netmask yang akan digunakan.
![image](https://user-images.githubusercontent.com/90242686/204094765-29dd89cf-4e0a-4484-9b1e-e52525427ea9.png)

- Pembagian subnetting

![image](https://user-images.githubusercontent.com/90242686/204097960-62a1e4fe-9ed1-4506-a543-d016b8e71a17.png)


-  Selanjutnya kami membuat pohon perhitungan CIDR
![image](https://user-images.githubusercontent.com/90242686/204095393-fa4c7793-1e24-4e43-928e-c7c61e43f222.png)





