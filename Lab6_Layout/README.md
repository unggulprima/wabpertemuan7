# Lab4web

Nama : Syifa Aurellia Rahma

NIM  : 312210009

Kelas : TI.22.A1

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Instruksi Praktikum|[Click Here](#instruksi-praktikum)|
|2|Langkah-langkah Praktikum|[Click Here](#langkah-langkah-praktikum)|
|3|Pertanyaan dan Tugas|[Click Here](#pertanyaan-dan-tugas)|

## Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama Lab3Web
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

## Langkah-langkah praktikum
**1. Membuat Box Element**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
<body>
    <header>
        <h1>Box Element</h1>
        <section>
            <div class="div1">Div 1</div>
            <div class="div2">Div 2</div>
            <div class="div3">Div 3</div>
        </section>
        <style>
            div {
            float:left;
            padding: 10px;
            }
            .div1 {
            background: red;
            }
            .div2 {
            background: yellow;
            }
            .div3 {
            background: green;
            }
            </style>
    </header>
</body>
</html>
```

![2](https://github.com/syifaaurellia/Lab4web/assets/115867244/43a8ef2f-6c96-4843-840a-eeb4bcce6746)


**2. Mengatur Clearfix Element**
> - **Clearfix** digunakan untuk mengatur element setelah float element. Property clear digunakan untuk
mengaturnya.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
<body>
    <header>
        <h1>Box Element</h1>
        <section>
            <div class="div1">Div 1</div>
            <div class="div2">Div 2</div>
            <div class="div3">Div 3</div>
            <div class="div4">Div 4</div>
        </section>
        <style>
            div {
            float:left;
            padding: 10px;
            }
            .div1 {
            background: red;
            }
            .div2 {
            background: yellow;
            }
            .div3 {
            background: green;
            }
            .div4 {
            background-color: blue;
            clear: left;
            float: none;
            }
            </style>
    </header>
</body>
</html>
```

![3](https://github.com/syifaaurellia/Lab4web/assets/115867244/3b99b210-69f0-4683-b9ce-2b733efe9708)

> - Lakukan eksperimen terhadap penggunaan property clear dengan nilai lainnya (left, both, right), dan amati perubahannya.

![5](https://github.com/syifaaurellia/Lab4web/assets/115867244/1cad2f39-edd6-4ae1-966f-5695843bc262)


**3. Membuat Layout Sederhana**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Layout Sederhana</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div id="container">
<header>
  <h1>Layout Sederhana</h1>
</header>
<nav>
  <a href="home.html" class="active">Home</a>
  <a href="artikel.html">Artikel</a>
  <a href="about.html">About</a>
  <a href="kontak.html">Kontak</a>
</nav>
<section id="hero"></section>
<section id="wrapper">
      <section id="main"></section>
      <aside id="sidebar"></aside>
</section>
<footer>
    <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```

![6](https://github.com/syifaaurellia/Lab4web/assets/115867244/48130335-60d8-4fd9-ba8a-bfc3480c3d51)

> - Kemudian tambahkan kode CSS untuk membuat layoutnya :
```
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0
,300;0,700;1,300&display=swap');

/* Reset CSS */
* {
    margin: 0;
    padding: 0;
}
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#5a5a5a;
}
#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}
/* header */
header {
    padding: 20px;
}
header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
```

![7](https://github.com/syifaaurellia/Lab4web/assets/115867244/ed0a5780-d573-4bcc-ac6e-9b929486f6d9)


**4. Membuat Navigasi**
> - Kemudian selanjutnya mengatur navigasi
```
/* navigasi */
nav {
    display: block;
    background-color: #1f5faa;
}
nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}
nav a.active,
nav a:hover {
    background-color: #2b83ea;
}
```

![8](https://github.com/syifaaurellia/Lab4web/assets/115867244/5b6d01de-d852-4877-b6b3-f548e6c84b2f)


**5. Mmebuat Hero Panel**
> - Membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.
```
<section id="hero">
    <h1>Hello World!</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```

```
/* Hero Panel */
#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#hero h1 {
      margin-bottom: 20px;
      font-size: 35px;
}
#hero p {
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
}
```
![11](https://github.com/syifaaurellia/Lab4web/assets/115867244/b196684c-b45d-4b0b-a438-38c14394de52)

**6. Mengatur Layout Main dan Sidebar**
> - Selanjutnya mengatur main content dan sidebar, tambahkan CSS float
```
/* main content */
#wrapper {
    margin: 0;
}
#main {
  float: left;
  width: 640px;
  padding: 20px;
}
/* sidebar area */
#sidebar {
  float: left;
  width: 260px;
  padding: 20px;
}
```

**7. Membuat Sidebar Widget**
> - Kemudian selanjutnya menambahkan element lain dalam sidebar
```
<aside id="sidebar">
    <div class="widget-box">
        <h3 class="title">Widget Header</h3>
        <ul>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
        </ul>
    </div>
    <div class="widget-box">
        <h3 class="title">Widget Text</h3>
        <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
pharetra est nunc, nec pretium nunc pretium ac.</p>
      </div>
</aside>
```
> - Kemudian tambahkan CSS
```
/* widget */
.widget-box {
    border:1px solid #eee;
    margin-bottom:20px;
}
.widget-box .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff;
}
.widget-box ul {
    list-style-type:none;
}
.widget-box li {
    border-bottom:1px solid #eee;
}
.widget-box li a {
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none;
}
.widget-box li:hover a {
    background-color:#eee;
}
.widget-box p {
    padding:15px;
    line-height:25px;
}
```

![13](https://github.com/syifaaurellia/Lab4web/assets/115867244/c2eba812-fa89-45b5-a345-36e28df936cc)



**8. Mengatur Footer**
> - Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer
```
/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
}
```

![12](https://github.com/syifaaurellia/Lab4web/assets/115867244/5f8c345f-2ebd-40c4-a85c-c5e335804ef0)


**9. Menambahkan Elemen lainnya pada Main Content**
```
<section id="main">
    <div class="row">
        <div class="box">
            <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
      </div>
      <div class="box">
          <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
