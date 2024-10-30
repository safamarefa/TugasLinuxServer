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

### 5. modifikasi file *ssh_config* untuk mencegah terjadinya file yang rusak, kita bisa terlebih dahulu menyalin file *ssh_config* dengan menggunakan command:

*$ cp /etc/ssh/ssh_config /etc/ssh/ssh_config.backup*

*$ nano /etc/ssh_config*

saat membuka file *ssh_config* menggunakan cmd nano, kita ubah config dengan mengubah baris yang ada unsur port 22: Protocol 2 & Port 40

![Screenshot (448)](https://github.com/user-attachments/assets/6d685960-4823-4587-9adc-3153a8dd8316)

### 6. untuk mengaktifkan cmd yang sudah kita lakukan, kita dapat menggunakan cmd:

*$ ufw allow 40/tcp*

*$ ufw enable*

*$ ufw status*

![Screenshot (451)](https://github.com/user-attachments/assets/865cc8c8-ea51-4943-af32-e47c9cf5e6b7)

![Screenshot (453)](https://github.com/user-attachments/assets/79b6ac3f-4257-43da-a5c8-7dec79d0b48f)

### 7. setelah dilakukannya config, untuk menghubungkan koneksi dapat menggunakan cmd:

*$ ssh -p 40 usernameHost@IPAdress*

![Screenshot (454)](https://github.com/user-attachments/assets/0fb6b0af-61aa-4e1a-909b-333a10fa0723)















