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
![surabaya](https://user-images.githubusercontent.com/48914928/102009355-83fa2000-3d69-11eb-965d-057c23e836c6.PNG)

* #### MOJOKERTO (Sebagai Server)

-IP pada Interface MOJOKERTO yang mengarah ke SURABAYA


* #### PASURUAN (Sebagai Router)

-IP pada Interface PASURUAN yang mengarah ke SURABAYA
![surabaya](https://user-images.githubusercontent.com/48914928/102009384-a5f3a280-3d69-11eb-8508-ea40681619eb.PNG)

-IP pada Interface PASURUAN yang mengarah ke PROBOLINGGO
![Probolinggo](https://user-images.githubusercontent.com/48914928/102009379-a429df00-3d69-11eb-82bb-f9dbfa658ef2.PNG)

-IP pada Interface PASURUAN yang mengarah ke SIDOARJO
![sidoarjo](https://user-images.githubusercontent.com/48914928/102009381-a5f3a280-3d69-11eb-9f88-2b3d19f7350f.PNG)

* #### PROBOLINGGO (Sebagai Router)

-IP pada Interface PROBOLINGGO yang mengarah ke PASURUAN
![pasuruan](https://user-images.githubusercontent.com/48914928/102009500-5792d380-3d6a-11eb-88a1-1c52cb53851c.PNG)



-IP pada Interface PROBOLINGGO yang mengarah ke JEMBER dan BANYUWANGI
![jember banyuwngi](https://user-images.githubusercontent.com/48914928/102009499-5792d380-3d6a-11eb-9a3f-0b244fa31885.PNG)

-IP pada Interface PROBOLINGGO yang mengarah ke BONDOWOSO
![bondowoso](https://user-images.githubusercontent.com/48914928/102009496-5661a680-3d6a-11eb-922c-b4ea5433ae97.PNG)


* #### JEMBER (Sebagai Klien)

-IP pada Interface JEMBER yang mengarah ke PROBOLINGGO

![probolinggo](https://user-images.githubusercontent.com/48914928/102009533-96288e00-3d6a-11eb-8c70-d81c308158fe.PNG)

* #### BANYUWANGI (Sebagai Klien)

-IP pada Interface BANYUWANGI yang mengarah ke PROBOLINGGO
![probolinggo](https://user-images.githubusercontent.com/48914928/102009542-a476aa00-3d6a-11eb-86b7-be71d6aea87b.PNG)

* #### BONDOWOSO (Sebagai Klien)

-IP pada Interface BONDOWOSO yang mengarah ke PROBOLINGGO

![probolinggo](https://user-images.githubusercontent.com/48914928/102009547-b1939900-3d6a-11eb-8dc6-eecb70d952e8.PNG)



# Perhitungan CIDR

Pertama, lakukan pembagian subnet pada topologi dengan cara menyatukan client&router yang berdekatan dan berada pada level yang sama. Berikut hasil dari pembagian subnet :

<p align ="center"><img width="500" src="https://user-images.githubusercontent.com/62512432/102009364-8eb4b500-3d69-11eb-92b7-8f0cfdb5b57d.png"></p>
<p align ="center"><img width="500" src="https://user-images.githubusercontent.com/62512432/102009383-a5f3a280-3d69-11eb-8336-9a5cb5f99894.png"></p>
<p align ="center"><img width="500" src="https://user-images.githubusercontent.com/62512432/102009409-d1768d00-3d69-11eb-9324-1ca42b2ffef8.png"></p>
<p align ="center"><img width="500" src="https://user-images.githubusercontent.com/62512432/102009424-e94e1100-3d69-11eb-8624-1c16c8c307ce.png"></p>
<p align ="center"><img width="500" src="https://user-images.githubusercontent.com/62512432/102009364-8eb4b500-3d69-11eb-92b7-8f0cfdb5b57d.png"></p>
<p align ="center"><img width="500" src="https://user-images.githubusercontent.com/62512432/102009364-8eb4b500-3d69-11eb-92b7-8f0cfdb5b57d.png"></p>
<p align ="center"><img width="500" src="https://user-images.githubusercontent.com/62512432/102009364-8eb4b500-3d69-11eb-92b7-8f0cfdb5b57d.png"></p
