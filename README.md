# LapKI_Pertemuan5_RivaMahyuli_478709

ANALISIS dan PEMBAHASAN

*TUGAS1 Ekstrak Executable dari PCAP 
Wireshark adalah salah satu alat analisis lalu lintas jaringan yang paling populer dan digunakan secara luas. Fungsi utama Wireshark dalam menganalisis log dalam lalu lintas adalah untuk menangkap dan menganalisis paket yang dikirim dan diterima di jaringan. Beberapa fungsi utama Wireshark dalam menganalisis log dalam lalu lintas meliputi:

Menangkap Paket: Wireshark memungkinkan pengguna untuk menangkap dan merekam semua paket yang melewati jaringan, termasuk paket dari berbagai protokol seperti TCP, UDP, HTTP, FTP, DNS, dan lainnya.

Menganalisis Paket: Wireshark memungkinkan pengguna untuk menganalisis setiap paket yang ditangkap dan mengeksplorasi isinya. Ini memungkinkan pengguna untuk memeriksa dan memvalidasi data yang dikirim dan diterima oleh aplikasi atau sistem di jaringan.

Menganalisis Protokol: Wireshark memungkinkan pengguna untuk menganalisis dan mempelajari berbagai protokol jaringan, termasuk protokol tingkat rendah seperti TCP/IP, serta protokol tingkat lebih tinggi seperti HTTP, SMTP, FTP, dan lainnya.

Filter Paket: Wireshark memungkinkan pengguna untuk membuat filter untuk paket yang ditangkap sehingga hanya paket tertentu yang ditampilkan dan dianalisis. Ini mempermudah pengguna dalam mencari dan menganalisis paket yang spesifik dan relevan.

Grafik Lalu Lintas: Wireshark memungkinkan pengguna untuk membuat grafik lalu lintas jaringan yang menampilkan jumlah paket yang ditangkap, serta bandwidth yang digunakan. Ini mempermudah pengguna dalam memantau dan memahami lalu lintas jaringan.

Pemecahan Masalah: Wireshark merupakan alat yang sangat berguna dalam pemecahan masalah jaringan. Dengan menggunakan Wireshark, pengguna dapat menemukan dan memperbaiki masalah jaringan seperti bottleneck, latency, dan paket yang hilang atau korup.

Secara keseluruhan, Wireshark sangat bermanfaat dalam menganalisis log dalam lalu lintas jaringan dan memungkinkan pengguna untuk memahami lebih dalam tentang kinerja jaringan dan protokol yang digunakan.

*TUGAS2 Persiapan Log File pada Security Onion Virtual Machine
- ELK (Elasticsearch, Logstash, dan Kibana) adalah solusi untuk mencapai hal berikut:
• Menormalkan, menyimpan, dan mengindeks log dengan volume dan tarif tak terbatas.
• Menyediakan antarmuka pencarian dan API yang sederhana dan bersih.
• Menyediakan infrastruktur untuk mengingatkan, melaporkan, dan berbagi log.

- Zeek (sebelumnya disebut Bro) adalah kerangka kerja yang dirancang untuk menganalisis lalu
lintas jaringan secara pasif dan menghasilkan log peristiwa berdasarkan itu. Setelah analisis lalu
lintas jaringan, Zeek membuat log yang menjelaskan peristiwa seperti berikut:
• Koneksi jaringan TCP/UDP/ICMP
• aktivitas DNS
• aktivitas FTP
• Permintaan dan balasan HTTPS
• Jabat tangan SSL/TLS
 
- Snort dan SGUIL
Snort adalah IDS yang bergantung pada aturan yang telah ditentukan sebelumnya untuk semua kejadian yang berbahaya. Snort melihat ke semua bagian dari paket jaringan (header dan payload), mencari pola yang ditentukan dalam aturannya. Saat, Snort mengambil tindakan yang ditentukan dalam aturan yang sama.

