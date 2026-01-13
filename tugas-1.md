# TUGAS 1 - PENGENALAN VISUAL STUDIO CODE & MARKDOWN

## Identitas
- Nama: Fadlan Maulana
- Kelas / PKL: (XII)
- Tanggal: (12-01-2026)

---
### - SYSTEM & USER

## 1. Whoami
Perintah `whoami` digunakan untuk mengetahui user yang sedang aktif di sistem operasi.

![screenshot whoami](/assets/whoami.png)


## 2. hostname
Perintah `hostname` digunakan untuk menampilkan nama host atau nama komputer pada sistem.

![sreenshot hostname](/assets/hostname.png)

## 3. uname -a
Perintah `uname -a` digunakan untuk menampilkan informasi kernel dan arsitektur sistem.

![screenshot uname-a](/assets/uname-a.png)

## 4. uptime
Perintah `uptime` digunakan untuk melihat lama sistem berjalan dan load average.

![screenshot uptime](/assets/uptime.png)

## 5. date
Perintah `date` digunakan untuk menampilkan tanggal dan waktu sistem.

![screenshot date](/assets/date.png)

## 6. timedatectl
Perintah `timedatectl` digunakan untuk melihat konfigurasi waktu dan zona waktu.

![screenshot timedatectl](/assets/timedatectl.png)

## 7. passwd
Perintah `passwd` digunakan untuk mengganti password user aktif.

![screenshot passwd](/assets/passwd.png)

## 8. adduser baru
Perintah `adduser` digunakan untuk menambahkan user baru ke sistem.

![screenshot adduser](/assets/adduser.png)

## 9. usermod -aG sudo userbaru
Perintah `usermod -aG sudo userbaru` ini menambahkan user ke grup sudo agar memiliki hak administrator.

![screenshot usermod](/assets/usermod.png)

## 10. su -
Perintah `su -` digunakan untuk berpindah ke user root.

![screenshot su -](/assets/su-.png)

## 11. exit
Perintah `exit` digunakan untuk keluar dari sesi user root.

![screenshot exit](/assets/exit.png)





### - FILE & DIRECTORY

## 1. ls
Perintah `ls` digunakan untuk menampilkan daftar file dan folder pada direktori saat ini.

![Screenshot ls](/assets/ls.png)

## 2. ls -la
Perintah `ls -la` digunakan untuk menampilkan semua file termasuk file tersembunyi
beserta detail permission, owner, ukuran, dan waktu.

![Screenshot ls -la](/assets/ls-la.png)

## 3. pwd
Perintah `pwd` digunakan untuk menampilkan path direktori kerja saat ini.

![Screenshot pwd](/assets/pwd.png)

## 4. cd
Perintah `cd` digunakan untuk berpindah ke direktori lain.

![Screenshot cd](/assets/cd.png)

## 5. cd ..
Perintah `cd ..` digunakan untuk berpindah ke direktori satu level di atasnya.

![Screenshot cd..](/assets/cd...png)

## 6. mkdir folder
Perintah `mkdir` digunakan untuk membuat folder baru.


![Screenshot mkdir](/assets/mkdir.png)

## 7. mkdir -p folder/subfolder
Perintah `mkdir -p` digunakan untuk membuat folder beserta subfolder secara langsung.

![Screenshot mkdir -p](/assets/mkdir-p.png)

## 8. rm file
Perintah `rm` digunakan untuk menghapus file.

![Screenshot rm](/assets/rm.png)

## 9. rm -rf folder
Perintah `rm -rf` digunakan untuk menghapus folder beserta isinya secara paksa.

![Screenshot rm -rf](/assets/rm-rf.png)

## 10. cp file tujuan
Perintah `cp` digunakan untuk menyalin file ke lokasi tujuan.

![Screenshot cp](/assets/cp.png)

## 11. mv file tujuan
Perintah `mv` digunakan untuk memindahkan atau mengganti nama file.

![Screenshot mv](/assets/mv.png)

## 12. touch file.txt
Perintah `touch` digunakan untuk membuat file kosong baru.

![Screenshot touch](/assets/touch.png)

