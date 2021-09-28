# ferry
Catatan HTML & CSS
- Website : Halaman yang menampilkan informasi melalui teks atau gambar. Website dapat diakses melalui internet dengan menggunakan browser.
- Browser : Sebuah perangkat lunak yang dapat menerjemahkan berkas HTML, CSS, dan Javascript yang di dapat dari server untuk ditampilkan dalam bentuk halaman website.
- HTTP Server : Server berperan pada sebuah website sebagai sebuah software yang dapat menerima transaksi dari HyperText Transfer Protocol.
- DNS Server : Server yang dapat mengubah/mengarahkan website melalui sebuah nama domain.
- Client : Perangkat yang meminta (request) suatu layanan tertentu ke suatu server.
- HTML : Salah satu markup language yang digunakan untuk membuat struktur dan menampilkan konten pada World Wide Web (Website).
- CSS : Bahasa yang digunakan untuk mengatur dan mempercantik tampilan pada website.
- JavaScript : Bahasa pemrograman yang digunakan untuk membantu website menampilkan informasi secara dinamis.
- Text Editor : Sebuah perangkat lunak yang digunakan untuk mengelola plain text. Kode HTML, CSS, dan Javascript dituliskan menggunakan perangkat ini.
- Plain text : Teks yang tidak terformat. Format teks yang digunakan dalam menuliskan berkas HTML, CSS, dan Javascript.
- Rich text : Teks terformat. Format teks yang digunakan ketika kita menulis menggunakan Microsoft Word atau teks editor berbasis WYSIWYG (What You See Is What You Get).
- Element : Sebuah komponen pada HTML yang ditandai dengan tag pembuka dan penutup.

HTML

accesskey

Menentukan tombol shortcut untuk mengaktifkan/memfokuskan pada sebuah element.

class

Menentukan satu atau lebih classname untuk sebuah elemen.

contenteditable

Menentukan konten dari elemen merupakan konten yang dapat diubah atau tidak.

data-*

Digunakan untuk menyimpan sebuah data pribadi khusus ke halaman atau aplikasi.

dir

Menentukan arah teks untuk konten pada suatu elemen.

draggable

Menentukan apakah suatu elemen dapat di-drag atau tidak.

dropzone

Menentukan apakah data yang di-drag adalah data yang disalin, dipindahkan, atau ditautkan saat dijatuhkan.

hidden

Menentukan apakah suatu elemen ditampilkan atau tidak pada browser.

id

Menetapkan id pada elemen.

lang

Menentukan bahasa pada konten elemen.

spellcheck

Menentukan apakah elemen harus diperiksa ejaannya dan tata bahasanya atau tidak.

style

Menentukan styling secara satu baris untuk suatu elemen.

tabindex

Menentukan urutan dari suatu elemen.

title

Menentukan informasi tambahan tentang suatu elemen.

translate

Menentukan apakah konten elemen harus diterjemahkan atau tidak.

LIST

Pada HTML terdapat tiga tipe list:

Unordered lists : daftar yang ditampilkan tidak memiliki urutan. 
Unordered List
Seperti namanya, unordered list merupakan daftar yang tidak mementingkan urutan. Standarnya, unordered list menampilkan bullet pada tiap item list-nya (tetapi kita bisa mengubahnya dengan styling). Untuk menetapkan konten sebagai unordered list kita gunakan <ul></ul> kemudian di dalam elemen tersebut kita gunakan tags <li></li> untuk menetapkan 
item pada list tersebut.

Ordered lists : daftar yang ditampilkan secara terurut.
Ordered list digunakan untuk membuat list yang mementingkan urutan. Contohnya, membuat daftar instruksi langkah demi langkah sehingga dibutuhkan urutan yang sesuai. Ordered list bekerja seperti unordered list, namun perbedaanya pada tiap item menampilkan angka bukan sebuah bullet. Angka yang ditampilkan, otomatis berurut tiap itemnya, sehingga kita tidak perlu menuliskan secara kasar urutan nomornya. Hal ini tentu mempermudah kita untuk mengorganisir tiap itemnya. Untuk menetapkan konten sebagai ordered list kita gunakan 
<ol></ol>. Sama seperti Unordered list, tiap item dalam list ditetapkan dengan menggunakan tags <li></li>.

