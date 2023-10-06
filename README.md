<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Wisnu Ikhwansyah Saputra</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210305</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A3</td>
  </tr>
</table>

---

<p align="center"><b>Praktikum 2</b></p>

### membuat dokumen html

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Dasar</title>
    </head>
    <body>
        <header>
            <h1>CSS Internal dan <i>Inline CSS</i></h1>
        </header>
        <nav>
            <a href="lab2_css_dasar.html">CSS Dasar</a>
            <a href="lab2_css_eksternal.html">CSS Eksternal</a>
            <a href="lab1_tag_dasar.html">HTML Dasar</a>
        </nav>
        <!-- CSS ID Selector-->
        <div id="intro">
            <h1>Hello World</h1>
            <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
            Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
            adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML 
        dan CSS.</p>
                <!--CSS Class Selector-->
                <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
        </div>
    </body>
    </html>

<img width="631" alt="image" src="https://github.com/Wizzs1/Lab2Web/assets/110619093/ad5811ed-4aac-40e8-aec5-8f786321b091">

### deklarasikan css internal

        <title>CSS Dasar</title>
    <style>
        body {
            font-family:'Open Sans', sans-serif;
        }
        header {
            min-height: 80px;
            border-bottom:1px solid #77CCEF;
        }
        h1 {
            font-size: 24px;
            color: #0F189F;
            text-align: center;
            padding: 20px 10px;
        }
        h1 i {
            color:#6d6a6b;
        }

<img width="631" alt="Screenshot 2023-10-06 151332" src="https://github.com/Wizzs1/Lab2Web/assets/110619093/7305deb0-3a44-4c8b-8406-e2f2084b9a4b">

### menambahkan inline css

    <p style="text-align: center; color: #ccd8e4;"

<img width="632" alt="image" src="https://github.com/Wizzs1/Lab2Web/assets/110619093/53b6ea79-b317-44d5-ba4d-75992241158d">

### membuat css eksternal

    nav {
    background: #20A759;
    color: #fff;
    padding: 10px;
    }
    nav a {
        color:#fff;
        text-decoration: none;
        padding:10px 20px;
    }
    nav .active
    nav a:hover{
        background: #0B6B3A;
    }

<b>kemudian tambahkan tag ```<link>``` untuk merujuk file cssyang sudah dibuat pada bagian ```<head>```</b>

    <!--menyisipkan css eksternal-->
    <link rel="stylesheet" href="style_ekternal.css" type="text/css">

<img width="632" alt="image" src="https://github.com/Wizzs1/Lab2Web/assets/110619093/64e427d1-f771-4ef2-a7b7-1237a2175334">

### menambahkan css selector

    /*ID Selector */
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

    /* Class Selector*/
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

<img width="631" alt="image" src="https://github.com/Wizzs1/Lab2Web/assets/110619093/c44c680c-c0ba-462e-9fed-ff0a0ae848c1">

## Pertanyaan

<b>1. lakukanLakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.</b>


        <link rel="stylesheet" href="style.css">
    
        <h1 class="title">Wisnu Ikhwansyah Saputra</h1>
        <p class="text">Galva Al Godzali</p>

<img width="463" alt="image" src="https://github.com/Wizzs1/Lab2Web/assets/110619093/9a994481-b99a-4b29-8da6-354b4e8d3453">


Pada contoh ini, terdapat elemen ```<h1>``` dengan class "title dan elemen ```<p>``` dengan class "text". Class tersebut akan digunakan sebagai selector dalam CSS untuk mengubah properti dan nilai. Dalam file CSS (style.css), terdapat aturan CSS yang dideklarasikan untuk class "title" dan "text". Aturan tersebut mengubah properti "color" pada elemen dengan class tersebut. Anda dapat mengubah nilai properti "color" pada file CSS sesuai keinginan Anda untuk melihat perubahan yang terjadi pada judul ```(h1)``` dan paragraf ```(p)``` dalam hal warna teks

    .title {
        color: purple;
    }

    .text {
        font-size: 20px;
    }

<b>contoh output</b>

<img width="633" alt="image" src="https://github.com/Wizzs1/Lab2Web/assets/110619093/1ba5e48c-dd16-43e8-aee5-b6fb6a138645">


<b> 2. Apa perbedaan pendeklarasian CSS elemen ```h1``` {...} dengan #intro ```h1``` {...}? berikan penjelasannya!</b>

    
    <div id="intro">
       <h1 class="title">Wisnu Ikhwansyah Saputra</h1> 
    </div>
    <h1>LILTOTO</h1>

<img width="632" alt="image" src="https://github.com/Wizzs1/Lab2Web/assets/110619093/d777a66b-58b6-43e7-9ea7-cacc71bcccb9">

Pada contoh ini, terdapat elemen ```<h1>``` yang berada di dalam elemen ```<div>``` dengan ID "intro" dan juga elemen ```<h1>``` yang berdiri sendiri tanpa ada elemen lain di dalamnya.

    h1 {
        color: cyan;
    }

    #intro h1 {
        color: aquamarine;
    }

<img width="633" alt="image" src="https://github.com/Wizzs1/Lab2Web/assets/110619093/803d5ef4-ad67-4289-adfc-e56f36d1d7f3">
