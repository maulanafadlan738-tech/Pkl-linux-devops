# Laporan langkah langkah mengpush dari local ke github, menggunakan git bash


## Judul

Penggunaan Git dan GitHub untuk Manajemen Versi dan Publikasi Repository

---

## Identitas Peserta

* Nama            : Fadlan Maulana
* Kelas / Jurusan : XII
* Tempat PKL      : PT. Edifly

---

## 1. Pendahuluan

Git adalah sistem version control yang digunakan untuk mengelola perubahan file atau kode secara terstruktur. GitHub adalah platform berbasis web yang digunakan untuk menyimpan repository Git secara online dan mendukung kolaborasi tim.

Tujuan dari praktikum ini adalah memahami dasar penggunaan Git dan GitHub serta mempraktikkan proses pembuatan repository dan pengiriman (push) file ke GitHub.

---

## 2. Tujuan Praktikum

1. Membuat akun GitHub
2. Memahami fungsi dasar Git dan GitHub
3. Menggunakan perintah dasar Git
4. Membuat repository di GitHub
5. Mengirim (push) file ke repository GitHub

---

## 3. Alat dan Bahan

* Laptop / PC
* Sistem Operasi Windows / Linux
* Git Bash
* Akun GitHub
* Koneksi Internet

---

## 4. Langkah Kerja

### 4.1 Membuat Akun GitHub

1. Mengakses website [https://github.com](https://github.com)
2. Klik tombol **Sign Up**
3. Mengisi username, email, dan password
4. Melakukan verifikasi akun
![sign up git hub](/assets/signup.png)

---

### 4.2 Konfigurasi Git

Perintah yang digunakan:

```bash
git config --global user.name "Fadlan Maulana"
git config --global user.email "maulanafadlan738@gmail.com"
```

Konfigurasi ini digunakan untuk mengatur identitas pengguna yang akan tercatat di setiap commit.

---
![gitconfig](/assets/gitconfig.png)

### 4.3 Inisialisasi Repository Lokal

```bash
git init
```

Perintah ini digunakan untuk membuat repository Git baru pada folder lokal.
![git init](/assets/gitinit.png)

---

### 4.4 Menambahkan File ke Staging Area

```bash
git add .
```

Perintah ini digunakan untuk menambahkan semua file ke staging area agar siap di-commit.
![gitadd](/assets/gitadd..png)

---

### 4.5 Commit Perubahan

```bash
git commit -m "Initial commit"
```

Commit digunakan untuk menyimpan perubahan ke dalam repository dengan pesan keterangan.
![git commit](/assets/gitcom.png)

---

### 4.6 Membuat Repository di GitHub

1. Login ke GitHub
2. Klik **New Repository**
3. Isi nama repository
4. Klik **Create Repository**
![create repository](/assets/create%20repository.png)
---

### 4.7 Menghubungkan Repository Lokal ke GitHub

```bash
git remote add origin https://github.com/username/nama-repo.git
```

Perintah ini digunakan untuk menghubungkan repository lokal dengan repository GitHub.
![git remote add](/assets/gitremad.png)
---

### 4.8 Push ke GitHub

```bash
git push -u origin master
```
![git push](/assets/gitpush.png)
Perintah ini digunakan untuk mengirim file dari repository lokal ke GitHub.

---

## 5. Hasil Praktikum

Repository berhasil dibuat dan file berhasil di-push ke GitHub.
![berhasil](/assets/berhasil.png)
Link Repository:

```
https://github.com/maulanafadlan738-tech/Pkl-linux-devops
```

---

## 6. Kesimpulan

Dengan menggunakan Git dan GitHub, pengelolaan versi file menjadi lebih terstruktur, aman, dan mudah untuk dikembangkan secara individu maupun tim.

---

## 7. Dokumentasi

(Lampirkan screenshot proses konfigurasi Git, pembuatan repository, dan hasil push ke GitHub)

---

## 8. Penutup

Demikian laporan praktikum ini dibuat sebagai bentuk dokumentasi kegiatan yang telah dilakukan.