1

Menggunakan angka dalam urutan item (default)

a

Menggunakan huruf kecil dalam urutan item

A

Menggunakan huruf besar dalam urutan item

i

Menggunakan huruf romawi kecil dalam urutan item

I

Menggunakan huruf romawi besar dalam urutan item

Selain tipe angka pada urutan, kita juga bisa menetapkan nilai awal pada sebuah ordered list dengan menggunakan atribut start. Contohnya, jika kita ingin memulai sebuah list dari angka 7, maka kita tetapkan atribut start dengan nilai 7 pada elemen <ol>.
Normalnya urutan list diawali dengan urutan paling rendah dengan menambahkan atribut reversed pada elemen <ol> maka urutan dalam sebuah list akan dibalik. Atribut ini berbeda 
dengan atribut yang lain (yang sudah dibahas sebelumnya), atribut ini tidak memerlukan sebuah nilai ketika menggunakannya. Atribut ini hanya menandakan sebuah list untuk 
membalikan urutan angka pada tiap itemnya.

Description lists : daftar yang terbuat dari beberapa istilah diikuti dengan deskripsi dari istilah tersebut.

img
Dengan menetapkan hanya satu atribut ukurannya, maka ukuran lainnya akan mengikuti sesuai dengan rasio gambar aslinya. Contohnya, kita bisa menetapkan ukuran gambar berdasarkan 
nilai lebarnya saja.
  <!-- Menetapkan ukuran gambar berdasarkan lebar -->
<img src="https://i.imgur.com/EUUXQcf.png" alt="dicoding" width="500px">

Atau kita bisa tetapkan ukuran gambar berdasarkan tingginya. Dengan begitu nilai lebar akan menyesuaikan nilainya berdasarkan rasio gambar aslinya.
<!-- Menetapkan ukuran gambar berdasarkan tinggi -->
<img src="https://i.imgur.com/EUUXQcf.png" alt="dicoding" height="100px">
Perhatikan penulisan nilai dari atribut src. Penulisan sedikit berbeda dengan yang telah kita pelajari. Penulisan alamat gambar tidak dimulai dengan https://www, karena kita 
menggunakan gambar lokal yang ada pada project kita. Sehingga untuk penulisan path-nya mengarah ke lokasi dari berkas gambar tersebut.

Teks
Teks Terformat
Sejauh ini, kita sudah mengenal paragraf, heading dan juga list pada HTML. Tapi masih ada beberapa lagi yang merupakan spesial teks format yang dapat kita gunakan yaitu <blockquote>, <pre>, dan <figure>.
Jika pada konten kita memiliki sebuah kutipan ataupun sebuah testimonial, kita dapat gunakan format long quotations dengan menggunakan tags <blockquote>. Konten di dalam elemen <blockquote> ini dapat berupa sebuah paragraf, heading, ataupun list. 

Preformatted text
Pada sub-modul sebelumnya, kita sudah mengetahui bahwa HTML akan mengabaikan penulisan spasi yang dituliskan secara berulang dan juga line breaks (baris baru). Tetapi pada 
beberapa tipe konten seperti contoh kode atau puisi hal tersebut sangat berarti. Dengan begitu, terdapat sebuah elemen yang dapat kita gunakan untuk menampilkan konten sesuai 
yang kita tulis pada text editor. Untuk menggunakannya, kita gunakan elemen <pre> sebagai pembungkus kontennya.

Figure
Elemen ini digunakan untuk merepresentasikan konten tersendiri (self-contained content) seperti ilustrasi, diagram, foto atau bisa juga sebuah baris kode. Banyak hal yang dapat 
digunakan dalam elemen ini. Elemen ini digunakan untuk mengkelompokkan blok konten yang dapat dipindahkan posisinya dari blok utama sebuah dokumen tanpa mempengaruhi arti dari 
induk dokumen.Di dalam elemen figure kita dapat menuliskan elemen <figcaption> sebagai sebuah caption (judul) untuk konten tersebut. Berikut contoh penggunaan figure pada 
sebuah konten gambar.

