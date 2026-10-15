# Praktikum 4: CSS Layout (Box Element & Layout Sederhana) - Pemrograman Web
Repository ini dibuat untuk menyelesaikan tugas Praktikum 4 Pemrograman Web.

## Identitas Mahasiswa

| Keterangan      | Data                 |
| --------------- | -------------------- |
| **Nama**        | Davarel Radivan Anwar|
| **Kelas**       | I251D                |
| **NIM**         | 312510384            |
| **Mata Kuliah** | Pemrograman Web      |
| **Dosen**       | Agung Nugroho, S.Kom., M.Kom. |

### Tujuan Praktikum

Mahasiswa mampu memahami konsep box element pada CSS (float dan clearfix).

Mahasiswa mampu membuat layout website sederhana menggunakan semantic element HTML5.

Mahasiswa mampu mengatur navigasi, hero panel, main content, sidebar, dan footer menggunakan CSS.

Mahasiswa mampu membuat halaman tambahan (About dan Kontak) dengan layout yang konsisten.

---

## Struktur Folder Proyek

```
Lab4Web/
├── Lab4_Layout/
│   ├── Lab4_Layout.html
│   ├── about.html
│   ├── kontak.html
│   └── style.css
├── Lab4web/
│   └── Lab4_box.html
└── README.md
```

<!-- Ganti dengan screenshot struktur folder -->

<img width="191" height="279" alt="image" src="https://github.com/user-attachments/assets/d816badb-1c07-4a8d-9a3f-8668b4719ae7" />


---

## Langkah-langkah Praktikum

### 1. Membuat Box Element (`Lab4_box.html`)

Langkah pertama adalah menyiapkan dokumen HTML dasar dengan nama `Lab4_box.html` yang berisi `<header>` dengan judul "Box Element".

<img width="658" height="370" alt="image" src="https://github.com/user-attachments/assets/6bc1d99a-9d28-4d56-96d2-46aeb1c99598" />


Kemudian di dalam `<body>` ditambahkan `<section>` yang berisi empat buah `<div>` dengan class `div1` sampai `div4`.

<img width="488" height="316" alt="image" src="https://github.com/user-attachments/assets/d9d107fa-4ba8-4f5f-85ad-6b02b1c4a59b" />



#### CSS Float Property

Pada bagian `<head>` ditambahkan CSS internal untuk membuat float element:

- Semua `div` diberi `float: left` dan `padding: 10px`.
- `.div1` berwarna merah, `.div2` kuning, `.div3` hijau.
- `.div4` berwarna biru dengan `clear: left` dan `float: none` (clearfix) agar tampil di baris baru.

<img width="453" height="594" alt="image" src="https://github.com/user-attachments/assets/71dc9520-04c8-4f2f-b153-9d7063f9cf20" />



Hasil di browser: Div1, Div2, dan Div3 tampil sejajar ke samping, sedangkan Div4 berada di bawahnya dengan lebar penuh.

<img width="748" height="136" alt="image" src="https://github.com/user-attachments/assets/f1377c5c-2a39-4c6e-8755-17f3c4bd6aac" />


---

### 2. Membuat Layout Sederhana (`Lab4_Layout.html`)

Membuat kerangka layout menggunakan semantic element. Dokumen ini menghubungkan file `style.css` dan memiliki `<div id="container">` sebagai pembungkus utama.

<img width="975" height="375" alt="image" src="https://github.com/user-attachments/assets/75807522-b7c2-499f-ac88-50af3e1f6acb" />



Di dalam container ditambahkan elemen `<header>`, `<nav>` (Home, Artikel, About, Kontak), `<section id="hero">`, `<section id="wrapper">` (berisi `<section id="main">` dan `<aside id="sidebar">`), serta `<footer>`.

<img width="652" height="522" alt="image" src="https://github.com/user-attachments/assets/85f24c66-c4c5-4ccd-9253-e15e897264d8" />