## 13. stat file
Perintah `stat` digunakan untuk menampilkan informasi detail sebuah file.

![Screenshot stat](/assets/stat.png)

## 14. tree
Perintah `tree` digunakan untuk menampilkan struktur folder secara hierarki.

![Screenshot tree](/assets/tree.png)




### - FILE VIEW & EDIT

## 1. less file
Perintah `less` digunakan untuk melihat isi file secara interaktif
tanpa mengubah isi file tersebut.

![Screenshot less](/assets/less.png)
## 2. head file
Perintah `head` digunakan untuk menampilkan beberapa baris awal dari sebuah file.

![Screenshot head](/assets/head.png)
## 3. tail file
Perintah `tail` digunakan untuk menampilkan beberapa baris terakhir dari sebuah file.

![Screenshot tail](/assets/tail.png)
## 4. tail -f file
Perintah `tail -f` digunakan untuk memantau perubahan isi file secara real-time,
biasanya digunakan untuk melihat log.

![Screenshot tail-f](/assets/tail-f.png)
## 5. nano file
Perintah `nano` digunakan untuk mengedit file menggunakan text editor berbasis terminal.

![Screenshot nano](/assets/nano.png)
## 6. vi file
Perintah `vi` digunakan untuk mengedit file menggunakan editor vi.

![Screenshot vi](/assets/vi.png)
## 7. vim file
Perintah `vim` digunakan untuk mengedit file menggunakan editor vim
yang merupakan versi lanjutan dari vi.

![Screenshot vim](/assets/vim.png)

### ARCHIVE & COMPRESSION

## 1. tar -cvf file.tar folder
Perintah `tar -cvf` digunakan untuk membuat file arsip `.tar`
dari sebuah folder.

![Screenshot tar -cvf](/assets/tar-cvf.png)

## 2. tar -xvf file.tar
Perintah `tar -xvf` digunakan untuk mengekstrak file arsip `.tar`. 

![Screenshot tar -xvf](/assets/tar-xvf.png)

## 3. tar -czvf file.tar.gz folder
Perintah `tar -czvf` digunakan untuk membuat arsip terkompresi `.tar.gz`
dari sebuah folder.

![Screenshot tar -czvf](/assets/tar-czvf.png)

## 4. tar -xzvf file.tar.gz
Perintah `tar -xzvf` digunakan untuk mengekstrak arsip `.tar.gz`.

![Screenshot tar -xzvf](/assets/tar-xzvf.png)

## 5. zip -r file.zip folder
Perintah `zip -r` digunakan untuk membuat file arsip `.zip`secara rekursif dari sebuah folder.

![Screenshot zip -r](/assets/zip-r.png)

## 6. unzip file.zip
Perintah `unzip` digunakan untuk mengekstrak file arsip `.zip`.

![Screenshot unzip](/assets/unzip.png)
### COMAND DOWNLOAD FILE VIA HTTPS/HTTPS

## 1. wget iso_8859-1.txt
Perintah `wget` digunakan untuk mengunduh file melalui protokol HTTP/HTTPS.

![Screenshot iso](/assets/iso.png)
## 2. wget gpl-3.0.txt
Perintah `wget` digunakan untuk mengunduh file teks lisensi GNU GPL.

![Screenshot gpl](/assets/gpl.png)
## 3. wget README.md
Perintah `wget` digunakan untuk mengunduh file README dari repository GitHub.

![Screenshot readme](/assets/readme.png)
## 4. curl -O iso_8859-1.txt
Perintah `curl -O` digunakan untuk mengunduh file dan menyimpannya
dengan nama asli.

![Screenshot curl iso](/assets/curliso.png)
## 5. curl -O gpl-3.0.txt
Perintah `curl -O` digunakan untuk mengunduh file teks melalui HTTPS.

![Screenshot curl gpl](/assets/curlgpl.png)
## 6. curl -L README.md
Perintah `curl -L` digunakan untuk mengikuti redirect dan menyimpan file
dengan nama yang ditentukan.

![Screenshot curl readme](/assets/curlreadme.png)

