# TugasLinuxServer

Nama: R.A. Siti Safa marefa

NIM: 09011282328073

Kelas: SK3A

Laporan tugas server linux

# Protokol SSH
SSH atau Secure Shell adalah protokol jaringan yang menjamin keamanan koneksi antara dua komputer melalui jaringan tidak aman. Dengan SSH, pengguna dapat mengakses dan mengendalikan komputer dari jarak jauh secara aman, berkat enkripsi yang melindungi data yang dikirim. SSH biasanya digunakan untuk login jarak jauh, mentransfer file, dan menjalankan perintah di server atau perangkat lain.

# Pembahasan

### 1. Download terlebih dahulu server ubuntu atau webgoat. Untuk memeriksa alamat IP server host, gunakan perintah *$ifconfig.*
![Screenshot (441)](https://github.com/user-attachments/assets/887f7ab9-9760-4193-a93a-a6d83bd40105)

### 2. Untuk memeriksa port terbuka pada Host Server, kamu bisa memanfaatkan fitur nmap di Linux dengan menggunakan perintah *$nmap.*
![Screenshot (444)](https://github.com/user-attachments/assets/471e0e0b-d254-48b2-92e3-00485c4cfb6b)

### 3. Untuk menghubungkan ke port dengan protokol SSH, gunakan perintah berikut untuk menyambungkan ke port default 22, yaitu:

*$ ssh -p 22 usernameHost@IPAdress*

![Screenshot (452)](https://github.com/user-attachments/assets/91d1b76d-2329-4e30-abe1-bbe9b10df618)

### 4. lalu lakukan konfigurasi port 40 ke host server, untuk memodifikasi lebih luas dapat menggunakan cmd *$sudo su* untuk masuk ke super user mode