<img width="499" height="332" alt="image" src="https://github.com/user-attachments/assets/db698d27-dc9f-47be-8105-1871dd4b0b60" />



Hasil sebelum diberi CSS:

<img width="313" height="172" alt="image" src="https://github.com/user-attachments/assets/7173647b-bb9d-4228-8132-a09613d26713" />


---

### 3. Menambahkan CSS Layout (`style.css`)

CSS ditambahkan untuk membuat tampilan dasar layout, meliputi:

- `@import` Google Font **Open Sans** dan **Open Sans Condensed**.
- Reset CSS (`margin: 0; padding: 0`).
- Pengaturan `body` (font-size, font-family, warna teks).
- `#container` dengan lebar `980px`, rata tengah (`margin: 0 auto`), dan `box-shadow`.
- Pengaturan `header` dan `header h1`.

<img width="905" height="474" alt="image" src="https://github.com/user-attachments/assets/4914cfab-a9ce-4a82-bbc5-924156155353" />


Hasil di browser:

<img width="913" height="163" alt="image" src="https://github.com/user-attachments/assets/2628705d-d3cf-4011-8a3e-5eafb5d9ae0a" />


---

### 4. Mengatur Navigasi

CSS navigasi dibuat dengan ketentuan:

- `nav` memiliki background biru (`#1f5faa`).
- Link `nav a` ditampilkan `inline-block`, berwarna putih, tebal, tanpa garis bawah.
- `nav a.active` dan `nav a:hover` memiliki background `#2b83ea`.

<img width="416" height="559" alt="image" src="https://github.com/user-attachments/assets/2c13c572-60a3-41e7-86cf-d575f6cfac21" />


<img width="975" height="184" alt="image" src="https://github.com/user-attachments/assets/d68b383b-2f86-47f9-be1d-0d2b786a49e8" />


---

### 5. Membuat Hero Panel

Menambahkan kode HTML pada `<section id="hero">` berisi judul, paragraf, dan tombol "Learn more", lalu diberi style: background abu-abu (`#e4e4e5`), padding, serta pengaturan ukuran font `h1` dan `p`.

<img width="650" height="298" alt="image" src="https://github.com/user-attachments/assets/6bf2fee6-91f9-47b5-978a-f12943d330b6" />

<img width="450" height="558" alt="image" src="https://github.com/user-attachments/assets/82382406-03d6-48a2-bf79-25059c93ae28" />


<img width="755" height="402" alt="image" src="https://github.com/user-attachments/assets/1f7ea10a-13ea-4b68-9450-4914916c017a" />


---

### 6. Menambahkan CSS Float untuk Main Content dan Sidebar

- `#main` dan `#sidebar` menggunakan `float: left`.
- Lebar `#main` = `640px`, lebar `#sidebar` = `260px`, keduanya dengan `padding: 20px`.
- Sidebar berisi dua `widget-box` (daftar link dan teks) yang diberi style border, title berwarna biru (`#428bca`), list tanpa bullet, dan efek hover.

<img width="478" height="489" alt="image" src="https://github.com/user-attachments/assets/b30d0d5c-e5b6-4c1e-83e1-f2ee78afdd29" />


<img width="475" height="409" alt="image" src="https://github.com/user-attachments/assets/3ecb609a-f373-48bf-8517-1680c8fb2c67" />


<img width="322" height="586" alt="image" src="https://github.com/user-attachments/assets/2e6ac3ee-1120-4b7d-ba81-79a0f6363418" />

<img width="1027" height="547" alt="image" src="https://github.com/user-attachments/assets/11c60cce-cb81-47c1-9a63-de5f809c09c2" />


---

### 7. Mengubah Tampilan Footer

Footer diberi style background gelap dengan teks putih agar terlihat berbeda dari konten utama.

<img width="758" height="302" alt="image" src="https://github.com/user-attachments/assets/fd583d35-27cb-4e9c-b6ca-81b7e9eac23b" />


---

### 8. Menambahkan Elemen Lain pada Main Content

