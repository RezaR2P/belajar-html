#FORMATING TAG
<b>,<strong> biasanya digunakan saat ada hal penting pro tips gunakan <b> saja saat hanya ingin menebalkan
<i>,<em> Gunakan elemen <i> hanya jika tidak ada elemen semantik yang lebih tepat, seperti:
    <em> (teks yang ditekankan)
    <strong> (teks penting)
    <mark	> (teks yang ditandai/disorot)
    <cite> (judul sebuah karya) bisa di gabung dengan block quote
    <dfn> (istilah definisi)
    <abbr title="">yaitu singkatan dari suatu kalimat contoh nya dr yaitu Doctor
<small> untuk teks kecil
<del> untuk text coret
<ins> untuk text garis bawah
<sub> untuk subscript text yang ada diatas seperti pangkat
<sup> untuk superscript text yg ada di bawah seperti CO(2)
<blockquote> yaitu kalimat kutipan yang panjang
<q> yaitu kalimat kutipan yang pendek

#LIST
1.list yg ada urutan (order list) dalam kodingan nya <ol> dan di lanjutkan dengan <li> atau list item
2.list yg tidak ada urutan nya (unorder list) dalam kodingan nya <ul> dan di lanjutkan dengan <li> atau list item
3.description list yg menjelaskan suatu kalimat (description list) dalam kodingan nya <dl> yaitu data list dan dilanjutkan dengan <dt> atau data term dan <dd> data description untuk menjelaskan definisinya
4.list bersarang yaitu list yg ada di dalam list (nested list) dalam kodingan nya hanya memasukkan list di dalam list seperti menggabungkan list ul dan ol maupun sebaliknya
!!catatan list ol bisa menggunakan huruf romawi atau angka atau huruf a kecil dan A besar

#LINK
1.link eksternal yaitu yang menggunakan dari website lain. ini sangat tidak di sarankan karena mungkin saja suatu saat website orang lain bisa saja mati dan link kita tidak bisa jalan
2.link internal yaitu link yang menggunakan local ini sangat di rekomendasikan karena kita yg mengatur sendiri bukan tergantung orang lain
3.link send email href nya yaitu mailto:namagmailygmaudikirimpesan
4.link juga bisa menerima id dengan menggunakan namafile#id maka akan loncat ke id tersebut
!!catatan pakai target="_self" akan ditampilkan dihalaman yang sama (default)
                target="_blank" akan ditampilkan dihalaman yang beda atau buat tab baru
                title="namalink" untuk menuliskan judul yg keluar ketika mouse berada di link tersebut

#Relative URL
Relative URL adalah lokasi href dimana tetap menggunakan domain website saat ini Relative URL memiliki dua format, bisa diawali dengan /, atau tidak diawali dengan/
Misal sekarang kita berada di halaman http://127.0.0.1/belajar-link/index.html, lalu kita memiliki link sebagai berikut:
hello.html, artinya akan menuju ke http://127.0.0.1/belajar-link/hello.html
../hello.html, artinya akan menuju ke http://127.0.0.1/hello.html
pzn/hello.html, artinya akan menuju ke http://127.0.0.1/belajar-link/pzn/hello.html
intinya gunakan ../ jika ingin keluar folder

#TABEL
1.untuk membuat tabel menggunakan tag table
2.tr untuk baris
3.th untuk header
4.td untuk data
5.thead untuk grup header
6.tbody untuk grup isi data
7.tfoot untuk grup footer
8.colspan untuk menggabungkan 2 atau lebih kolom
9.rowspan untuk menggabukan 2 atau lebih baris

#RESERVED CHARACTERS
jika tidak bisa menggunakan simbol cari di google simbol entity ada di github dan google lainnya

