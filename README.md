# Jarkom_Lapres_Modul4_A12

##### Oleh :
- Achmad Sofyan Pratama (05111840000061)
- Oktarizka Asviananda Nursanty (05111840000156)

### Penyelesain Subnetting dan Routing 

![Capture](https://user-images.githubusercontent.com/48914928/102007807-a470ad00-3d5e-11eb-9639-dbd0df43748f.PNG)

Topologi tersebut dilakukan perhitungan pembagian subnet dengan menggunakan metode Classless yaitu:

* VLSM (Variable Length Subnet Masking) di Cisco Packet Tracer
* CIDR (Clasless Inter Domain Routing) di Uml

# Perhitungan VLSM
Melakukan pembagian subnet terhadap topologi yang ada

![InkedSoal Shift Modul 4_LI](https://user-images.githubusercontent.com/48914928/102008369-64132e00-3d62-11eb-80c8-6a0bb5f35a37.jpg)

Dari hasil pembagian subnet, kita mendapatkan sejumlah 13 subnet dan 2 subnet untuk server.

1. Hasil Perhitungang VLSM dperoleh jumlah ip, netmask masing-masing ip dan ip total 

![ip](https://user-images.githubusercontent.com/48914928/102008430-f582a000-3d62-11eb-886e-61873e04bb74.PNG)

Jadi, kita dapat menggunakan netmask /19 untuk memberikan pengalamatan IP pada 13 subnet

2. Subnet besar yang kami bentuk memiliki NID 192.168.0.0 dengan netmask /19. Lalu, kita mulai 
dengan perhitungan pembagian IP dengan bantuan pohon IP

![tree](https://user-images.githubusercontent.com/48914928/102008433-f9162700-3d62-11eb-9d87-3a71303a61de.PNG)

Sehingga, pembagian IP yang memungkinkan untuk topologi yang ada adalah sebagai berikut:

![NID](https://user-images.githubusercontent.com/48914928/102008431-f74c6380-3d62-11eb-8510-508379edf8c1.PNG)


3. Setting IP untuk masing-masing interface yang ada di setiap device sesuai dengan pembagian subnet pada pohon VLSM. Interface dapat diatur pada menu Config > INTERFACE > “nama interface”

* #### SURABAYA (Sebagai Router)

-IP pada Interface SURABAYA yang mengarah ke CLOUD

![cloud](https://user-images.githubusercontent.com/48914928/102008935-9d4d9d00-3d66-11eb-865d-5856e86757bc.PNG)

-IP pada Interface SURABAYA yang mengarah ke MOJOKERTO


![mojokerto](https://user-images.githubusercontent.com/48914928/102008937-9de63380-3d66-11eb-972c-e0fe57a29569.PNG)

-IP pada Interface SURABAYA yang mengarah ke PASURUAN

![pasuruan](https://user-images.githubusercontent.com/48914928/102008938-9e7eca00-3d66-11eb-8993-b00ab799c507.PNG)

-IP pada Interface SURABAYA yang mengarah ke SAMPANG

![sampang](https://user-images.githubusercontent.com/48914928/102008940-9e7eca00-3d66-11eb-859a-e4a6097df56a.PNG)

-IP pada Interface SURABAYA yang mengarah ke BATU

![batu](https://user-images.githubusercontent.com/48914928/102008931-9c1c7000-3d66-11eb-9d45-c5b1fc2f6cb4.PNG)

* #### SAMPANG (Sebagai Klien)

-IP pada Interface SAMPANG yang mengarah ke SURABAYA

![surabaya](https://user-images.githubusercontent.com/48914928/102011395-4b147800-3d76-11eb-8496-89329eb91a33.PNG)

* #### MOJOKERTO (Sebagai Server)

-IP pada Interface MOJOKERTO yang mengarah ke SURABAYA

![surabaya](https://user-images.githubusercontent.com/48914928/102011409-6a130a00-3d76-11eb-9488-5ab47ac3920d.PNG)

* #### PASURUAN (Sebagai Router)

-IP pada Interface PASURUAN yang mengarah ke SURABAYA

![surabaya](https://user-images.githubusercontent.com/48914928/102011418-80b96100-3d76-11eb-9687-dbaeca3652d2.PNG)


-IP pada Interface PASURUAN yang mengarah ke PROBOLINGGO

![Probolinggo](https://user-images.githubusercontent.com/48914928/102011415-7eef9d80-3d76-11eb-8be2-0b15d041025c.PNG)


-IP pada Interface PASURUAN yang mengarah ke SIDOARJO

![sidoarjo](https://user-images.githubusercontent.com/48914928/102011417-8020ca80-3d76-11eb-974f-cbbdcbe2b7bc.PNG)


* #### PROBOLINGGO (Sebagai Router)

-IP pada Interface PROBOLINGGO yang mengarah ke PASURUAN

![pasuruan](https://user-images.githubusercontent.com/48914928/102011443-a8102e00-3d76-11eb-881b-22fa15755f2e.PNG)


-IP pada Interface PROBOLINGGO yang mengarah ke JEMBER dan BANYUWANGI

![jember banyuwngi](https://user-images.githubusercontent.com/48914928/102011442-a7779780-3d76-11eb-845f-7a80fec59221.PNG)

-IP pada Interface PROBOLINGGO yang mengarah ke BONDOWOSO

![bondowoso](https://user-images.githubusercontent.com/48914928/102011440-a6466a80-3d76-11eb-9f87-9172dcfa90ba.PNG)

* #### JEMBER (Sebagai Klien)

-IP pada Interface JEMBER yang mengarah ke PROBOLINGGO

![probolinggo](https://user-images.githubusercontent.com/48914928/102011462-ddb51700-3d76-11eb-8d97-4d8c1a80804d.PNG)


* #### BANYUWANGI (Sebagai Klien)

-IP pada Interface BANYUWANGI yang mengarah ke PROBOLINGGO

![probolinggo](https://user-images.githubusercontent.com/48914928/102011466-ead20600-3d76-11eb-91c9-6e3977141961.PNG)


* #### BONDOWOSO (Sebagai Klien)

-IP pada Interface BONDOWOSO yang mengarah ke PROBOLINGGO

![probolinggo](https://user-images.githubusercontent.com/48914928/102011473-f9202200-3d76-11eb-867d-86523e2e8825.PNG)

* ####BATU (Sebagai Router)

-IP pada Interface BATU yang mengarah ke SURABAYA
![surabaya](https://user-images.githubusercontent.com/48914928/102010202-29fc5900-3d6f-11eb-838c-9be2635ef3ac.PNG)


-IP pada Interface BATU yang mengarah ke KEDIRI
![kediri](https://user-images.githubusercontent.com/48914928/102010199-2963c280-3d6f-11eb-9e6f-980b891416cb.PNG)

-IP pada Interface BATU yang mengarah ke JOMBANG dan MADIUN
![jombang madiun](https://user-images.githubusercontent.com/48914928/102010198-2799ff00-3d6f-11eb-88f8-e349a05318e9.PNG)

-IP pada Interface BATU yang mengarah ke NGANJUK
![ngajnjuk](https://user-images.githubusercontent.com/48914928/102010201-29fc5900-3d6f-11eb-95e9-6564636dffa8.PNG)


* #### JOMBANG (Sebagai Klien)

-IP pada Interface JOMBANG yang mengarah ke BATU dan MADIUN
![BATU dan MADIUN](https://user-images.githubusercontent.com/48914928/102010238-6a5bd700-3d6f-11eb-87e7-422f40c0ba1b.PNG)

* #### MADIUN (Sebagai Router)

-IP pada Interface MADIUN yang mengarah ke BATU dan JOMBANG
![jombang](https://user-images.githubusercontent.com/48914928/102010249-7cd61080-3d6f-11eb-914d-2572d10603e8.PNG)

-IP pada Interface MADIUN yang mengarah ke BOJONEGORO
![bojonegoro](https://user-images.githubusercontent.com/48914928/102010248-7b0c4d00-3d6f-11eb-907c-3198f58052b4.PNG)


* #### BOJONEGORO (Sebagai Klien)

-IP pada Interface BOJONEGORO yang mengarah ke MADIUN
![madiun](https://user-images.githubusercontent.com/48914928/102010257-924b3a80-3d6f-11eb-9910-3fb997d2ba81.PNG)

* #### NGANJUK (Sebagai Klien)

-IP pada Interface NGANJUK yang mengarah ke BATU
![batu](https://user-images.githubusercontent.com/48914928/102010263-a2631a00-3d6f-11eb-89f8-eb95cf9202d8.PNG)



* #### KEDIRI (Sebagai Router)

-IP pada Interface KEDIRI yang mengarah ke BATU
![batu](https://user-images.githubusercontent.com/48914928/102010284-c6bef680-3d6f-11eb-849c-6670301ca789.PNG)

-IP pada Interface KEDIRI yang mengarah ke MALANG
![malang](https://user-images.githubusercontent.com/48914928/102010287-c888ba00-3d6f-11eb-8a09-2c99c1b1c7e3.PNG)

-IP pada Interface KEDIRI yang mengarah ke BLITAR dan LUMAJANG
![BLITAR dan LUMAJANG](https://user-images.githubusercontent.com/48914928/102010286-c7f02380-3d6f-11eb-8c79-ae7e4aa69234.PNG)



* #### MALANG (Sebagai Server)

-IP pada Interface MALANG yang mengarah ke KEDIRI
![kediri](https://user-images.githubusercontent.com/48914928/102010305-dd654d80-3d6f-11eb-8b99-2c3e79a5cdea.PNG)



* #### BLITAR (Sebagai Router)

-IP pada Interface BLITAR yang mengarah ke KEDIRI dan LUMAJANG
![lumajang dan kediri](https://user-images.githubusercontent.com/48914928/102010317-f3730e00-3d6f-11eb-8565-fadb2d262d34.PNG)

-IP pada Interface BLITAR yang mengarah ke TULUNGAGUNG
![TULUNGAGUNG](https://user-images.githubusercontent.com/48914928/102010319-f4a43b00-3d6f-11eb-963d-c3173fe3bc34.PNG)



* #### LUMAJANG (Sebagai Klien)

-IP pada Interface LUMAJANG yang mengarah ke KEDIRI dan BLITAR
![kediri dan blitar](https://user-images.githubusercontent.com/48914928/102010334-084fa180-3d70-11eb-800a-01860e260bd3.PNG)



* #### TULUNGAGUNG (Sebagai Klien)

-IP pada Interface TULUNGAGUNG yang mengarah ke BLITAR
![blitar](https://user-images.githubusercontent.com/48914928/102010356-2917f700-3d70-11eb-86f6-b8a36696c592.PNG)






4.Routing pada setiap router. Routing dapat dilakukan pada menu Config > Routing > Static pada device Router. Lalu isi Static Routes dengan subnet tujuan yang ingin ditambahkan di dalam rute

* Surabaya 
```192.168.0.8/30 via 192.168.0.14
192.168.0.128/25 via 192.168.0.14
192.168.2.0/23 via 192.168.0.6
192.168.0.16/28 via 192.168.0.6
192.168.12.0/22 via 192.168.0.6
192.168.0.0/30 via 192.168.0.6
192.168.1.0/24 via 192.168.0.6
192.168.24.0/22 via 192.168.0.6
192.168.8.0/22 via 192.168.0.14
192.168.16.0/21 via 192.168.0.14
10.151.73.108/30 via 192.168.0.6
```

* Pasuruan 

```192.168.0.128/25 via 192.168.0.10
192.168.16.0/21 via 192.168.0.10
0.0.0.0/0 via 192.168.0.13
```

* Probolinggo

```
0.0.0.0/0 via 192.168.0.9

```

* Batu

```0.0.0.0/0 via 192.168.0.5
192.168.0.16/28 via 192.168.2.2
192.168.1.0/24 via 192.168.0.2
192.168.24.0/22 via 192.168.0.2
10.151.73.108/30 via 192.168.0.2
10.151.73.104/30 via 192.168.0.5
```

* Madiun 

```
0.0.0.0/0 via 192.168.2.1
```

* Kediri

```192.168.24.0/22 via 192.168.1.2
0.0.0.0/0 via 192.168.0.1
```


* Blitar 

```
0.0.0.0/0 via 192.168.1.1

```

# Perhitungan CIDR

Pertama, lakukan pembagian subnet pada topologi dengan cara menyatukan client&router yang berdekatan dan berada pada level yang sama. Berikut hasil dari pembagian subnet :

![Pt1](https://user-images.githubusercontent.com/62512432/102009490-5366b600-3d6a-11eb-92b6-166994b4bce4.png)
![Pt2](https://user-images.githubusercontent.com/62512432/102009383-a5f3a280-3d69-11eb-8336-9a5cb5f99894.png)
![Pt3](https://user-images.githubusercontent.com/62512432/102009409-d1768d00-3d69-11eb-9324-1ca42b2ffef8.png)
![Pt4](https://user-images.githubusercontent.com/62512432/102009424-e94e1100-3d69-11eb-8624-1c16c8c307ce.png)
![Pt5](https://user-images.githubusercontent.com/62512432/102009468-2ca87f80-3d6a-11eb-8381-9f1d16be16ab.png)
![Pt6](https://user-images.githubusercontent.com/62512432/102009481-45189a00-3d6a-11eb-9786-575280be6dae.png)
![Pt7](https://user-images.githubusercontent.com/62512432/102009519-785b2900-3d6a-11eb-85d8-f216aa00f84d.png)

Lalu dari hasil pengelompokan seperti diatas, didapatkan hasil tree sebagai berikut :

![Tree CIDR](https://user-images.githubusercontent.com/62512432/102009536-9a54ab80-3d6a-11eb-9cf5-f5a242497f34.png)

Dari hasil tree tersebut, didapat IP setiap subnet, dan dilakukan perhitungan IP lebih lanjut untuk mendapatkan netmask dan broadcast id seperti berikut :

![Hasil IP](https://user-images.githubusercontent.com/62512432/102009566-dbe55680-3d6a-11eb-9285-f63103c55672.png)

Setelah didapatkan hasil diatas, dapat dilakukan proses routing pada UML.

# Routing CIDR

Pertama, buat topologi pada ```topocidr.sh``` sebagai berikut :
```
# Switch
uml_switch -unix switch0 > /dev/null < /dev/null &
uml_switch -unix switch1 > /dev/null < /dev/null &
uml_switch -unix switch2 > /dev/null < /dev/null &
uml_switch -unix switch3 > /dev/null < /dev/null &
uml_switch -unix switch4 > /dev/null < /dev/null &
uml_switch -unix switch5 > /dev/null < /dev/null &
uml_switch -unix switch6 > /dev/null < /dev/null &
uml_switch -unix switch7 > /dev/null < /dev/null &
uml_switch -unix switch8 > /dev/null < /dev/null &
uml_switch -unix switch9 > /dev/null < /dev/null &
uml_switch -unix switch10 > /dev/null < /dev/null &
uml_switch -unix switch11 > /dev/null < /dev/null &
uml_switch -unix switch12 > /dev/null < /dev/null &
uml_switch -unix switch13 > /dev/null < /dev/null &
uml_switch -unix switch14 > /dev/null < /dev/null &

# Router
xterm -T SURABAYA -e linux ubd0=SURABAYA,jarkom umid=SURABAYA eth0=tuntap,,,10.151.74.41 eth1=daemon,,,switch1 eth2=daemon,,,switch2 eth3=daemon,,,switch7 eth4=daemon,,,switch0 mem=64M &
xterm -T PASURUAN -e linux ubd0=PASURUAN,jarkom umid=PASURUAN eth0=daemon,,,switch2 eth1=daemon,,,switch3 eth2=daemon,,,switch8 mem=64M &
xterm -T PROBOLINGGO -e linux ubd0=PROBOLINGGO,jarkom umid=PROBOLINGGO eth0=daemon,,,switch3 eth1=daemon,,,switch4 eth2=daemon,,,switch9 mem=64M &
xterm -T BATU -e linux ubd0=BATU,jarkom umid=BATU eth0=daemon,,,switch7 eth1=daemon,,,switch11 eth2=daemon,,,switch10 eth3=daemon,,,switch6 mem=64M &
xterm -T MADIUN -e linux ubd0=MADIUN,jarkom umid=MADIUN eth0=daemon,,,switch6 eth1=daemon,,,switch5 mem=64M &
xterm -T KEDIRI -e linux ubd0=KEDIRI,jarkom umid=KEDIRI eth0=daemon,,,switch11 eth1=daemon,,,switch14 eth2=daemon,,,switch12 mem=64M &
xterm -T BLITAR -e linux ubd0=BLITAR,jarkom umid=BLITAR eth0=daemon,,,switch14 eth1=daemon,,,switch13 mem=64M &

# Server
xterm -T MOJOKERTO -e linux ubd0=MOJOKERTO,jarkom umid=MOJOKERTO eth0=daemon,,,switch0 mem=64M &
xterm -T MALANG -e linux ubd0=MALANG,jarkom umid=MALANG eth0=daemon,,,switch12 mem=64M &

# Klien
xterm -T SAMPANG -e linux ubd0=SAMPANG,jarkom umid=SAMPANG eth0=daemon,,,switch1 mem=64M &
xterm -T BONDOWOSO -e linux ubd0=BONDOWOSO,jarkom umid=BONDOWOSO eth0=daemon,,,switch4 mem=64M &
xterm -T JEMBER -e linux ubd0=JEMBER,jarkom umid=JEMBER eth0=daemon,,,switch9 mem=64M &
xterm -T BANYUWANGI -e linux ubd0=BANYUWANGI,jarkom umid=BANYUWANGI eth0=daemon,,,switch9 mem=64M &
xterm -T SIDOARJO -e linux ubd0=SIDOARJO,jarkom umid=SIDOARJO eth0=daemon,,,switch8 mem=64M &
xterm -T JOMBANG -e linux ubd0=JOMBANG,jarkom umid=JOMBANG eth0=daemon,,,switch6 mem=64M &
xterm -T BOJONEGORO -e linux ubd0=BOJONEGORO,jarkom umid=BOJONEGORO eth0=daemon,,,switch5 mem=64M &
xterm -T NGANJUK -e linux ubd0=NGANJUK,jarkom umid=NGANJUK eth0=daemon,,,switch10 mem=64M &
xterm -T LUMAJANG -e linux ubd0=LUMAJANG,jarkom umid=LUMAJANG eth0=daemon,,,switch14 mem=64M &
xterm -T TULUNGAGUNG -e linux ubd0=TULUNGAGUNG,jarkom umid=TULUNGAGUNG eth0=daemon,,,switch13 mem=64M &
```
Kemudian di bash, dan lakukan login pada setiap UML dengan ```username : root``` dan ```password : praktikum```. Lalu pada setiap router, uncomment bagian ```net.ipv4.ip_forward=1``` di ```/etc/sysctl.conf``` agar dapat melakukan proses routing. Selanjutnya, ```/etc/network/interfaces``` diedit menjadi seperti dibawah ini :

## ROUTER ##

**SURABAYA**
![sby](https://user-images.githubusercontent.com/62512432/102010310-e5bd8880-3d6f-11eb-8a92-50f06db7096f.png)

**PASURUAN**
![pasuruan](https://user-images.githubusercontent.com/62512432/102010343-1a314480-3d70-11eb-9163-eb203a8b201d.png)

**PROBOLINGGO**
![probo](https://user-images.githubusercontent.com/62512432/102010378-464cc580-3d70-11eb-9190-92e181d6dac3.png)

**BATU**
![batu](https://user-images.githubusercontent.com/62512432/102010436-97f55000-3d70-11eb-85a3-f0d3687c78bc.png)

**MADIUN**
![madiun](https://user-images.githubusercontent.com/62512432/102010462-c3783a80-3d70-11eb-91d9-32e737512ce3.png)

**KEDIRI**
![kediri](https://user-images.githubusercontent.com/62512432/102010491-ef93bb80-3d70-11eb-8f85-0b97144354d2.png)

**BLITAR**
![blitar](https://user-images.githubusercontent.com/62512432/102010516-1b16a600-3d71-11eb-87ad-5ca9253ab961.png)

## SERVER ##

**MOJOKERTO**

**MALANG**

## KLIEN ##

**SAMPANG**

**SIDOARJO**

**BANYUWANGI**

**JEMBER**

**BONDOWOSO**

**JOMBANG**

**BOJONEGORO**

**NGANJUK**

**TULUNGAGUNG**

**LUMAJANG**

Kemudian setelah selesai, lakukan ```service networking restart``` dan pada router, lakukan ```iptables –t nat –A POSTROUTING –o eth0 –j MASQUERADE –s 192.168.0.0/16```.