Block & Inline
Standarnya elemen HTML memiliki dua sifat yaitu block dan inline. Elemen yang memiliki sifat block selalu membuat baris baru ketika menampilkannya, contohnya seperti elemen 
paragraf, list, heading, dan lainnya. Berlawanan dengan elemen yang memiliki sifat inline, elemen ini tidak menambahkan baris baru ketika dibuat. Apa saja elemen tersebut? Mari 
kita bahas satu persatu.

Anchor
Apa itu anchor? Anchor (jangkar) merupakan elemen yang digunakan untuk membuat sebuah hyperlink ke halaman atau website lain, file, alamat email, atau URL lainnya. Untuk 
menggunakan elemen ini kita gunakan tag <a>...</a> bersama dengan atribut href untuk menetapkan sebuah target yang akan dituju. 
Selain atribut href, terdapat beberapa atribut khusus yang dapat digunakan pada elemen ini, antara lain:

download

filename

Menginstruksikan browser untuk mengunduh pada URL yang ditetapkan daripada mengarahkannya.  

href

URL

Menetapkan target yang akan diarahkan/unduh ketika pengguna menekan hyperlink.

hreflang

language_code

Menetapkan bahasa dari dokumen target.

ping

list_of_URLs

Menetapkan URL yang akan diberitahu dengan mengirimkan post request ping pada body oleh browser (berjalan di belakang layar) ketika target URL pada hyperlink ditekan. Biasanya 
atribut ini digunakan untuk pelacakan.

referrerpolicy

no-referrer,

no-referrer-when-downgrade,

origin,

origin-when-cross-origin,

unsafe-url

Menetapkan referensi untuk dikirim pada target.

rel

alternate,

author,

bookmark,

external,

help,

license,

next,

nofollow,

noreferrer,

noopener,

prev,

search,

tag

Menetapkan hubungan antara halaman yang ditampilkan dengan target.

target

_blank,

_parent,

_self,

_top

Menetapkan lokasi ketika membuka target contohnya pada sebuah tab, window atau pada tab itu sendiri.

media

media_type

Menetapkan tipe media yang digunakan pada target.

Emphasized text
Gunakan elemen <em> untuk menunjukan bagian kata yang perlu kita tekankan. Elemen ini menunjukan stress emphasis atau konten/kata yang perlu mendapatkan penekanan atau 
perhatian khusus. Berikut contoh penggunaannya.

<p><em>Oding</em> adalah seorang pelajar</p>
<p>Dia adalah seorang <em>pelajar</em></p>

Important text
Gunakan elemen <strong> untuk menunjukan sebuah teks yang begitu penting (strong importance), serius, ataupun mendesak. Dalam arti teks tersebut harus dapat perhatian lebih 
dari teks biasa lainnya.

<p>Kesehatan merupakan hal yang penting, jaga pola makan yang teratur dan <strong>jangan sampai makan tengah
   malam!</strong></p>

Standarnya pada browser sebuah teks yang diberi markup <strong> akan ditampilkan secara tebal. Dan ketika pengguna menggunakan pembaca layar (screen reader), suara yang 
terdengar akan berbeda. Ini mengartikan bahwa teks tersebut penting tidak hanya sekedar tebal.
20200619114537f8b876288310e434844a1df72202ea98.jpeg 


Short quotations
Gunakan elemen <q> untuk menandai sebuah kutipan dalam sebuah teks. Elemen short quations berbeda dengan <blockquote>. Elemen ini digunakan untuk kutipan pendek yang terletak 
di dalam baris (inline).

<p>Sebelum pulang kerja, ia berkata kepadaku: <q>Maaf saya tidak bisa hadir dalam pertemuan nanti</q></p>


Standarnya pada browser sebuah teks yang diberi markup <q> akan ditampilkan di dalam tanda kutip (Quotation marks).
202006191147088a27b9e3b4e6109fbd24333e47d3c83e.jpeg