#FORM
1.<form> untuk mengawali pembuka
2.diwajikan menggunakan name, berisi informasi nama form dan nama form harus unik tidak boleh ada yang sama
3.action berisi url kemana informasi form tersebut akan dikirimkan
4.sangat disarankan menggunakan enctype agar data yg dikirim kan ke server aman
-application/x-www-form-urlencoded(default) cocok untuk mengirimkan data teks biasa
-multipart/form-data digunakan ketika kita mau mengirim file agar terenkripsi lebih aman
4.method ada dua yaitu get dan post, get adalah menerima data dari server sedangkan post adalah mengirim data ke server
2.<label> untuk melabelkan suatu kata dan diwajibkan menggunakan id di inputnya agar bisa terhubung dengan label
3.<input type=""> untuk membuat sebuah interaksi dan input banyak macam nya
-type text membuat sebuah text area kecil untuk mengisi sebuah data
-tag textarea untuk input text multi baris kita juga bisa mengatur kolom dan baris
-tag button sangat flexible di bandinkan dengan type button, button bisa menjadi submi,reset,maupun image src
-type password membuat sebuah text menjadi *** agar tidak di ketahui orang
-type radio untuk membuat pilihan lebih dari 1
!!untuk radio name nya harus sama
-type checkbox untuk membuat sebuah pilihan centang hanya 1
!!untuk checkbox name nya harus sama
-type color type untuk menerima input warna
-type date adalah jenis input untuk memasukan tahun,bulan,dan tanggal
-type datetime-local jenis inout mirip seperti date tapi lebih spesifik ada tambahan jamnya contohnya <input type="datetime-local" name="waktu" id="waktu">
!!ntah kenapa di laptop saya tidak bisa memilih waktu
-type month hanya bulan dan tahun
!!ini juga sama tidak bisa memilih dari kalender
-type time hanya jam dan menit
!!error juga tidak bisa pilih waktu di browser saya kemungkinan besar firefox tidak support
-type week hanya minggu dan tahun
!!error juga
-type email harus berformat email jika tidak maka tidak akan bisa di submit
-type tel yaitu input telephone bisa digunakan untuk mengisi no telephone dan tidak bisa di submit ketika yg dikirim bukan number dan ada beberapa rule lainnya akan dipelajarin lebih dalam di javascript
!!tambahkan pattern (harus diawali contoh 62)[angka yg di perbolehkan misalkan 0-9] {min max misalkan 5,20}
-type number harus berfortmat number jika tidak maka akan tidak bisa di submit
-type range sama seperti number tapi bukan teks hanya bisa menggeser ke kanan dan ke kiri dengan defaultnya 1+ dan -1 dimulai dari 0
-type file untuk mengupload sebuah file
!!diharus kan mengunakan method post dan juga enctype multipart/form
-type url digunakan ketika menerima url seperti medsos,website dll
!!url memiliki rule dimana harus url
-type hidden input datanya tidak terlihat oleh penggguna web akan tetapi akan di tambahkan saat kita submit
-type button tombol tidak berguna ketika tidak memakai javascript
-type image fungsinya sama seperti tombol submit tapi berupa gambar
!!type="image" src="file"
-type reset adalah input yg akan ditampilkan dalam bentuk tombol sama seperti submit jika di klik maka akan berubah menjadi nilai default seperti diawal
-type submit untuk mengirim sebuah data yg kita buat 
4.jangan lupa kasih name, value, dan id untuk menandai sebuah data
5.dropdown list membuat sebuah pilihan kebawah
-menggunakan <select> name, dan id
-di dalam nya menggunakan <option value="ini yang akan dikirim ke database"> sdan selected adalah yg dipilih pertama kali
-selected juga bisa menggunakan optgruop untuk memilih lebih spesifik
-optgroup menggunakan label untuk kategori misalkan gaming
-dilanjutkan dengan option value pilihan biasa contohnya free fire
8.datalist membuat pilihan auto complite
-datalist menggunakan list pada input lalu di hubungkan dengan id hobbies
-lalu datalist menggunakan option sama seperti memakan select atau drop down
9.fieldset digunakan tuntuk membungkus beberapa input sehingga mudah dibaca oleh pengguna
-legend digunakan untuk mendeskripsikan grouping

#GAMBAR
1.membuat folder img untuk menyimpan semua gambar
2.untuk menampilkan gambar kita menggunakan <img src="nama file" namafolder/gambar.jpg /adalah untuk masuk ke dalam folder
3.jangan lupa atur height atau width dengan px untuk seberapa besar dan kecil atau % mengikuti seberapa besar dan kecil nya browser kita
-saya sarankan pilih salah satu diantara width dan heigth agar gambar tidak gepeng
-alt adalah alternatif text ketika gambar kita rusak atau eror
-tittle adalah text nama pada gambar kita, akan kelihatan saat kita menghover pada gambar tersebut
4.align="" untuk merapihkan huruf dan gambar
-top atas
-left kiri
-right kanan
-bottom bawah
-justify kiri dan kanan
-center tengah
5.Picure Content kita bisa menambahkan tag source yang berisi lokasi gambar, dan tag img sebagai default gambar ketika semua kondisi tag source tidak terpenuhi

#VIDEO
1.membuat folder video untuk menyimpan semua video
2.kita juga bisa memakai thumbnail video menggunakan foto yg tersimpan di folder img
3.<video src="namafile"> untuk pembuka
-pakai width atau heigh untuk menyesuaikan ukuran video
-tambahkan controls agar bisa mengontrol seperti play pause dll
-poster untuk membuat tumbnail atau cover video
-autoplay ketika membuat browser langsung play videonya
-preload ada none,auto dan metadata disarankan metadata agar tidak menghabiskan kuota orang lain
-loop memutar video kembali ketika sudah selesai

