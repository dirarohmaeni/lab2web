# Nama: Dira Rohmaeni
# NIM: 312410465
# Kelas: TI.24.A5

1. Buat file baru dengan nama **lab2_css_dasar.html**

2. Membuat dokumenHTML
<img src="/code 1.png" width="500">
Buka Browser untuk melihat hasilnya
<img src="/hasil 1.png" width="500">

3. Kemudian tambahkan deklarasi CSS internal
<img src="/code 2.png" width="500">
refresh untuk melihat hasilnya
<img src="/hasil 2.png" width="500">

4. menambahkan inline CSS 
Kemudian tambahkan deklarasi inline CSS pada tag <p>
<img src="/code 3.png" width="500">
refresh untuk melihat hasilnya
<img src="/hasil 3.png" width="500">

5. Membuat CSS Eksternal
Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS
<img src="/code 4.png" width="500">
refresh untuk melihat hasilnya
<img src="/hasil 4.png" width="500">

Kemudian tambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian <head>
<img src="/menambahkan tag link.png" width="500">
refresh untuk melihat hasilnya
<img src="/hasil menambahkan tag link.png" width="500">

6. Menambahkan CSS Selector
Kemudian menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css
<img src="/code 5.png" width="500">
refresh untuk melihat hasilnya
<img src="/hasil 5.png" width="500">

### Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )

### Jawaban:
1. 
body {


font-family: 'Open Sans', sans-serif;

  
  background: #f9f9f9;
  
  
  margin: 0;
}


h1 {

  
  font-size: 28px;
  
  
  color: #5c6bc0;
  
  
  text-align: center;
  
  
  padding: 20px 10px;
  
  
  text-shadow: 1px 1px 3px rgba(0,0,0,0.2);
  
  
  letter-spacing: 2px;


}


Eksperimen ini menambahkan warna pastel, shadow, letter-spacing, padding sehingga tampilannya lebih aesthetic.


2. 


h1 {

  
  color: #5c6bc0;


}


#intro h1 {

  
  color: #f68084;


}


Jadi h1 {} → berlaku untuk semua <h1>.


intro h1 {} → khusus <h1> di dalam elemen dengan id="intro".


3. Urutan prioritas: Inline > Internal > Eksternal


<head>

  
  <!-- Eksternal -->
  
  
  <link rel="stylesheet" href="style_eksternal.css">


  <!-- Internal -->

  
  <style>
  
    
    p {
    
      
      color: orange;
    
    
    }
  
  
  </style>


</head>


<body>

  
  <p style="color: #36ad36;">Teks ini warna hijau</p>


</body>


Walaupun eksternal p { color: blue; } dan internal p { color: orange; }, hasil akhirnya tetap hijau karena inline CSS punya prioritas tertinggi.


4. 
.text-paragraf {

  
  color: #5c6bc0;


}


#paragraf-1 {

  
  color: #f68084;


}


Jadi teks berwarna pink pastel karena ID lebih kuat dibanding class.
