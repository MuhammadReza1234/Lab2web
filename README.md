<h1 <p align="center"><b>Praktikum 2</b></p></h1> 

<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Muhammad Reza Maulana</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210303</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A3</td>
  </tr>
</table>

---

## 1. Membuat dokumen HTML

Buatlah dokumen HTML seperti berikut:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
</head>
<body>
    <header>
        <h1>CSS Internal dan <i>Inline </i>CSS</h1>
    </header>
    <nav>
        <a href="lab2_css_dasar.html">CSS Dasar</a>
        <a href="lab2_css_eskternal.html">CSS Eskternal</a>
        <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <!-- CSS ID Selector -->
    <div id="intro">
        <h1>Hello World</h1>
        <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS</p>

        <!-- CSS Class Selector -->
        <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
    </div>
</body>
</html>
```

Kemudian simpan perubahannya dan buka web browser kemudian refresh, berikut hasilnya

![IMG_20231007_233807](https://github.com/MuhammadReza1234/Lab2web/assets/115516607/97c30cde-f703-44de-93b0-12ba0533d788)

---

## 2. Mendeklarasikan CSS Internal

Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.

```html
    <head>
        <title>CSS Dasar</title>
        <style>
            body {
                font-family: 'Open Sans', sans-serif;
            }
    
            header {
                min-height: 80px;
                border-bottom: 1px solid #77ccef;
            }
    
            h1 {
                font-size: 24px;
                color: #0f189f;
                text-align: center;
                padding: 20px 10px;
            }
    
            h1 i {
                color: #6d6a6b;
            }
        </style>
    </header>
```

Kemudian simpan perubahannya dan buka web browser kemudian refresh, berikut hasilnya

![IMG_20231007_233940](https://github.com/MuhammadReza1234/Lab2web/assets/115516607/0db66040-cd26-4e7d-b81f-89a861b71399)

---

## 3. Menambahkan Inline CSS

Kemudian tambahkan deklarasi inline CSS pada tag `<p>` seperti berikut.

```html
<p style="text-align: center; color: #ccd8ef;">
```

Kemudian simpan perubahannya dan buka web browser kemudian refresh, berikut hasilnya

![IMG_20231007_234047](https://github.com/MuhammadReza1234/Lab2web/assets/115516607/76775488-7fa2-449c-8eec-002f884f2afa)

---

## 4. Membuat CSS Eksternal

Buatlah file baru dengan nama **style_eksternal.css** kemudian buatlah deklarasi CSS seperti berikut.

```css
nav {
    background: #20A759;
    color:#fff;
    padding: 10px;
    }
    nav a {
    color: #fff;
    text-decoration: none;
    padding:10px 20px;
    }
    nav .active,
    nav a:hover {
    background: #0B6B3A;
    }
```

Kemudian tambahkan tag `<link>` untuk merujuk file css yang sudah dibuat pada bagian `<head>`

```html
    <head>
        <!-- menyisipkan css eksternal -->
        <link rel="stylesheet" href="style_eksternal.css" type="text/css">
    <head>

```

Kemudian simpan perubahannya dan buka web browser kemudian refresh, berikut hasilnya

![IMG_20231007_234139](https://github.com/MuhammadReza1234/Lab2web/assets/115516607/fcb4d93f-2409-483e-a5f6-635ed8a6cf3c)

---

## 5. Menambahkan CSS Selector

Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file **style_eksternal.css**, tambahkan kode berikut.

```css
 /* ID Selector */
#intro {
    background: #418fb1;
    border: 1px solid #099249;
    min-height: 100px;
    padding: 10px;
    }
    #intro h1 {
    text-align: left;
    border: 0;
    color: #fff;
    }
    /* Class Selector */
    .button {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
    display: inline-block;
    margin: 10px;
    text-decoration: none;
    }
    .btn-primary {
    background: #E42A42;
    }
```

Kemudian simpan perubahannya dan buka web browser kemudian refresh, berikut hasilnya

![IMG_20231007_234241](https://github.com/MuhammadReza1234/Lab2web/assets/115516607/7ac73de4-d346-4ebb-bb17-6a17620410f8)

---

## Menjawab Pertanyaan

<b> 1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini. </br>
Jawab: </b>

```
header
{
    background-image:Url(C:/Users/Asus/Pictures/milik reza/DSC04430.JPG);
    background-position: center center;
    background-size: 630px;
    background-repeat: no-repeat;
    border: 4px solid #000;
}

```

![IMG_20231007_234346](https://github.com/MuhammadReza1234/Lab2web/assets/115516607/248ddac7-d044-460f-beff-ab2a030987e1)

<b> 2. Apa perbedaan pendeklarasian CSS elemen `h1 {...}` dengan `#intro h1 {...}`? berikan penjelasannya! </br>
Jawab: </b>

Kalau `h1 {...}` menggunakan internal dan inline pada penggunaan style nya sedangkan `#intro h1 {...}` menggunakan eksternal css style nya

<b> 3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! </br>
Jawab: </b>

Semuanya akan tampil tergantung penyebutnya contohnya pada gambar no. 1

<b> 4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! `( p id="paragraf-1" class="text-paragraf" )` </br>
Jawab: </b>

Di praktek Hari ini keduanya tampil tapi berbeda

---

<h1 <p align="center"><b>======== Sekian Terima Kasih ==========</b></p></h1>
