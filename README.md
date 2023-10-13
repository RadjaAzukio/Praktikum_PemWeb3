# Praktikum_PemWeb3

# Praktikum 3 web: Membuat List, Table dan Form

## Langkah-langkah Praktikum
-Persiapan membuat dokumen HTML dengan nama file lab3_list.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
</body>
</html>
```

![image](https://github.com/RadjaAzukio/Praktikum_PemWeb3/assets/115551911/4dd09c0a-15a9-4ab8-afcc-e6f7b999627f)


### Membuat Ordered List
- Kemudian tambahkan kode untuk membuat Ordered List seperti berikut.
```
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
      <li>Pemrograman Web</li>
      <li>Sistem Informasi</li>
      <li>Basis Data 2</li>
    </ol>
</section>
```

### Membuat Unorderd List
- Kemudian tambakan kode untuk membuat Unordered List, setelah deklarasi ordered list pada section unordered-list, seperti berikut.
```
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
      <li>Jaringan Komputer</li>
      <li>Struktur Data</li>
      <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```

![image](https://github.com/RadjaAzukio/Praktikum_PemWeb3/assets/115551911/e663bf22-4f7d-4aab-a70a-ebaa3e9614bd)



### Membuat Description List
- Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.
```
<section id="unorder-list">
        <h2>Description List</h2>
        <dl>
            <dt>Fakultas Teknik</dt>
            <dd>Teknik Industi</dd>
            <dd>Teknik Informatika</dd>
            <dd>Teknik Lingkungan</dd>
            <dt>Fakultas Ekonomi dan Bisnis</dt>
            <dd>Akuntasi</dd>
            <dd>Manajemen</dd>
            <dd>BisnIS Digital</dd>
        </dl>
    </section>
```


![image](https://github.com/RadjaAzukio/Praktikum_PemWeb3/assets/115551911/f21010d6-145e-4654-9e21-a9ac81d3216b)



### Membuat Tabel
- Buat file baru dengan nama lab3_tabel.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML lanjutan</title>
</head>
<body>
  <header>
    <h1>Membuat table</h1>
  </header>
</body>
</html>
```

- Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:
```
<table border="1" cellpadding="4" cellspacing="3">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>Teknik</td>
      <td>Teknik Informatika</td>
  </tr>
  <tr>
      <td>2.</td>
      <td>Teknik</td>
      <td>Teknik Industri</td>
  </tr>
  <tr>
      <td>3.</td>
      <td>Teknik</td>
      <td>Teknik Lingkungan</td>
  </tr>
  </tbody>
</table>
```

![image](https://github.com/RadjaAzukio/Praktikum_PemWeb3/assets/115551911/b63e970a-f26b-4213-ae58-cd93889b8887)


### Mengatur Margin dan Padding
- Untuk mengatur margin dan padding pada cel data, tambahkan atribut cellpadding dan cellspacing pada tag table.

```
<table border="1" cellpadding="4" cellspacing="3">
```

![image](https://github.com/RadjaAzukio/Praktikum_PemWeb3/assets/115551911/61b7c339-751e-4d09-8064-cf713e438e7b)



### Menggabungkan Sel Data
- Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara horizontal).
```
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td rowspan="3">Teknik</td>
      <td>Teknik Informatika</td>
  </tr>
  <tr>
      <td>2.</td>
      <td>Teknik Industri</td>
  </tr>
  <tr>
      <td>3.</td>
      <td>Teknik Lingkungan</td>
  </tr>
  </tbody>
</table>
```
![image](https://github.com/RadjaAzukio/Praktikum_PemWeb3/assets/115551911/48e37763-fe59-4916-90df-ea499c274c98)


### Membuat Form
- Buat file baru dengan nama lab3_form.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>Membuat From</header>
</body>
</html>
```

- Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut.

```
form action="proses.php" method="post">
    <fieldset>
        <legend>Data Pelanggan</legend>
    <p>
        <label for="nama">Nama</label>
        <input type="text" id="nama" name="nama">
    </p>
    <p>
        <label for="alamat">Alamat</label>
        <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
    </p>
    <p>
        <label>Jenis Kelamin</label>
        <input id="jk_l" type="radio" name="kelamin" value="L" /><label
        for="jk_l">Laki-laki</label>
        <input id="jk_p" type="radio" name="kelamin" value="P" /><label
        for="jk_p">Perempuan</label>
    </p>
        <p><input type="submit" value="Login"></p>
        </fieldset>
</form>
```

![image](https://github.com/RadjaAzukio/Praktikum_PemWeb3/assets/115551911/8e4c16ce-c6c1-4a86-9dda-0481ab3f401b)


### Menabahkan Style pada Form
- Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.
```
 <style>
        form p > label {
            display: inline-block;
            width: 100px;
        }
        form input[type="text"], form textarea {
            border: 1px solid #197a43;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 5px 15px;
        }
    </style>
```

![image](https://github.com/RadjaAzukio/Praktikum_PemWeb3/assets/115551911/e2196901-47d3-449c-8330-1ded7e00da25)


### Pertanyaan dan Tugas
- Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.

![image](https://github.com/RadjaAzukio/Praktikum_PemWeb3/assets/115551911/786624cc-e17d-4f36-98b6-ebb13eb30168)


