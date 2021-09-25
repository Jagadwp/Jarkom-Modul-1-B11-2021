# Jarkom-Modul-1-B11-2021

## **Kelompok B-11**
- Muhammad Nevin        (05111940000079)
- Albert Filip Silalahi (05111940000116)
- Jagad Wijaya Purnomo	(05111940000132)

## **Pembagian Tugas**
- Muhammad Nevin: Mengerjakan no. 1,2,4,10,11
- Albert Filip Silalahi: Mengerjakan no. 3,5,6,8,12
- Jagad Wijaya Purnomo:	Mengerjakan no. 7,9,13,14,15

## **Nomor 1**
Sebutkan webserver yang digunakan pada <a href='ichimarumaru.tech'>"ichimarumaru.tech"</a>!

### Solusi
- Filter menggunakan filter command http contains “ichimarumaru.tech”
- Kemudian klik kanan, pilih Follow > TCP Stream, dan dapat terlihat bahwa webserver yang digunakan adalah nginx/1.18.0 (Ubuntu), dengan destination port 80 (HTTP).
 <p align="center"><img width="60%" src="https://lh5.googleusercontent.com/P4NIhZrlizDzUCJHjFDh8xliId6nai38MXjEWKKH_LKdDO3nVncDZ-Ayl4RQU90wlIntianNIk6HYX3fP-w08OjpuXI4esO2GqgEaIXjqLtsxv8bAq3-D4D4W1DkN1M9EzN6BdGu=s0"></p>
 
## **Nomor 2**
Temukan paket dari **web-web** yang menggunakan **basic authentication** method!

### Solusi
- Gunakan command ``` http.authbasic ```
<p align="center"><img width="60%" src="https://lh5.googleusercontent.com/iD6Z6TNxPz6WacG-2tc-yZ91h1JWFC91uSbAIBKHjSFbxSrQ_C5u4KwLjFc3sr9VNIHiAHmeiTsAjxGUqDlq-leA7o-Ev7Mg4VXWWGhpekguuxZmxWmCg8Au9DryRXYK0eWV9QhS=s0"></p>

## **Nomor 3**
Ikuti perintah di <a href='basic.ichimarumaru.tech'>basic.ichimarumaru.tech</a>! Username dan password bisa didapatkan dari file .pcapng!

### Solusi
- Melakukan display filter ``` http.host ==  basic.ichimarumaru.tech ``` . Pilih yang memiliki method **GET**, lalu akan didapatkan username dan passwordnya
<p align="center"><img width="70%" src="https://lh4.googleusercontent.com/RzC9i9AIsYsTGLx3yteZ6KyEMnKaNFN-nukZeu-H2WBs35FyyQbIHOtxn7bwRNAq7_mgfaOp-w9VoVqgAlqNNlJdIlqVEJu8ZE0nTgVbXYLoPpZO1mr8ywq_jF_bNDLYtJZXck6X=s0"></p>

- Login dengan username: **kuncimenujulautan** dan password: **“tQKEJFbgNGC1NCZlWAOjhyCOm6o3xEbPkJhTciZN”** sesuai credentials.
<p align="center"><img width="70%" src="https://lh4.googleusercontent.com/qFtDiWqjbVsDbRU5DWHEE-AQRncanDXV-E38BHd5rIh2AU7Ufm2qDrgs3-rYLvEmHDLEuQOvvmvDjn1Jb3EKa-m8t8vsMcGbLjeN2uFUos9IanprO-3XqU8-KssqI-zMZukbUGFH=s0"></p>

- Masukkan jawaban dari soal yang diberikan


## **Nomor 4**
Temukan paket **mysql** yang mengandung **perintah query select**!

### Solusi
- Melakukan display filter ``` mysql.command == 3 and frame matches "SELECT" ``` . 
<p align="center"><img width="70%" src="https://lh3.googleusercontent.com/qgwS4qjIpcCr67K60O8Orxkk-rqXrpjh4_iBTB7pDaGIA77uXB9z_6gSK3Q-s0OykHMO6SGPSth22bUuhD2xfxp1DDstdPo7z_Rx8Sx5VbsFzC6EhvXH5pngzcS5lUdcP6Va--Ys=s0"></p>


## **Nomor 5**
Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan password bisa didapat dari **query insert** pada table **users** dari file .pcap!

### Solusi
- Melakukan display filter ``` mysql.command == 3 and frame matches "INSERT" ```
<p align="center"><img width="70%" src="https://lh5.googleusercontent.com/4dDbD6pJp5SV-hCF6yNBfcIH0NTn1P7XayhPAjI7vlGACkwc8HKNwnITRh9UhcjyE0Xt4-r6c9x1rED5ASWzIeRkt2kIh0bSM-lFJYl1iTknAI93bI5DbVQGe92kpAZ7lc1lGXmJ=s0"></p>

- Login dengan username: **akakanomi** dan password: **pemisah4lautan**
- Tulis jawaban soal yang diberikan
<p align="center"><img width="70%" src="https://lh4.googleusercontent.com/o08qcsO1-EWgSUVluU1PhQYnNZsu29ziON0pHACI8uOw25zrLT6SQCMBAX4OBn9CPvF_bX5BvvbZD9j7bf8lgenTqxJs6wj55FzRkZ1cxQhUOvrfUICyaFBEiIY9n7ZPHDu5BQR_=s0"></p>

## **Nomor 6**
Cari username dan password ketika melakukan login ke FTP Server!

### Solusi
Gunakan command ``` ftp.request.command == "USER" || ftp.request.command == "PASS" ```
user		: **secretuser**
pass		: **aku.pengen.pw.aja**
<p align="center"><img width="70%" src="https://lh6.googleusercontent.com/l_5SwB4N6qD5yRLnattTOewIYfeYdkQMXe4QaMgNMFC3bQCac7au4ewv6JOfpT48jveZ-J-9nuKRO6vWaBvkBNpgKU2NI2lE-OYfMQi8uu7847CdJnEpFSwoTtBUfj5TJUb49AQM=s0"></p>

## **Nomor 7**
Ada 500 file zip yang disimpan ke FTP Server dengan nama 0.zip, 1.zip, 2.zip, ..., 499.zip. Simpan dan Buka file pdf tersebut. (Hint = nama pdf-nya "Real.pdf")

### Solusi
- Melakukan filter command ``` tcp contains “Real.pdf” ``` untuk mendapatkan pdf yang diinginkan
<p align="center"><img width="70%" src="https://lh5.googleusercontent.com/wWEnYOPnb4vkmslFvCjdDOKN3Ms0z-tikm6EidyX2O_jZ48InEwsU4pV9IeuycED-4BVCezLjMVyXbT1miHpF6rG9gcpKZQEPd7OLRkZCZh8m4n3K_ygyNG_CfENls_8LdIjPxHV=s0"></p>

- Melakukan download file dengan cara klik kanan, lalu pilih **Follow -> TCP Stream**, lalu pilih Raw dan Save As, simpan dengan nama file “Real.zip”
<p align="center"><img width="70%" src="https://lh4.googleusercontent.com/9HpMXINjV5eCU5-0cvrWG9J51SHldjt8A3lASoBsujLcSdKIzsaJFrmjdFL0ipDqm1SOMhm8cEwSoTDNWgtTL3BR1ZPG4d3P5lnS7Jj8nTLzykdLtLNGjn1snUMz0CPblctXHlBG=s0"></p>

Hasilnya :
<p align="center"><img width="70%" src="https://lh3.googleusercontent.com/QZa8RLMffAG0qWpAC9Al4Xs2n75tS6VCMxvBrrZTKQ5ZnabBWyHLc85PU-6FSbXbTqVfP5Pb8econNqP5m_znoDPt0IYtsyieqdEGjUPDheYMKqQTlBHRun0dhtLMkpNr8NsDr-K=s0"></p>

## **Nomor 8**
Cari paket yang menunjukan pengambilan file dari FTP tersebut!

### Solusi
Menggunakan command ``` ftp.request.command == RETR ```
<p align="center"><img width="70%" src="https://lh6.googleusercontent.com/Y0U1KAjA_AvQgU9OAms5CQCreuMY7bAGX9l5qvx-FvW5xmrtJELEeCUXUXPIPlTm3_VwfPIDrFEMnuqRgQtAhhi7pIlJPUAMjkwE3e8TOmB77lqZbKMN9vU8d97fz2R1I_uwMRBw=s0"></p>

