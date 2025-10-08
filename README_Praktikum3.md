# 🧩 Praktikum 3: Membuat List, Table, dan Form

**Mata Kuliah:** Pemrograman Web  
**Dosen:** Agung Nugroho, S.Kom., M.Kom.  
**Universitas:** Universitas Pelita Bangsa  
**Nama:** _(Isi dengan nama kamu)_  
**NIM:** _(Isi dengan NIM kamu)_  

---

## 🎯 Tujuan Praktikum
1. Memahami struktur dasar pembuatan **List** di HTML.  
2. Memahami struktur dasar pembuatan **Tabel**.  
3. Memahami tag-tag dasar pembuatan **Form**.  
4. Membuat dokumen HTML yang lebih kompleks.  
5. Menerapkan **CSS** pada List, Table, dan Form.

---

## 🧱 1. Persiapan Dokumen HTML
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

📸 **Screenshot:**  
_(Tambahkan hasil tampilan browser di sini)_

---

## 🔢 2. Membuat Ordered List
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

📘 **Penjelasan:**  
- `<ol>` digunakan untuk membuat daftar terurut.  
- `<li>` adalah elemen item daftar.  
- Atribut `type` dan `start` bisa digunakan untuk mengubah jenis penomoran.  

📸 **Screenshot Ordered List**

---

## 🔘 3. Membuat Unordered List
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

📘 **Penjelasan:**  
- `<ul>` membuat daftar tidak berurutan.  
- Atribut `type` dapat berupa: `disc`, `circle`, `square`.  

📸 **Screenshot Unordered List**

---

## 📄 4. Membuat Description List
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

📘 **Penjelasan:**  
- `<dl>` mendefinisikan daftar deskripsi.  
- `<dt>` adalah istilah (judul).  
- `<dd>` adalah deskripsi dari istilah tersebut.  

📸 **Screenshot Description List**

---

## 📊 5. Membuat Tabel
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

📘 **Penjelasan:**  
- `<table>` membuat tabel.  
- `<thead>` untuk kepala tabel.  
- `<tbody>` untuk isi tabel.  
- `<tr>` membuat baris, `<th>` untuk judul kolom, `<td>` untuk isi data.  

📸 **Screenshot Tabel**

---

## 🧩 6. Menggabungkan Sel (Rowspan & Colspan)

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

📘 **Penjelasan:**  
- `rowspan` digunakan untuk menggabungkan sel secara **vertikal**.  
- `colspan` digunakan untuk menggabungkan sel secara **horizontal**.  

📸 **Screenshot Penggabungan Sel**

---

## 🧾 7. Membuat Form
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

📘 **Penjelasan:**  
Form digunakan untuk **mengambil input dari pengguna**.  
Elemen penting:
- `<input>` untuk input teks/radio/button.  
- `<textarea>` untuk input banyak baris.  
- `<fieldset>` dan `<legend>` untuk mengelompokkan form.

📸 **Screenshot Form**

---

## 🎨 8. Menambahkan CSS pada Form

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

📘 **Penjelasan:**  
- CSS digunakan untuk **memperindah tampilan form**.  
- Label diatur lebar tetap agar sejajar.  
- Tombol submit diberi warna dan padding agar menarik.  

📸 **Screenshot Form dengan CSS**

---

## 🧠 9. Tugas Tambahan
Buat form tambahan yang menampilkan **dropdown menu** dan **listbox multiple selection**.

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
    <label for="hobi">Hobi</label>
    <select id="hobi" name="hobi" multiple>
        <option>Membaca</option>
        <option>Olahraga</option>
        <option>Musik</option>
    </select>
</p>
```

📸 **Screenshot Dropdown & Listbox**

---

## ✅ Hasil Akhir
- Terdapat **tiga file utama:**
  1. `lab3_list.html`
  2. `lab3_tabel.html`
  3. `lab3_form.html`

- Semua file telah divalidasi menggunakan [W3C Validator](http://validator.w3.org/).  
- CSS telah diterapkan untuk mempercantik tampilan form.

---

## 💾 Repository GitHub
Upload seluruh hasil ke repository dengan nama:  
> **`Lab3Web`**

Struktur folder:
```
Lab3Web/
├── lab3_list.html
├── lab3_tabel.html
├── lab3_form.html
└── README.md
```

Commit hasil pekerjaan dan kirim URL repository ke e-learning.

---

✍️ **Dibuat oleh:**  
_(Nama & NIM kamu)_  
_Pemrograman Web - Universitas Pelita Bangsa_