class="image-circle">
          <h3>Heading</h3>
          <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
    <a href="#" class="btn btn-default">View detail</a>
      </div>
      <div class="box">
          <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
        </div>
    </div>
</section>
```
> - Kemudian tambahkan CSS :
```
/* box */
.box {
    display:block;
    float:left;
    width:33.333333%;
    box-sizing:border-box;
    -moz-box-sizing:border-box;
    -webkit-box-sizing:border-box;
    padding:0 10px;
text-align:center;
}
.box h3 {
    margin: 15px 0;
}
.box p {
    line-height: 20px;
    font-size: 14px;
    margin-bottom: 15px;
}
box img {
    border: 0;
    vertical-align: middle;
}
.image-circle {
    border-radius: 50%;
}
.row {
    margin: 0 -10px;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box;
}
.row:after, .row:before,
.entry:after, .entry:before {
    content:'';
    display:table;
}
.row:after,
.entry:after {
    clear:both;
}
```

![13](https://github.com/syifaaurellia/Lab4web/assets/115867244/df6c3f9a-96cb-4af9-be0a-1795f197ac96)


**10. Menambahkan Content Artikel**
> - Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content
```
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
class="right-img">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
```

> - Kemudian tambahkan CSS
```
.divider {
    border:0;
    border-top:1px solid #eeeeee;
    margin:40px 0;
}
/* entry */
.entry {
    margin: 15px 0;
}
.entry h2 {
    margin-bottom: 20px;
}
.entry p {
    line-height: 25px;
}
.entry img {
    float: left;
    border-radius: 5px;
    margin-right: 15px;
}
.entry .right-img {
    float: right;
}
```

![Screenshot (81)](https://github.com/syifaaurellia/Lab4web/assets/115867244/dec4e622-bf82-44d8-8646-cd756442cde8)




**11. Lakukan validasi dokumen HTML dengan mengakses http://validator.w3.org/**

![15](https://github.com/syifaaurellia/Lab4web/assets/115867244/0d8b82d2-433d-48c9-b96d-f8aefe7b9fc1)


![16](https://github.com/syifaaurellia/Lab4web/assets/115867244/554bf716-c1ae-41bb-8f28-98e2d24a78fb)


## Pertanyaan dan Tugas
1. Tambahkan Layout untuk menu `About` => buat single layout yang berisi deskripsi, portfolio, dll
```
<!DOCTYPE html>
<html>
<head>
    <title>About Me</title>
    <style>
        /* Tambahkan CSS sesuai kebutuhan untuk mengatur tampilan layout */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f2f2f2;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        nav {
            background-color: #97b28c;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 10px;
        }
        .container {
            padding: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>About Me</h1>
    </header>
    <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="contact.html">Kontak</a>
    </nav>
    <div class="container">
        <h2>About Me</h2>
        <p>Perkenalkan nama saya <b>Syifa Aurellia Rahma</b>. Saya merupakan mahasiswa Universitas Pelita Bangsa dari fakultas teknik dan program studi <i>Teknik Informatika</i>.
           Saya sedang belajar HTML dasar, seperti tugas yang saat ini saya kerjakan yaitu <b>Membuat Layout Web Sederhana.</b>
           Untuk pada halaman ini saya ditugaskan untuk membuat isi dari menu layout <b>"About"</b></p>
    </div>    
     
    <div class="container">
        <h1>Portofolio</h1>
        <h2>Tentang saya</h2>
        <p>Saya adalah seorang mahasiswa yang minat dengan desain, pengembangan web, dan proyek-proyek sederhana.</p>
    </div>
    <div class="container">
    <h2>Keterampilan</h2>
    <ul>
        <li>HTML dan CSS</li>
        <li>Python</li>
    </ul>
    </div>
</body>
</html>
```


![17](https://github.com/syifaaurellia/Lab4web/assets/115867244/0d53dd2a-2211-40f1-be47-66e5e891562f)


2. Tambahkan layout untuk menu `Contact` => yang berisi form isian: nama, email, message, dll
```
<!DOCTYPE html>
<html>
<head>
    <title>Contact Me</title>
    <style>
        /* Tambahkan CSS sesuai kebutuhan untuk mengatur tampilan layout */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f2f2f2;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        nav {
            background-color: #97b28c;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 10px;
        }
        .container {
            padding: 20px;
            text-align: center;
        }
        form {
            background-color: #fff;
            padding: 20px;
            border-radius: 5px;
            width: 50%;
            margin: 0 auto;
        }
        label {
            display: block;
            margin-bottom: 10px;
        }
        input[type="text"],
        input[type="email"],
        textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        input[type="submit"] {
            background-color: #333;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <h1>Contact Me</h1>
    </header>
    <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="contact.html">Kontak</a>
    </nav>
    <div class="container">
        <form>
            <label for="name">Nama:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Pesan:</label>
            <textarea id="message" name="message" rows="4" required></textarea>
            
            <input type="submit" value="Kirim Pesan">
        </form>
    </div>
</body>
</html>
```


![18](https://github.com/syifaaurellia/Lab4web/assets/115867244/71baaad9-545c-4319-925a-aec0499bc892)



## Finish, Terima Kasih
