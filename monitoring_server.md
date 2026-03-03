# MONITORING SERVER MENGGUNAKAN SHELL SCRIPT .SH & CRONJOB UNTUK OTOMATISASI INFORMASI DARI SERVER
## ALUR KERJA SCRIPT DAN CRONJOB
Script `server_monitor.sh` digunakan untuk melakukan monitoring kondisi server secara otomatis. Script mengambil informasi uptime, penggunaan disk, memory, CPU load, IP address, serta waktu eksekusi. Script dijalankan secara otomatis setiap 2 menit menggunakan cronjob. Hasil monitoring dikirimkan ke grup Telegram melalui Telegram Bot API sehingga administrator dapat memantau kondisi server secara real-time tanpa harus login ke server.

---

## Informasi Server yang Dimonitor
- Uptime server
- Disk usage
- Memory usage
- CPU load
- IP address server
- Tanggal dan waktu eksekusi script

---

## Tools yang Digunakan
- Ubuntu Server
- Bash Shell
- Cronjob
- Telegram Bot
- Telegram Bot API
- Curl untuk 

---

## Langkah-Langkah Konfigurasi

### 1. Membuat Telegram Bot
1. Membuat bot melalui @BotFather.

Buka Telegram, lalu search dan klik `@BotFather`.
![Screenshoot](/assets/botfaher.png)

2. Membuat bot.

Ketik `/start`, `/newbot`, Beri nama bot nya lalu beri username bot nya. Jangan lupa untuk menyimpan tokennya.
![Screenshoot](/assets/newbot.png)
![Screenshoot](/assets/lanserver_bot.png)

3. Ping bot yang sudah di buat.

Jika sudah terbuat, Cari bot lalu `/start` untuk mengaktifkan. 
![Screenshoot](/assets/test.png)

3. Menambahkan bot ke grup Telegram.

Buat grup terlebih dahulu di tele `"lanserver_monitoring"`, lalu tambahkan bot yang telah di buat. Jika sudah ketik `test` atau apapun untuk mengambil chat id menggunakan API.
![Screenshoot](/assets/grupaddbot.png)
![Screenshoot](/assets/test.png)

4. Mengambil Chat ID grup menggunakan Telegram API.

Jika sudah di ketik test, selanjutnya kita akan mengambil chat id `(-XXXXXXXX)` untuk di cantumkan di script yang akan di buat.
Untuk melihatnya gunakan ini. 
`https://api.telegram.org/botBOTTOKEN/getUpdates`
![Screenshoot](/assets/id.png)
---

### 2. Membuat Shell Script
1. Membuat file `server_monitor.sh`.

Jika Bot dan id sudah terbuat dan ada, Selanjutnya kita akan membuat shell script .sh untuk output monitoringnya dengan ketentuan 
- Uptime server
- Disk usage
- Memory usage
- CPU load
- IP address server
- Tanggal dan waktu eksekusi script
Ketik
 `nano monitoring_lanserver.sh`.
![Screenshoot](/assets/sh.png)

2. Menambahkan script monitoring server.

Jika Bot dan id sudah terbuat dan ada, Selanjutnya kita akan membuat shell script .sh untuk output monitoringnya dengan ketentuan 
- Uptime server
- Disk usage
- Memory usage
- CPU load
- IP address server
- Tanggal dan waktu eksekusi script
Ketik `nano monitoring_lanserver.sh`.
 
di nano masukkan 
![Screenshoot](/assets/nanocp.png)

3. Memberikan permission executable pada script.

Jika sudah di buat, `ctrl + x` untuk exit, `enter`, dan `ctrl + o` untuk save.
Selanjutnya kita executable file .sh tadi yang sudah di buat dengan command `chmod +x monitoring_lanserver.sh`
![Screenshoot](/assets/exec.png)

dan coba ls -l file sh `ls -l monitoring_lanserver.sh`, untuk melihat output executable sudah benar atau belum
![Screenshoot](/assets/exec1.png)

4. test file .sh Berjalan

Jika sudah test menggunakan `./monitoring_lanserver.sh` untuk melihat ouput yang di minta, cek juga di grup telegram
![Screenshoot](/assets/testsh.png)
![Screenshoot](/assets/testsh1.png)
---
### 3. Membuat penjadwalan otomatis menggunakan cronjob
1. Konfigurasi cronjob 

Gunakan command `crontab -e` untuk masuk ke teks editor cronjob, di dalamnya ada petunjuk template untuk membuat konf cronjob/crontab. Di bagian paling bawah masukkan conf sesuai template misal di sini saya akan mengkonfigurasi monitoring server yang tadi sudah di buat menggunakan file script `.sh` agar muncul informasi yang di cantumkan di `.sh`  setiap 2 menit oleh bot tele. 
`*/2 * * * * /root/monitoring_lanserver.sh`
![Screenshoot](/assets/crontab%20-e.png)
![Screenshoot](/assets/nano%20crontab.png)
![Screenshoot](/assets/conf%20cront.png)
 
2. Jika sudah, tinggal cek di grup telegram, apakah pesan sudah masuk tiap 2 menit sekali oleh bot tele.
![Screenshoot](/assets/pesan%20masuk.png) 