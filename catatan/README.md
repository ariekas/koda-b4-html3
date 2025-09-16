# HTML dan CSS

## HTML

Hypertext Markup Language.

Basic structure html

```html
<!DOCTYPE html>
<html>
  <head>
   <!-- Metadata -->
  </head>
  <body>
    <!-- content -->
  </body>
</html>
```

### Metadata
```html
 <!-- mengatur judul halaman -->
<title>Judul Halamaan</title>
 <!-- memberikan deskripsi singkat -->
<meta name="deskripsi" content="deskripsi halaman disni">

 <!-- dukungan responsif dasar halaman -->
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<!-- informasi encoding -->
 <meta charset="UTF-8">
```

1. Tag Formatting
   Tag yang berguna untuk mengubah tampilan atau format teks

- strong
- em
- i
- pre
- b
- u

2. Tag Layouting
   Tag yang berguna untuk menyusun struktur halaman website

- header
- nav
- main
- section
- article
- footer
- div

3. Form
   Form digunakan untuk mendapatkan sebuah data dari inputan user

### Form terkait teks

elememt elememt yang berhubungan langsung dengan input berbasis teks, contoh nya:

```html
<input type="text"> → Untuk input teks biasa

<input type="email"> → Input teks tapi divalidasi harus dalam format email.

<input type="password"> → Input teks yang tersembunyi

<input type="url"> → Input teks tapi divalidasi dalam format URL.

<input type="tel"> → Input teks tapi diformat sebagai nomor telepon.

<textarea> → Untuk input teks panjang

<input type="search"> → Mirip text, tapi dioptimalkan untuk kolom pencarian.
```

Standart penulisan form di html:

```html
<form action="/submit" method="POST">
  <fieldset>
    <legend>Form Registrasi</legend>

    <label for="username">Username:</label>
    <input type="text" id="username" name="username" required /><br /><br />

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required /><br /><br />

    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required /><br /><br />

    <label for="hobby">Hobby:</label>
    <input type="checkbox" name="hobby" value="reading" /> Reading
    <input type="checkbox" name="hobby" value="coding" /> Coding
    <input type="checkbox" name="hobby" value="gaming" /> Gaming <br /><br />

    <label for="country">Country:</label>
    <select id="country" name="country">
      <option value="id">Indonesia</option>
      <option value="us">USA</option></select
    ><br /><br />

    <button type="submit">Register</button>
  </fieldset>
</form>
```

4. Table
   Tag html yang berguna untuk menampilkan data dalam bentuk col dan row atau dalam bentuk table

contoh tag nya:

```html
<table>
  → wadah utama tabel.

  <tr>
    → table row (baris tabel).

    <td>→ table data (isi sel).</td>

    <th>→ table header (judul kolom, teks biasanya tebal & rata tengah).</th>
  </tr>
</table>
```

Struktur Semantik Lengkap :

```html
<caption>
  → judul tabel (ditampilkan di atas tabel).

  <thead>
    → bagian kepala tabel (judul kolom).
  </thead>

  <tbody>
    → isi utama tabel (baris data).
  </tbody>
</caption>
```

contoh pengunaan nya :

```html
<table border="1">
  <caption>
    Daftar Nilai Mahasiswa
  </caption>
  <thead>
    <tr>
      <th>Nama</th>
      <th>Mata Kuliah</th>
      <th>Nilai</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Siti</td>
      <td>Matematika</td>
      <td>90</td>
    </tr>
    <tr>
      <td>Andi</td>
      <td>Fisika</td>
      <td>85</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="2">Rata-rata</td>
      <td>87.5</td>
    </tr>
  </tfoot>
</table>
```

5. List
   List digunakan untuk menampilkan data dalam bentuk list

- Unordered List (ul)

```html
<ul>
  <li>Apel</li>
  <li>Pisang</li>
  <li>Mangga</li>
</ul>
```

- Ordered List (ol)

```html
<ol>
  <li>Bangun tidur</li>
  <li>Sarapan</li>
  <li>Berangkat kerja</li>
</ol>
```

- Description List (dl)

```html
<dl>
  <dt>HTML</dt>
  <dd>Bahasa markup untuk membuat halaman web.</dd>
  <dt>CSS</dt>
  <dd>Bahasa untuk mendesain tampilan web.</dd>
</dl>
```

- Nested List
  List yang digunakan di dalam list lain

```html
<ul>
  <li>
    Buah
    <ul>
      <li>Apel</li>
      <li>Pisang</li>
    </ul>
  </li>
  <li>
    Sayur
    <ul>
      <li>Bayam</li>
      <li>Wortel</li>
    </ul>
  </li>
</ul>
```

## CSS
