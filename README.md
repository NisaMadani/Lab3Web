# Lab3Web

Nama: Nisa Madani
NIM: 311910754
Kelas: 19.TI.B1

Persiapan membuat dokumen HTML dengan nama file lab3_list.html, setelah itu membuat ordered list seperti pada gambar di bawah ini

![1](https://user-images.githubusercontent.com/81978276/114298759-20e38480-9ae2-11eb-967e-8f0ec5c6d070.png)

hasil yang kita dapatkan ketika buka di browser adalah sebagai berikut:

![1b](https://user-images.githubusercontent.com/81978276/114298761-22ad4800-9ae2-11eb-9a23-3c504056d8ba.png)

Kemudian tambakan kode untuk membuat Unordered List, setelah deklarasi ordered list pada 
section unordered-list

![2](https://user-images.githubusercontent.com/81978276/114298762-24770b80-9ae2-11eb-9df9-729f1c738224.png)

Kita buka browser yang telah kita buka, lalu refresh. Tampilannya akan berubah seperti di bawah ini

![2a](https://user-images.githubusercontent.com/81978276/114298764-24770b80-9ae2-11eb-8600-da03d706c1c3.png)

Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list, dengan kode seperti di bawah ini

![3](https://user-images.githubusercontent.com/81978276/114298765-250fa200-9ae2-11eb-923d-d84b06d3d4a5.png)

refresh kembali browser, agar tampilan baru muncul

![3a](https://user-images.githubusercontent.com/81978276/114298766-25a83880-9ae2-11eb-9223-66a3d4f51b3e.png)

Membuat Tabel
Buat file baru dengan nama lab3_tabel.html, dilanjutkan dengan menambahkan kode untuk membuat tabel sederhana seperti berikut:

![4](https://user-images.githubusercontent.com/81978276/114298767-2640cf00-9ae2-11eb-94f7-a09edf4d007f.png)

Buka di browser, maka tampilan akan menjadi seperti di bawah ini. 

![4a](https://user-images.githubusercontent.com/81978276/114298768-26d96580-9ae2-11eb-958a-488d774cc3aa.png)

  Mengatur Margin dan Padding
Untuk mengatur margin dan padding pada cel data, tambahkan atribut cellpadding dan 
cellspacing pada tag table. yang awalnya cellpadding bernilai 4, hasil tampilan tabel di browser space antara tulisan dengan border terlalu dekat. untuk merubah agar lebih lebar, maka cellpadding kita rubah jadi bernilai 6.

<table border="1" cellpadding="6" cellspacing="0">
  
berikut tampilan setelah di refresh

![5a](https://user-images.githubusercontent.com/81978276/114298770-280a9280-9ae2-11eb-9bfc-ed6fd93c4292.png)

Menggabungkan Sel Data
Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk 
menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara 
horizontal). hasil akhir kode di tab tabel seperti dibawah ini:

![5](https://user-images.githubusercontent.com/81978276/114298769-2771fc00-9ae2-11eb-9713-cb07a98dfecd.png)

hasil di browser setelah kita refresh, seperti di bawah ini:

![5b](https://user-images.githubusercontent.com/81978276/114298771-28a32900-9ae2-11eb-8d2d-a27f82734203.png)

Membuat Form
Buat file baru dengan nama lab3_form.html . Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut

![6](https://user-images.githubusercontent.com/81978276/114298772-2f31a080-9ae2-11eb-9f8a-c5b907033cac.png)

hasilnya adalah sebagai berikut:

![6a](https://user-images.githubusercontent.com/81978276/114298774-2fca3700-9ae2-11eb-956b-497490710970.png)

Menabahkan Style pada Form
Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.

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

kode keseluruhan seperti dibawah ini:

![7](https://user-images.githubusercontent.com/81978276/114298775-3062cd80-9ae2-11eb-803f-737a0f9358e2.png)

Tampilan yang dapat kita lihat di browser seperti berikut:

![7a](https://user-images.githubusercontent.com/81978276/114298776-30fb6400-9ae2-11eb-9334-58246f6d08b3.png)

Pertanyaan dan Tugas
1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.
jawaban: 

A. DROPDOWN
Kita mulai dengan membuat wrapper(pembungkus) div dan kita akan memberikan class menu-wrap.

<!doctype html>
 
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Judul Halaman Saya</title>
  </head>
<body>
  <div class="menu-wrap">

  </div>
</body>
</html>

Didalam wrapper kita masukkan daftar link yang ingin kita tampilkan, daftar link tersebut kita bungkus dengan tag <ul> dan tag <li>:
	
  <ul>
		<li><a href="Profil.html">Profil</a></li>
		<li><a href="Daftar Buku.html">Daftar Buku</a></li>
		<li><a href="kontak.html">Kontak Kami</a>
			<ul>
				<li><a href="alamat.html">Alamat Kami</a></li>
				<li><a href="kebijakan.html">Kebijakan</a></li>
			</ul>
		</li>
	</ul>
  
  Karena kita akan menggunakan eksternal CSS, maka tambahkan skrip berikut dalam tag head:
  
   <link rel="stylesheet" type="text/css" href="style.css" media="all" />
   
   Sehingga skrip akhir kita menjadi seperti ini:
   
![dropdown 1](https://user-images.githubusercontent.com/81978276/114298777-3193fa80-9ae2-11eb-9990-613054fcae67.png)

Setelah kita menyelesaikan pembuatan file HTML, selanjutnya dalam membuat menu dropdown kita akan melengkapinya dengan file CSS. Buat file baru dan simpan sebagai “style.css”, dalam file tersebut mulai ketikkan skrip css berikut:

![dropdown 2](https://user-images.githubusercontent.com/81978276/114298780-35c01800-9ae2-11eb-915b-ffc7b0c76f2a.png)

![dropdown 3](https://user-images.githubusercontent.com/81978276/114298781-36f14500-9ae2-11eb-8cc0-c12640d3bbb5.png)

maka tampilan yang akan kita peroleh seperti berikut

![dropdown 4](https://user-images.githubusercontent.com/81978276/114298782-3789db80-9ae2-11eb-88f8-1768d48150e8.png)

![dropdown 5](https://user-images.githubusercontent.com/81978276/114298783-38bb0880-9ae2-11eb-84ba-28f9416453c8.png)

B. LISTBOX
List Box pada web HTML prisipnya sama dengan combo box, hanya tidak terdapat drop down button. Semua item pilihan langsung
ditampilkan dalam box sekaligus. Perintahnya juga sama dengan combo box, perbedaannya adalah adalah adanya atribut size=”n”
pada tag < select name=”namakomponen”> dengan n adalah jumlah item yang akan ditampilkan.

![listbox 1](https://user-images.githubusercontent.com/81978276/114298784-39539f00-9ae2-11eb-8a92-5e60cb1d4282.png)

Tampilan yang akan muncul seperti di bawah ini:

![listbox 2](https://user-images.githubusercontent.com/81978276/114298787-39ec3580-9ae2-11eb-9f18-14a4915d040e.png)