#AUDIO
1.membuat folder sound untuk menyimpan suara file mp3
2.<audio src="namafile"> untuk pembuka
-tambahkan controls agar bisa mengontrol seperti play pause dll
-autoplay ketika membuat browser langsung play
-preload ada none,auto dan metadata disarankan metadata agar tidak menghabiskan kuota orang lain
-loop memutar suara kembali ketika sudah selesai

#COMPUTER CODE
1.<pre> ingin menulis kode apa adanya seperti enter dan spasi lebih dari 1 misalnya kita saat membuat kode program
2.<code> digunakan untuk menandai teks yang merupakan kode sumber atau kode pemrograman dalam suatu dokumen

#EMOJI
kita bisa menggunakan emoji dengan kode hexadesimal untuk link nya ada di bawah ini :
https://www.quackit.com/character_sets/emoji/emoji_v3.0/unicode_emoji_v3.0_characters_all.cfm

#FAVICON
yaitu logo perusahaan yang muncul di samping title tab
1.untuk menggunakan favicon kita bisa menggunakan tag link
2.dimana dalam link kita perlu menggunakan attribut rel="icon" dan href menuju lokasi gambar contohnya <link rel="icon" href="facebook.jpg"
3.gambar icon bisa file berupa .ico .png .jpg .svg atau .gif

#DIV
1.<div> adalah sebuah pembungkus atau wadah untuk menandai setiap element element kode html contohnya:
<div id="menu"> div ini adalah menu
<p>beranda</p>
</div>
<div id="content"> div ini adalah content
<p>ini adalah artikel</p>
</div>
2.dan div ini adalah block display dimana menghabiskan semua block dari kiri ke kanan

#SPAN
1.span ini adalah inline display misal kita membuat tulisan facebook, namun tiap kata bisa berbeda warna tapi hal itu tidak bisa dilakukan jika menggunakan tag p

#INLINE FRAME
1.inline frime bisa mengambil atau menggabungkan sebuah kode ke halaman kita
2.koding nya <iframe src="sumber kode yang mau kita masukan" frameborder="0 (gunakan default nya saja 0 agar rapih tidak terlihat ada garisnya" height="" width="" (heigh dan width menyesuaikan saja)> disini kita isi apa saja, jadi ketika browser tidak mendukung atau error maka akan memunculkan tulisan ini </iframe>

#SEMANTIC TAG
1.Tag article, untuk konten artikel
2.Tag aside, untuk bagian disamping konten, misal sidebar
3.Tag figure, untuk konten ilustrasi, diagram, foto, dan lain-lain
4.Tag figurecaption, untuk keterangan tag figure
5.Tag footer, untuk bagian footer dokumen
6.Tag header, untuk bagian header dokumen
7.Tag main, untuk konten utama dokumen Tag mark, untuk bagian yang ditandai atau highlight
8.Tag nav, untuk bagian navigasi link
9.Tag section, untuk section di dokumen
10.Tag details, untuk bagian yang lebih detail yang bisa pengguna lihat
11.Tag summary, untuk heading untuk tag details
12.Tag time, untuk konten waktu/tanggal
!!CATATAN sangat di sarankan menggunakan Semantic tag dibandigkan menggunakan div atau span dikarenakan ketika <div> nya sudah banyak, kita akan kesulitan membacanya
!!Salah satu kegunaan menggunakan semantic layout adalah akan lebih mudah saat menggunakan layout/css hal ini dikarenakan tiap tag memiliki arti

#RESPONSIV
tips and trick
Responsive ini berguna ketika kita membuat sebuah web atau projek dengan layar yg berbeda seperti diakses dengan komputer,handphone,tablet maupun tv maka ukuran suatu gambar atau teks akan beradaptasi tergantung layar
1.pada html 5 kita bisa menggunakan meta viewport contohnya:
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
yang artinya ketika dibuka oleh handphone atau pun tablet maka web kita mengikuti ukuran layar dari devicenya
2.jika saat kita menentukan ukuran dan ingin responsive di semua device maka disarankan menggunakan % sebagai ukuran element nya contohnya 100%
3.untuk responsive pada teks kita bisa menggunakan vw (viewport width)untuk ukuran font contohnya 5vw
4.untuk kasus dimana gambar terlalu kecil dan layar terlalu besar gambar akan pecah maka kita bisa menggunakan MEDIA QUERY ini akan di pelajari di materi css

#ID
1.id merupakan attribut yg digunakan untuk menandai element html
2.id harus unik di dalam 1 halaman html,artinya tidak boleh ada yang sama
3.dengan menggunakan id kita bisa memanngil suatu element lebih mudah apalagi jika saat menggunakan css ada lebih dari 5 tag div
4.untuk pemanggilan kode id pada css maka kita bisa menggunakan # contohnya id="tes" di css #tes

web tag element html 5
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/portal