Citation
Selain sebuah atribut, <cite> juga merupakan sebuah elemen yang digunakan untuk sebuah rujukan pada sebuah dokumen, contohnya sebuah buku, majalah, artikel dan lainnya.

<p>Informasi selengkapnya bisa Anda dapatkan di <cite><a href="https://dicoding.com">dicoding.com</a></cite>.</p>

Standarnya pada browser sebuah teks yang diberi markup <cite> akan ditampilkan dengan garis miring (italic).
20200619114757d2953d11afea469ca28408ed961c8f12.jpeg



Defining terms
Elemen <dfn> digunakan ketika mendefinisikan sebuah istilah (term). Elemen ini harus terletak pada elemen lain yang menaunginya. Contohnya pada sebuah elemen <p> atau elemen 
<section>. Berikut contoh penggunaannya:

<p><dfn>Website</dfn> merupakan halaman yang menampilkan informasi melalui teks atau gambar. Website dapat diakses melalui internet dengan menggunakan browser.</p>

Standar pada browser yakni sebuah teks yang diberi markup <dfn> akan ditampilkan dengan garis miring (italic).




Subscript dan Superscript
Subscript <sub> dan superscript <sup> merupakan elemen yang dapat membuat teks yang ditampilkan nampak kecil, dengan posisi di bawah (sub) atau di atas (sup) dari teks 
biasanya. Elemen ini digunakan untuk menunjukan sebuah rumus kimia ataupun matematika.

<p>Sukrosa merupakan suatu disakarida yang dibentuk dari monomer-monomernya yang berupa unit glukosa dan fruktosa,dengan rumus molekul 
C<sub>12</sub>H<sub>22</sub>O<sub>11</sub>.</p>
 
<p>Salah satu persamaan paling umum dalam semua fisika adalah E=MC<sup>2</sup></p>

Jika kita lihat pada browser, tampilan akan tampak seperti ini:
20200619115528d60c86b36ee29b8964700e8c99816856.jpeg



Highlighted text
Untuk menandai atau menyorot sebuah teks kita bisa menggunakan elemen <mark>. Elemen ini digunakan ketika terdapat sebuah teks yang memiliki peran penting, biasanya teks 
tersebut merupakan bagian yang paling relevan atau penting dalam sebuah konteks kalimat.

<p>Ini adalah periode perang saudara. Pesawat ruang angkasa pemberontak, menyerang dari pangkalan tersembunyi, telah
   memenangkan kemenangan pertama mereka melawan Kekaisaran Galactic yang jahat. Selama pertempuran,
   <mark>mata-mata
       Pemberontak berhasil mencuri rencana rahasia
   </mark>
   ke senjata pamungkas Kekaisaran, STAR DEATH, stasiun ruang angkasa
   berlapis baja dengan kekuatan yang cukup untuk menghancurkan seluruh planet.
</p>

Standarnya pada browser teks yang diberi markup <mark> akan ditampilkan dengan background kuning dan teks hitam.
202006191159200762944f2098e172dd4cbd4db1ab3fc0.jpeg



Line Break
Terkadang kita mungkin perlu menambahkan sebuah baris baru pada sebuah baris teks (termasuk di dalam paragraf), tetapi kita mengetahui bahwa browser akan mengabaikan sebuah 
penulisan spasi ganda ataupun garis baru, sehingga kita memerlukan sebuah tanda yang dapat digunakan untuk memberitahu browser untuk “Tambahkan garis baru di sini!”.

Inline line break element atau <br> dapat digunakan untuk memberitahu browser untuk memberikan sebuah garis baru pada baris teks. Sama seperti gambar, elemen ini merupakan 
elemen kosong sehingga kita tidak membutuhkan sebuah tag penutup.

<p>
   Dicoding Space,<br>
   Jln. Batik Kumeli No. 50.<br>
   Bandung.<br>
   40123
</p>

Jika kita lihat pada browser, maka tampilan akan tampak seperti ini:
