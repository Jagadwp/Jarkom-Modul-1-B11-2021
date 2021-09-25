# Jarkom-Modul-1-B11-2021

## **Kelompok B-11**
- Muhammad Nevin        (05111940000079)
- Albert Filip Silalahi (05111940000116)
- Jagad Wijaya Purnomo	(05111940000132)

## **Nomor 1**
Sebutkan webserver yang digunakan pada <a href='ichimarumaru.tech'>"ichimarumaru.tech"</a>!

### Solusi
- Filter menggunakan filter command http contains “ichimarumaru.tech”
- Kemudian klik kanan, pilih Follow > TCP Stream, dan dapat terlihat bahwa webserver yang digunakan adalah nginx/1.18.0 (Ubuntu), dengan destination port 80 (HTTP).

## **Nomor 2**
Temukan paket dari **web-web** yang menggunakan **basic authentication** method!

### Solusi
Gunakan command ``` http.authbasic ```

## **Nomor 3**
Ikuti perintah di <a href='basic.ichimarumaru.tech'>basic.ichimarumaru.tech</a>! Username dan password bisa didapatkan dari file .pcapng!

### Solusi
- Melakukan display filter ``` http.host ==  basic.ichimarumaru.tech ``` . Pilih yang memiliki method **GET**, lalu akan didapatkan username dan passwordnya
- Login dengan username: **kuncimenujulautan** dan password: **“tQKEJFbgNGC1NCZlWAOjhyCOm6o3xEbPkJhTciZN”** sesuai credentials.
- Masukkan jawaban dari soal yang diberikan


## **Nomor 4**
Temukan paket **mysql** yang mengandung **perintah query select**!

### Solusi
Melakukan display filter ``` mysql.command == 3 and frame matches "SELECT" ``` . 


## **Nomor 5**
Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan password bisa didapat dari **query insert** pada table **users** dari file .pcap!

### Solusi
- Melakukan display filter ``` mysql.command == 3 and frame matches "INSERT" ```
- Login dengan username: **akakanomi** dan password: **pemisah4lautan**
- Tulis jawaban soal yang diberikan

## **Nomor 6**
Cari username dan password ketika melakukan login ke FTP Server!

### Solusi
Gunakan command ``` ftp.request.command == "USER" || ftp.request.command == "PASS" ```
user		: **secretuser**
pass		: **aku.pengen.pw.aja**

## **Nomor 7**
Ada 500 file zip yang disimpan ke FTP Server dengan nama 0.zip, 1.zip, 2.zip, ..., 499.zip. Simpan dan Buka file pdf tersebut. (Hint = nama pdf-nya "Real.pdf")

### Solusi
- Melakukan filter command ``` tcp contains “Real.pdf” ``` untuk mendapatkan pdf yang diinginkan
- Melakukan download file dengan cara klik kanan, lalu pilih **Follow -> TCP Stream**, lalu pilih Raw dan Save As, simpan dengan nama file “Real.zip”

Hasilnya :


## **Nomor 8**
Cari paket yang menunjukan pengambilan file dari FTP tersebut!

### Solusi
Menggunakan command ``` ftp.request.command == RETR ```

## **Nomor 9**
Dari paket-paket yang menuju FTP terdapat inidkasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama "secret.zip". Simpan dan buka file tersebut!

### Solusi
- Gunakan command ``` ftp-data.command contains secret.zip ```
- Melakukan download file dengan cara klik kanan, lalu pilih **Follow -> TCP Stream**, lalu pilih Raw dan Save As, simpan dengan nama file “secret.zip”
- File .zip harus dibuka dengan password yang dicari di soal no.10

## **Nomor 10**
Selain itu terdapat "history.txt" yang kemungkinan berisi history bash server tersebut! Gunakan isi dari "history.txt" untuk menemukan password untuk membuka file rahasia yang ada di "secret.zip"!

### Solusi
- Gunakan command ``` ftp-data.command contains history.txt ```
- Melakukan download file dengan cara klik kanan, lalu pilih **Follow -> TCP Stream**, lalu pilih Raw dan Save As, simpan dengan nama file “history.txt”
- File yang berhasil di extract :

- Di dalam file history.txt terdapat kode CLI. Pada kode tersebut terdapat variabel key yang mengambil nilai yang ada di dalam bukanapaapa.txt. Variabel key tersebut pada line 290 menjadi password dari file secret.zip. Sehingga langkah selanjutnya adalah mencari file bukanapaapa.txt untuk mendapatkan nilai yang ada di dalamnya untuk menjadi password secret.zip dengan menggunakan command ``` ftp-data.command contains bukanapaapa.txt ```
- Isi dari bukanapaapa.txt :

- Selanjutnya membuka file secret.zip dengan password **“d1b1langbukanapaapajugagapercaya”** . Hasilnya adalah sebagai berikut



## **Nomor 11**
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80! 

### Solusi
Filter command: ``` src port 80 ```

## **Nomor 12**
Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!

### Solusi
 Filter command: ``` port 21 ```

## **Nomor 13**
Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!

### Solusi
Filter command: ``` dst port 443 ```

## **Nomor 14**
Filter sehingga wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!

### Solusi
- Akses kemenag.go.id pada browser
- Pada wireshark, gunakan capture filter ``` dst host kemenag.go.id ```


## **Nomor 15**
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

### Solusi
- Temukan dahulu IP Address kita dengan cara membuka command prompt dan masukkan command **ipconfig**
- Gunakan capture filter ``` ip src 192.168.100.22 ```
