# Lab3Web

Nama : Syifa Aurellia Rahma

NIM  : 312210009

Kelas : TI.22.A1

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Instruksi Praktikum|[Click Here](#instruksipraktikum)|
|2|Praktikum|[Click Here](#praktikum)|
|3|Pertanyaan dan Tugas|[Click Here](#pertanyaandantugas)|

## Instruksi Praktikum
> 1. Persiapkan text editor misalnya VSCode.
> 2. Buat folder baru dengan nama Lab3Web
> 3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
> 4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

## Praktikum
**1. Membuat Ordered List & Undordered List**

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

![1](https://github.com/syifaaurellia/Lab3Web/assets/115867244/a24ab92d-1fba-4605-a742-a4dda32759fa)


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

![2](https://github.com/syifaaurellia/Lab3Web/assets/115867244/11fe18db-b456-4904-8f95-701dc1d66b79)


**2. Membuat Description List**

```
<section id="unorder-list">
  <h2>Description List</h2>
  <dl>
    <dt>Fakultas Teknik</dt>
    <dd>Teknik Industri</dd>
    <dd>Teknik Informatika</dd>
    <dd>Teknik Lingkungan</dd>
    <dt>Fakultas Ekonomi dan Bisnis</dt>
    <dd>Akuntansi</dd>
    <dd>Manajemen</dd>
    <dd>Bisnis Digital</dd>
  </dl>
</section>
```

![3](https://github.com/syifaaurellia/Lab3Web/assets/115867244/c9c5516a-02a8-4612-ab03-d10ba1c75476)


**3. Membuat Table**

```
<table border="1" cellpadding="4" cellspacing="0">
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

![4](https://github.com/syifaaurellia/Lab3Web/assets/115867244/df980a75-94de-45dd-b0cc-a8953fe23fb0)


**4. Membuat Margin dan Padding**

```
<table border="1" cellpadding="4" cellspacing="0"></table>
```

![5](https://github.com/syifaaurellia/Lab3Web/assets/115867244/7dfae970-e7a2-45fb-b97b-a9c0ebae228a)


**5. Menggabungkan Sel Data**

```
<tr>
  <td>1.</td>
  <td rowspan="3">Teknik</td>
  <td>Teknik Informatika</td>
</tr>
```

![6](https://github.com/syifaaurellia/Lab3Web/assets/115867244/8f407cc7-da85-441d-8404-7bc9e991ae04)


**6. Membuat Form**

```
<form action="proses.php" method="post">
  <fieldset>
    <legend>Data Pelanggan</legend>
    <p>
      <label for="nama">Nama</label>
      <input type="text" id="nama" name="nama" />
    </p>
    <p>
      <label for="alamat">Alamat</label>
      <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
    </p>
    <p>
      <label>Jenis Kelamin</label>
      <input id="jk_l" type="radio" name="kelamin" value="L" /><label for="jk_l"
        >Laki-laki</label
      >
      <input id="jk_p" type="radio" name="kelamin" value="P" /><label
        qafor="jk_p"
        >Perempuan</label
      >
    </p>
    <p><input type="submit" value="Login" /></p>
  </fieldset>
</form>
```

![7](https://github.com/syifaaurellia/Lab3Web/assets/115867244/07bcf8fc-b430-43da-a3aa-be3cf12c3326)


**7. Menambahkan Style**

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

![8](https://github.com/syifaaurellia/Lab3Web/assets/115867244/fdcea895-6f6b-41d7-b107-0cd4b45e1f4d)


**8. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org**


![Screenshot (46)](https://github.com/syifaaurellia/Lab3Web/assets/115867244/3c8eadc5-7fb4-43ad-bdc6-4a54cd9ee31b)

![Screenshot (47)](https://github.com/syifaaurellia/Lab3Web/assets/115867244/1fc5bf7c-4f16-44bc-bfbb-569a792f5644)


## Pertanyaan dan Tugas
1. Buatlah form yang menampilkan **dropdown** menu dan **listbox** dengan *multiple selection.*

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tugas Form Dropdown and Listbox</title>
    <link rel="style" href="style.css">
</head>

<body>
    <nav>
        <a href="lab3_list.html">List HTML</a>
        <a href="lab3_tabel.html">Tabel HTML</a>
        <a href="lab3_form.html">Form HTML</a>
        <a href="lab3_tugas.html">Form Dropdown & Listbox</a>
    </nav>
    <header>
        <h1>Form Dropdown & Listbox</h1>
    </header>

    <form class="form_tugas">
        <label for="dropdown">Pilih salah satu buah:</label>
        <select name="dropdown" id="dropdown">
            <option value="apel">Apel</option>
            <option value="jeruk">Jeruk</option>
            <option value="durian">Durian</option>
            <option value="mangga">Mangga</option>
            <option value="semangak">Semangka</option>
        </select>

        <br><br>

        <label for="listbox">Pilih beberapa buah:</label>
        <select name="buah[]" multiple id="listbox">
            <option value="apel">Apel</option>
            <option value="jeruk">Jeruk</option>
            <option value="durian">Durian</option>
            <option value="mangga">Mangga</option>
            <option value="semangka">Semangka</option>
            <option value="kelapa">Kelapa</option>
            <option value="anggur">Anggur</option>
            <option value="melon">Melon</option>
            <option value="pepaya">Pepaya</option>
            <option value="nanas">Nanas</option>
        </select>

        <br>

        <input type="submit" value="Submit" id="input_tugas">
    </form>
</body>

</html>
```

```
body {
    font-family: Tahoma;
  }
  
  h1 {
    margin-top: 50px;
    text-align: center;
    color: #3d9a38;
  }
  
  .tabel {
    margin: 20px auto;
  }
  
  form p > label {
    display: inline-block;
    width: 100px;
  }
  
  form input[type="text"],
  form textarea {
    border: 1px solid #4dacd1;
  }
  
  form input[type="submit"] {
    border: 1px solid #84a9d4;
    background-color: #5375b9;
    color: #da8383;
    font-weight: bold;
    padding: 5px 15px;
    border-radius: 10px;
  }
  
  form input[type="submit"]:hover {
    background-color: #2098cb;
    cursor: pointer;
  }
  
  nav {
    background-color: #3fb8e0c5;
    padding: 10px;
    position: fixed;
    top: 0px;
    right: 0px;
    left: 0px;
    text-align: center;
  }
  
  nav a {
    color: #fff;
    text-decoration: none;
    padding: 2px 4px;
    font-size: 13px;
  }
  
  nav a:hover {
    color: #487689;
  }
  
  nav a:active {
    color: #3dd274;
  }
  
  /* Style untuk form dropdown & listbox */
  .form_tugas {
    max-width: 400px;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #a9e664;
    background-color: #eb9ee1;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  
  /* Style untuk label */
  .form_tugas label {
    display: block;
    font-weight: bold;
    margin-bottom: 5px;
  }
  
  /* Style untuk select dropdown dan listbox */
  .form_tugas select {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #be77a7;
    border-radius: 3px;
  }
  
  /* Style untuk tombol Submit */
  .form_tugas #input_tugas {
    background-color: #6caaed;
    color: #984f4f;
    padding: 5px 15px;
    border: none;
    border-radius: 6px;
    cursor: pointer;
  }
  
  .form_tugas #input_tugas:hover {
    background-color: #d469ca;
  }
```

![9](https://github.com/syifaaurellia/Lab3Web/assets/115867244/0635f525-d98c-456d-8621-bbb08d8d39d1)


## Finish, Terima Kasih