## **Nomor 9**
Dari paket-paket yang menuju FTP terdapat inidkasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama "secret.zip". Simpan dan buka file tersebut!

### Solusi
- Gunakan command ``` ftp-data.command contains secret.zip ```
<p align="center"><img width="70%" src="https://lh3.googleusercontent.com/s3Re42QlhuCnFlCM2A02dKzmEBKDe_UNHgdIi25k6BHDRAKyVFMxkO_mx4vx2KWolnEUGjbEBA1memZByVB81CSxV9lE122bAeYqy-uW1l_1We_lUDA1wwOPuurkXpd7pNiU95nK=s0"></p>

- Melakukan download file dengan cara klik kanan, lalu pilih **Follow -> TCP Stream**, lalu pilih Raw dan Save As, simpan dengan nama file “secret.zip”
<p align="center"><img width="70%" src="https://lh3.googleusercontent.com/o_al4I16AGeWUOfGX-SiRK7jt2xIBTZXXqI7ZxNnRCEa-4bXefIQ43YEcA3uMvd3uYAkDSz9D2n-ZXQWz8ye4LkaDtwfq5FGarTVai78FfjsO_HdcJFxY-X-9m7DCRNhbu6J4-db=s0"></p>

- File .zip harus dibuka dengan password yang dicari di soal no.10
<p align="center"><img width="70%" src="https://lh5.googleusercontent.com/OyOEnMq9Fkvl2BSPiqyR4p0oO9kj7Zj_YGVUr633tv1_g4zagBtGKdhFq4lRJ2PVK4tDIr7W3UmE-hsV8tyL-yg1edvJoTzs2cY1DOzrR8Z44ywfyqptUkk0CE1tn1XhZ2wVQPsM=s0"></p>

## **Nomor 10**
Selain itu terdapat "history.txt" yang kemungkinan berisi history bash server tersebut! Gunakan isi dari "history.txt" untuk menemukan password untuk membuka file rahasia yang ada di "secret.zip"!

### Solusi
- Gunakan command ``` ftp-data.command contains history.txt ```
<p align="center"><img width="70%" src="https://lh6.googleusercontent.com/ySnnCQ60scBkE_iL6bWUul_O2kbvBVyxybPYOIjTvo3JCzLb_eo-YAqvZAsRo1QrsyoTJ1ct6TnQf1Mp7s8AgEj3pSU7_fXnE5mXjEp6ufnKQ-pyRq8EjelzfE1n_foBeLzLftKV=s0"></p>

- Melakukan download file dengan cara klik kanan, lalu pilih **Follow -> TCP Stream**, lalu pilih Raw dan Save As, simpan dengan nama file “history.txt”
- File yang berhasil di extract :
<p align="center"><img width="70%" src="https://lh4.googleusercontent.com/VOz0E1x-2JQCrkDuLOdFBxrhxlP9jCPNvgaigP1FDeHJdlz1i6nig0F5qUGqDUDAw-UDbVmEO8XBqaJIRLMEaUb65A5_Db5STNFMZNUR9wMzof1b2sqTlmPCiqW-EVf3Q0qbHLvX=s0"></p>

- Di dalam file history.txt terdapat kode CLI. Pada kode tersebut terdapat variabel key yang mengambil nilai yang ada di dalam bukanapaapa.txt. Variabel key tersebut pada line 290 menjadi password dari file secret.zip. Sehingga langkah selanjutnya adalah mencari file bukanapaapa.txt untuk mendapatkan nilai yang ada di dalamnya untuk menjadi password secret.zip dengan menggunakan command ``` ftp-data.command contains bukanapaapa.txt ```
<p align="center"><img width="70%" src="https://lh5.googleusercontent.com/kt4RgVjXFrPkjbEy1QH_-n1gmwxwyPWOTaHgM8y3dgMtnPLrtgRPe5TbXE1oAZJ92EylbVnwfeWDt8H__Sxnn04mF9mN9-kKQYwEz4i7A1j_gw_qiswxusRWyqLqoz7Nk1NWzYga=s0"></p>

