# Lab4Web

## 1. Buat Dokumen HTML Dengan Nama File `Lab4Web`

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/a3d40204-703a-4e51-a85e-f2a7f1fdf01d)

## 2. Membuat Box Element

Tambahkan kode untuk membuat box element dengan tag div seperti berikut ini:

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/00300fcf-2bea-4f37-a381-a03cb9afe783)

## 3. CSS Float Property

Tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut ini:

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/30425452-7adc-4ee1-8acd-1d7f8ce69630)

### OUTPUT:

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/9b3aed9b-3f25-47b7-a5e9-8f5c67107559)

## 4. Mengatur Clearfix Element

Ketika menggunakan clearfix, biasanya menambahkannya sebagai kelas pada elemen yang mengandung floating, dan dengan cara ini Anda menginstruksikan browser untuk "membersihkan" elemen tersebut sehingga elemen-elemen setelahnya akan diposisikan dengan benar. Ini sering digunakan dalam desain web untuk menghindari masalah tumpukan floating (float stacking) yang dapat merusak tata letak halaman.

- Menambahkan element div lainnya setelah div3 seperti berikut ini:
  
![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/3599aac6-c3ed-43f1-86a1-fa056bdcd7d7)

- Kemudian, atur property clear pada CSS seperti berikut ini:

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/036c9c7e-e7c4-45f2-8558-7aee285f2907)

### OUTPUT

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/56508ad0-7bd7-46e3-a87b-393418f1a977)

# MEMBUAT LAYOUT SEDERHANA

## 1. Buat folder HTML baru dengan nama `lab4_layout` dan file CSS `style.css`

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/d820483a-8b0a-4969-a169-2bf4d05f2d7f)

## 2. Tuliskan Code berikut ini:

### CODE HTML
```
<header>
        <h1>Layout Sederhana</h1>
      </header>
      <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Kontak</a>
      </nav>
      <section iid="hero"></section>
      <section id="wrapper">
        <section id="main"></section>
        <aside id="sidebar"></aside>
      </section>
      <footer>
        <p>&copy; 2021 - Universitas Pelita Bangsa</p>
      </footer>
```

### OUTPUT

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/05d28349-f15b-48f0-95d7-54a914e608e5)

### CODE CSS

```
/* import google font */
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap");

/* Reset CSS */
* {
  margin: 0;
  padding: 0;
}
body {
  line-height: 1;
  font-size: 100%;
  font-family: "Open Sans", sans-serif;
  color: #5a5a5a;
}

#container {
  width: 980px;
  margin: 0 auto;
  box-shadow: 0 0 1em #cccccc;
}

/* header */
header {
  padding: 20 px;
}

header h1 {
  margin: 20px 10px;
  color: #b5b5b5;
}
```

### OUTPUT

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/b8606280-4530-4e78-a43a-b7051550a7fa)

## 2. Membuat Navigasi

### CODE CSS:

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

### OUTPUT:

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/b23aba3c-566e-439b-8562-71b103fde886)

## 3. Membuat Hero Panel

### CODE HTML:

```
<section id="hero">
        <h1>Hello World!</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
          lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin
          in leo fringilla, vestibulum mi porta, faucibus felis. Integer
          pharetra est nunc, nec pretium nunc pretium ac.
        </p>
        <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
      </section>
```

### CODE CSS:

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

### OUTPUT:

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/bb85dc14-a3d7-442f-a74b-9caa25212674)

## 4. Mengatur Layout Main Dan SiDebar

```
/* main content */
#wrapper {
  margin: 0;
}
#main {
  float: right;
  width: 640px;
  padding: 20px;
}
/* sidebar area */
#sidebar {
  float: right;
  width: 260px;
  padding: 20px;
}
```

## 5. Membuat Sidebar Widget

### CODE HTML:

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
          <p>
            Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
            arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis.
            Integer pharetra est nunc, nec pretium nunc pretium ac.
          </p>
        </div>
      </aside>
```

### CODE CSS:

```
/* widget */
.widget-box {
  border: 1px solid #eee;
  margin-bottom: 20px;
}
.widget-box .title {
  padding: 10px 16px;
  background-color: #428bca;
  color: #fff;
}
.widget-box ul {
  list-style-type: none;
}
.widget-box li {
  border-bottom: 1px solid #eee;
}
.widget-box li a {
  padding: 10px 16px;
  color: #333;
  display: block;
  text-decoration: none;
}
.widget-box li:hover a {
  background-color: #eee;
}
.widget-box p {
  padding: 15px;
  line-height: 25px;
}
```

### OUTPUT:

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/1a861eed-499d-438d-837c-1b059fa046a7)

## 6. Mengatur Footer

### CODE CSS:

```
/* footer */
footer {
clear:both;
background-color:#1d1d1d;
padding:20px;
color:#eee;
}
```

### OUTPUT:

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/258b57fd-7608-48f1-8766-e77e61d4e892)

## 7. Menambahkan Elemen Lainnya

### CODE HTML:

```
 <section id="main">
        <div class="row">
          <div class="box">
            <img
              src="https://dummyimage.com/120/db7d25/fff.png"
              alt=""
              class="image-circle"
            />
            <h3>Heading</h3>
            <p>
              Donec sed odio dui. Etiam porta sem malesuada magna mollis
              euismod.
            </p>
            <a href="#" class="btn btn-default">View detail</a>
          </div>
          <div class="box">
            <img
              src="https://dummyimage.com/120/3e73e6/fff.png"
              alt=""
              class="image-circle"
            />
            <h3>Heading</h3>
            <p>
              Donec sed odio dui. Etiam porta sem malesuada magna mollis
              euismod.
            </p>
            <a href="#" class="btn btn-default">View detail</a>
          </div>
          <div class="box">
            <img
              src="https://dummyimage.com/120/71e6d4/fff.png"
              alt=""
              class="image-circle"
            />
            <h3>Heading</h3>
            <p>
              Donec sed odio dui. Etiam porta sem malesuada magna mollis
              euismod.
            </p>
            <a href="#" class="btn btn-default">View detail</a>
          </div>
        </div>
      </section>
```

### CODE CSS:

```
/* box */
.box {
  display: block;
  float: left;
  width: 33.333333%;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  padding: 0 10px;
  text-align: center;
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
.row:after,
.row:before,
.entry:after,
.entry:before {
  content: "";
  display: table;
}
.row:after,
.entry:after {
  clear: both;
}
```

### OUTPUT:

![image](https://github.com/Aliyahasmarani/Lab4Web/assets/115197672/a0a35cbc-d301-4187-b79c-a3ab9ae8dfc9)


















