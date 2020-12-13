# Jarkom_Lapres_Modul4_A12

##### Oleh :
* Achmad Sofyan Pratama 
* OKtarizka Asviananda Nursanty

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

*IP pada Interface SURABAYA yang mengarah ke CLOUD

![cloud](https://user-images.githubusercontent.com/48914928/102008935-9d4d9d00-3d66-11eb-865d-5856e86757bc.PNG)

*IP pada Interface SURABAYA yang mengarah ke MOJOKERTO


![mojokerto](https://user-images.githubusercontent.com/48914928/102008937-9de63380-3d66-11eb-972c-e0fe57a29569.PNG)

*IP pada Interface SURABAYA yang mengarah ke PASURUAN

![pasuruan](https://user-images.githubusercontent.com/48914928/102008938-9e7eca00-3d66-11eb-8993-b00ab799c507.PNG)

*IP pada Interface SURABAYA yang mengarah ke SAMPANG

![sampang](https://user-images.githubusercontent.com/48914928/102008940-9e7eca00-3d66-11eb-859a-e4a6097df56a.PNG)

*IP pada Interface SURABAYA yang mengarah ke BATU

![batu](https://user-images.githubusercontent.com/48914928/102008931-9c1c7000-3d66-11eb-9d45-c5b1fc2f6cb4.PNG)