SGUIL menyediakan antarmuka grafis untuk log dan peringatan Snort, memungkinkan analisis keamanan untuk beralih dari SGUIL ke alat lain untuk informasi lebih lanjut. Misalnya, jika paket yang berpotensi berbahaya dikirim ke server web dan Snort memunculkan peringatan, SGUIL akan
peringatan itu. Analis kemudian dapat mengklik kanan peringatan itu untuk mencari database ELSA atau Bro untuk pemahaman yang lebih baik tentang acara tersebut.

Normalisasi log penting dan tergantung pada lingkungan yang digunakan. Alat populer menyertakan fitur normalisasi mereka sendiri, tetapi normalisasi log juga dapat dilakukan secara manual. Saat menormalkan dan menyiapkan file log secara manual, periksa ulang skrip untuk memastikan hasil yang diinginkan tercapai. Skrip normalisasi yang ditulis dengan buruk dapat mengubah data, secara langsung berdampak pada pekerjaan analis

*TUGAS3 Menafsirkan Data HTTP dan DNS untuk Mengisolasi Pelaku Ancaman

1. alamat IP sumber, IP tujuan, dan nomor port tujuan
<img width="352" alt="image" src="https://user-images.githubusercontent.com/99727334/226173290-ce24dee8-2340-4731-9700-0053675cc347.png">
source IP      = 209.165.200.227
destination IP = 209.165.200.235

nomor port tujuan adalah 80
<img width="357" alt="image" src="https://user-images.githubusercontent.com/99727334/226173364-fbcf1294-8d62-4a0a-a2a6-6776c40264a1.png">

2. daftar 10 hasil pertama
<img width="354" alt="image" src="https://user-images.githubusercontent.com/99727334/226173557-039e3434-4e62-4e69-90a3-95ffcf330493.png">
<img width="354" alt="image" src="https://user-images.githubusercontent.com/99727334/226173574-68736f5e-1c8c-41ee-b87f-2c25e396ae88.png">


detail informasi dari salah hasil pertama
<img width="351" alt="image" src="https://user-images.githubusercontent.com/99727334/226173538-c28a3f2a-11c3-4c4a-a644-176bdf11cb41.png">

timestamp dari hasil pertama adalah 12 june 2020, 21:30:09.445

3. contoh username, password , dan signature yang telah dieksfiltrasi
<img width="394" alt="image" src="https://user-images.githubusercontent.com/99727334/226173699-0ff0f510-b98d-45ab-a592-0ee3bd0871fa.png">

4. alamat IP klien dan server DNS.
<img width="359" alt="image" src="https://user-images.githubusercontent.com/99727334/226173746-61237c5c-e8db-4739-a36f-aa03493b2ba4.png">

5. Apakah subdomain dari subdomain kueri DNS? Jika tidak, apa teksnya?
SECRET DOCUMENTS
DO NOT SHARE
This document contains information about the last security breach
<img width="360" alt="image" src="https://user-images.githubusercontent.com/99727334/226173937-5d7c2730-32cc-4808-a97e-688eba0bcf96.png">


Apa yang disiratkan hasil ini tentang permintaan DNS khusus ini? Apa signifikansi yang lebih besar? Hasilnya menunjukkan bahwa permintaan DNS terpisah, permintaan terkoordinasi yang berisi konten tersembunyi. Signifikansi yang lebih besar dari hasilnya adalah bahwa permintaan DNS dapat digunakan untuk menyembunyikan pengiriman file dan melewati keamanan jaringan

Apa yang mungkin membuat kueri DNS yang disandikan ini dan mengapa DNS
dipilih sebagai sarana untuk mengekstrak data?
Ada kemungkinan bahwa malware membuat permintaan ini dengan menelusuri
dokumen di host dan menyandikan kontennya dalam heksadesimal dan kemudian
membuat kueri DNS yang menggunakan string heksadesimal sebagai subdomain
DNS. Permintaan DNS sangat umum dikirim dari jaringan ke internet, sehingga
permintaan DNS mungkin tidak dipantau.
