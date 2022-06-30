| Nama   | Sardin         |
| ------ | -------------- |
| NIM    | 312010135      |
| Kelas  | TI.20.A1       |
| Matkul | Pemograman web |

# Pratikum 13:Framework Lanjutan (Modul Login)

## Langkah-langkah Praktikum

### 1). Membuat Model User

Selanjutnya adalah membuat Model untuk memproses data Login. Buat file baru pada direktori app/Models dengan nama UserModel.php
![img](img/ss1.png)

### 2). Membuat Controller User

Buat Controller baru dengan nama User.php pada direktori app/Controllers. Kemudian tambahkan method index() untuk menampilkan daftar user, dan method login() untuk proses login.
![img](img/ss2.png)

### 3). Membuat View Login

Buat direktori baru dengan nama user pada direktori app/views, kemudian buat file baru dengan nama login.php.
![img](img/ss3.png)

### 4). Membuat Database Seeder

Buat direktori baru dengan nama user pada direktori app/views, kemudian buat file baru dengan nama login.php.

```
 php spark make:seeder UserSeeder
```

![img](img/ss4.png)

### Uji Coba Login

Selanjutnya buka url http://localhost:8080/user/login seperti berikut:
![img](img/ujicoba1.png)

### 5). Menambahkan Auth Filter

Selanjutnya membuat filer untuk halaman admin. Buat file baru dengan nama Auth.php pada direktori app/Filters.
![img](img/ss5.png)
Selanjutnya buka file app/Config/Filters.php tambahkan kode berikut: 'auth' => App\Filters\Auth::class
![img](img/ss6.png)
Selanjutnya buka file app/Config/Routes.php dan sesuaikan kodenya.
![img](img/ss7.png)

### Pertanyaan dan Tugas

Selesaikan programnya sesuai Langkah-langkah yang ada. Anda boleh melakukan improvisasi.

Membuat Tombol Home pada bagian login pada bagian views\user\login.php tembahkan tombol untuk kembali ketampilan awal.<br>
![img](img/ss8.png)

Tampilan

![img](img/ss10.png)

### Membuat Tombol Logout

Memberikan tombol logout pada bagian admin

![img](img/ss11.png)

Tampilan

![img](img/ss12.png)