Menambahkan `div.row` yang berisi tiga `div.box`. Masing-masing box memiliki gambar, heading, paragraf, dan tombol "View detail". CSS yang digunakan:

- `.box` dengan `float: left`, `width: 33.333333%`, `box-sizing: border-box`, dan `text-align: center`.
- `.image-circle` dengan `border-radius: 50%` agar gambar berbentuk lingkaran.
- `.row` dengan margin negatif dan clearfix (`:before` dan `:after` dengan `display: table` dan `clear: both`).

<img width="555" height="802" alt="image" src="https://github.com/user-attachments/assets/bc5260a1-48b5-48b9-8f2b-e24f1b241703" />

<img width="436" height="592" alt="image" src="https://github.com/user-attachments/assets/ec1251e9-2680-4094-a59f-0612faa6a3d1" />
<img width="492" height="716" alt="image" src="https://github.com/user-attachments/assets/383eea6a-f644-451b-8ff0-efb7b3540600" />
<img width="975" height="520" alt="image" src="https://github.com/user-attachments/assets/0f46e8be-6cb3-4be8-ae1d-9bf7156e754d" />


---

### 9. Membuat Content Artikel

Menambahkan dua `<article class="entry">` yang dipisah dengan `<hr class="divider">`. Artikel pertama memiliki gambar di kiri, sedangkan artikel kedua memakai class `right-img` sehingga gambar berada di kanan.

CSS `.entry`:
- `margin: 15px 0`, `h2` dengan `margin-bottom: 20px`, dan `p` dengan `line-height: 25px`.
- `.entry img` menggunakan `float: left`, `border-radius: 5px`, dan `margin-right: 15px`.
- `.entry .right-img` menggunakan `float: right` dengan margin kiri `15px`.

<img width="578" height="248" alt="image" src="https://github.com/user-attachments/assets/19ff8570-955d-47e1-aa65-10052dccbc5c" />


<img width="244" height="376" alt="image" src="https://github.com/user-attachments/assets/25ac8edb-f782-4d35-8a59-0a75fc69fb66" />


<img width="469" height="316" alt="image" src="https://github.com/user-attachments/assets/cce429ae-882d-4f25-9c75-d7394e306fa7" />


---

## Pertanyaan dan Tugas

### 1. Menambahkan Menu About (`about.html`)

Membuat halaman About dengan layout yang sama (header, nav, hero, main, footer). Halaman ini berisi bagian **Tentang Saya** (hero), **Deskripsi Diri**, dan **Portfolio** (Website Layout Sederhana, Desain UI/UX, dan Project Pemrograman). Menu "About" diberi `class="active"`.

<img width="689" height="1350" alt="image" src="https://github.com/user-attachments/assets/430d0fbc-c54d-4882-9400-e3187688c6df" />

<img width="975" height="462" alt="image" src="https://github.com/user-attachments/assets/99f75a6e-5994-48a8-9475-7506e6c0af84" />


### 2. Menambahkan Menu Kontak (`kontak.html`)

Membuat halaman Kontak yang berisi **Form Contact** dengan field Nama Lengkap, Email, Subjek, dan Pesan (textarea), serta tombol "Kirim Pesan". Semua field menggunakan atribut `required`, dan menu "Kontak" diberi `class="active"`.

<img width="618" height="1350" alt="image" src="https://github.com/user-attachments/assets/fa9ef1b0-f294-49be-a146-ba998e0fcce6" />


<img width="975" height="490" alt="image" src="https://github.com/user-attachments/assets/898b1d3c-70ae-45f3-b313-3400b7c84b2c" />


---

## Kesimpulan

Pada praktikum ini telah dipelajari cara membuat layout website dengan CSS menggunakan properti `float` dan `clear`, penggunaan semantic element HTML5, serta pembuatan komponen seperti navigasi, hero panel, sidebar widget, box, dan artikel. Selain itu juga dibuat halaman About dan Kontak dengan layout yang konsisten.
