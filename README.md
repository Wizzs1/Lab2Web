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

# Praktikum 2
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

## Pertanyaan dan Jawaban