- Isi dari bukanapaapa.txt :
<p align="center"><img width="70%" src="https://lh6.googleusercontent.com/2nNSTN_I_HI6Bif3X7AFfgSUPmOqNDsj6QU4YehOpNM0ahbBfLmLcGzklzOWt3bhNWJglqcqAHXw8cmtPBpJuiDBRLToggQNGRJQzbaFFjfv6HygGzp0bFJKktEsp4LJeXLQ7Tdp=s0"></p>

- Selanjutnya membuka file secret.zip dengan password **“d1b1langbukanapaapajugagapercaya”** . Hasilnya adalah sebagai berikut
<p align="center"><img width="70%" src="https://lh3.googleusercontent.com/1g8mNTS-shdi9Wp0PKezQCQ8upKeTxM4dqWInHm35CZBv4Q8NhaH_9J6AG7sagI2eFq1HZ2pgWS9o2xAODpcI9R0x25AOeZQk5rPUcKpalffwbiC8Eqj53kvONIfeMedgKo55Rvi=s0"></p>

## **Nomor 11**
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80! 

### Solusi
- Filter command: ``` src port 80 ```
<p align="center"><img width="70%" src="https://lh6.googleusercontent.com/E5skaoy3pMO_NrNO_ODrwPKpwxRaWa7P0t4myF5KSPr3RMMZVF0SuU-RVuQS0Ct60J5y9pfMh4yNG1IrU8ZgL1YLmFAR8Vy8xIDjBg-dJNBjcIxluULcD5QRpdEfT3SV1AbNmNp3=s0"></p>

## **Nomor 12**
Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!

### Solusi
- Filter command: ``` port 21 ```
<p align="center"><img width="70%" src="https://lh3.googleusercontent.com/EbhYdDmyWcqU5P77t-HyJ1nXDx6fRmBTOeGNSrcDVSXw9LckGRk7QDI4be58DHta78ccFfH_D3NLojCqYCTTfdNcTSL65FzNdID5k_aWkU7oAN-ZRXJ76ns8njW7D_z5sesmDeUU=s0"></p>

## **Nomor 13**
Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!

### Solusi
- Filter command: ``` dst port 443 ```
<p align="center"><img width="70%" src="https://lh3.googleusercontent.com/FswMWqqOSbmH0MQDQptE0XI3wU1ytkLZJMEhWNMQIisXnWZoOrKJmg7kUYTb_ROk8CWR6oyJ1d7iNcU1m0yOiiirXRVPaUlM77O0DSx1cntUhgrTRmN4lICjPmeICmskEFS0HpW4=s0"></p>

## **Nomor 14**
Filter sehingga wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!

### Solusi
- Akses kemenag.go.id pada browser
- Pada wireshark, gunakan capture filter ``` dst host kemenag.go.id ```
<p align="center"><img width="70%" src="https://lh5.googleusercontent.com/OeNRZVgzGV0aWdsrVA2SZf3PMWmxJs-FA8v22kLMOFEb3uajrM-5JnaCyKbJhONRlB3H6o2V2BFce5Q5Ub0TwAR5Exsg0PfRrc-Mm21fQtShhLNrFYDC2ft6W2SLS-gYMrv4_vYL=s0"></p>

## **Nomor 15**
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

### Solusi
- Temukan dahulu IP Address kita dengan cara membuka command prompt dan masukkan command **ipconfig**
<p align="center"><img width="70%" src="https://lh5.googleusercontent.com/bMm8DOS9rtEKe-gFel9ufR9F-SuGo4xuz0HWjrbEDrCoT8oxbGlYBD81fnbCMlRPnLQtuyZqiINlrr0HveUI3mBQhnUT7rwD_U4UKbqt4fCH98FORWygg7Bx4bY0_u2_GysNpeX9=s0"></p>

- Gunakan capture filter ``` ip src 192.168.100.22 ```
<p align="center"><img width="70%" src="https://lh6.googleusercontent.com/yop_ofDA3hP1O-av3hA3bvDKarAP43c3M0Vt812hx6n8qBb4lOqG70C3gl9Ae0aV8ABWs8u4OUAAE2PW5yFxlI-B3VSHh79kKy1FyrYOojIVqyz-WaUQv1qyR5SUo4BiEHvRRyzz=s0"></p>
