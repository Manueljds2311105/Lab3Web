# Lab3Web

**Nama:** Manuel Johansen Dolok Saribu  
**NIM:** 312410493  
**Mata Kuliah:** Pemrograman Web  
**Dosen Pengampu:** Agung Nugroho, S.Kom., M.Kom.  

---

## 1. Persiapan Dokumen HTML
Buat file baru bernama **`lab3_list.html`** dan tuliskan struktur dasar HTML berikut:

```html
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

---

## 2. Membuat Ordered List
Tambahkan kode berikut untuk membuat list terurut:

```html
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
        <li>Pemrograman Web</li>
        <li>Sistem Informasi</li>
        <li>Basis Data 2</li>
    </ol>
</section>
```

**Penjelasan:**  
- `<ol>` digunakan untuk membuat daftar terurut.  
- `<li>` adalah elemen item daftar.  
- Atribut `type` dan `start` bisa digunakan untuk mengubah jenis penomoran.  

![foto](https://github.com/Manueljds2311105/foto/blob/be06d5b3607d4ed0f94b34d81db3909ab4a13b0e/HTML%20Lanjutan%20-%20Google%20Chrome%2010_8_2025%2010_50_39%20AM.png)

---

## 3. Membuat Unordered List
Tambahkan list tanpa urutan angka menggunakan tag `<ul>`:

```html
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```

**Penjelasan:**  
- `<ul>` membuat daftar tidak berurutan.  
- Atribut `type` dapat berupa: `disc`, `circle`, `square`.  

![foto](https://github.com/Manueljds2311105/foto/blob/be06d5b3607d4ed0f94b34d81db3909ab4a13b0e/HTML%20Lanjutan%20-%20Google%20Chrome%2010_8_2025%2010_51_50%20AM.png)

---

## 4. Membuat Description List
Tambahkan description list menggunakan tag `<dl>`, `<dt>`, dan `<dd>`:

```html
<section id="desc-list">
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

**Penjelasan:**  
- `<dl>` mendefinisikan daftar deskripsi.  
- `<dt>` adalah istilah (judul).  
- `<dd>` adalah deskripsi dari istilah tersebut.  

![foto](https://github.com/Manueljds2311105/foto/blob/be06d5b3607d4ed0f94b34d81db3909ab4a13b0e/HTML%20Lanjutan%20-%20Google%20Chrome%2010_8_2025%2010_52_57%20AM.png)

---

## 5. Membuat Tabel
Buat file baru bernama **`lab3_tabel.html`**.  
Tambahkan kode berikut:

```html
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

**Penjelasan:**  
- `<table>` membuat tabel.  
- `<thead>` untuk kepala tabel.  
- `<tbody>` untuk isi tabel.  
- `<tr>` membuat baris, `<th>` untuk judul kolom, `<td>` untuk isi data.  

![foto](https://github.com/Manueljds2311105/foto/blob/be06d5b3607d4ed0f94b34d81db3909ab4a13b0e/HTML%20Lanjutan%20-%20Google%20Chrome%2010_8_2025%2011_01_44%20AM.png)

---

## 6. Menggabungkan Sel (Rowspan & Colspan)

```html
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

**Penjelasan:**  
- `rowspan` digunakan untuk menggabungkan sel secara **vertikal**.  
- `colspan` digunakan untuk menggabungkan sel secara **horizontal**.  

![foto](https://github.com/Manueljds2311105/foto/blob/be06d5b3607d4ed0f94b34d81db3909ab4a13b0e/HTML%20Lanjutan%20-%20Google%20Chrome%2010_8_2025%2011_05_13%20AM.png)

---

## 7. Membuat Form
Buat file baru bernama **`lab3_form.html`**.  
Tambahkan kode berikut:

```html
<form action="proses.php" method="post">
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
            <input id="jk_l" type="radio" name="kelamin" value="L"><label for="jk_l">Laki-laki</label>
            <input id="jk_p" type="radio" name="kelamin" value="P"><label for="jk_p">Perempuan</label>
        </p>
        <p><input type="submit" value="Login"></p>
    </fieldset>
</form>
```

**Penjelasan:**  
Form digunakan untuk **mengambil input dari pengguna**.  
Elemen penting:
- `<input>` untuk input teks/radio/button.  
- `<textarea>` untuk input banyak baris.  
- `<fieldset>` dan `<legend>` untuk mengelompokkan form.

![foto](https://github.com/Manueljds2311105/foto/blob/be06d5b3607d4ed0f94b34d81db3909ab4a13b0e/HTML%20Lanjutan%20-%20Google%20Chrome%2010_8_2025%2011_08_56%20AM.png)

---

## 8. Menambahkan CSS pada Form

```html
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

**Penjelasan:**  
- CSS digunakan untuk **memperindah tampilan form**.  
- Label diatur lebar tetap agar sejajar.  
- Tombol submit diberi warna dan padding agar menarik.  

![foto](https://github.com/Manueljds2311105/foto/blob/be06d5b3607d4ed0f94b34d81db3909ab4a13b0e/HTML%20Lanjutan%20-%20Google%20Chrome%2010_8_2025%2011_10_42%20AM.png)

---

## 9. Tugas Tambahan
Buat form tambahan yang menampilkan **dropdown** menu dan **listbox** multiple selection.

```html
        <p>
          <label for="jurusan">Pilih Jurusan</label>
          <select id="jurusan" name="jurusan">
            <option>Teknik Informatika</option>
            <option>Teknik Industri</option>
            <option>Manajemen</option>
          </select>
        </p>

        <p>
          <label for="hobi">Pilih Hobi:</label>
          <select id="hobi" name="hobi" multiple size="5">
            <option value="membaca">Membaca</option>
            <option value="olahraga">Olahraga</option>
            <option value="musik">Musik</option>
            <option value="traveling">Traveling</option>
            <option value="memasak">Memasak</option>
            <option value="gaming">Gaming</option>
            <option value="fotografi">Fotografi</option>
          </select>
        </p>
```

![foto](https://github.com/Manueljds2311105/foto/blob/f4f59ab8d2ea82961177d394e571462543b9e06b/HTML%20Lanjutan%20-%20Google%20Chrome%2010_8_2025%202_49_11%20PM.png)

---
