# PADLibrary
Library Digital
TAHAPAN MEMBANGUN DIGITAL LIBRARY dengan MIT APP INVENTOR
Langkah 1: Persiapan Awal desain perpustakaan digital
Buka MIT APP INVENTOR: Akses MIT APP INVENTOR melalui browser Chrome. Masuk dengan email dan klik “New Project” untuk memulai. 
Desain Tampilan Utama: Rancang layout aplikasi menggunakan komponen “Horizontal Arrangement” dari palette. Atur height dan width dengan memilih “Fill Parent”.
Tambahkan Komponen Interaktif: selanjutnya klik User interface lalu drag-and-drop “Label” untuk menampilkan teks dalam aplikasi. Dan “Button” untuk mendeteksi ketukan penggunal.
Membuat Layar Baru: klik “Add Screen” untuk membuat layar baru bernama “PADLIB” atau nama perpustakaan digital sesuai keinginan. Susun komponen secara horizontal dengan “Horizontal Arrangement”  atur height dan width dengan memilih “Fill Parent” . Tambahkan “label” dan “button” untuk kategori buku (disini kami mencontohkan dengan kategori fiksi dan nonfiksi). Beri label pada tombol dengan nama kategori masing-masing. 

Langkah 2: Membuat layar buku fiksi
Buat layar baru: buat layar baru bernama “Buku Fiksi”. 
Susun layout: drag-and-drop komponen “Horizontal Arrangement” atur height dan width dengan memilih fill parent.
TAmbahkan tombol buku: drag-and-drop “Button” untuk mewakili buku yang ingin ditampilkan. 
Beri nama tombol: beri nama pada tombol dengan format “Buku 1” dan seterusnya sesuai jumlah buku yang akan ditampilkan.
Tambahkan “ActivityStarter” dengan melakukan drag-and-drop. lalu isi bagian “Action” dengan “android.intent.action.VIEW”

Langkah 3: Pemrograman dengan Blocks
Membuat program untuk tampilan halaman buku fiksi: 
Pilih ‘Variables’ dan drag-and-drop ‘initialize global name to’ untuk membuat suatu variabel global. 
Ubah ‘Name’ menjadi ‘buku-buku’.
Pilih ‘Dictionaries’ lalu drag-and-drop ‘Make a dictionary’ 
Tambahkan ‘Pair’ untuk setiap buku yang ingin ditampilkan. 
Menghubungkan tombol dengan buku:
Klik ‘Buku 1” pada ‘TableArragement1’ 
Drag-and-drop ‘Buku 1’ yang letaknya paling bawah lalu letakkan pada ‘key’ yang berada di ‘Make a dictionary’.
Lakukan langkah tersebut sampai semua ‘key’ terisi. 
Mengisi link untuk buku:
Isi ‘value’ dengan menu “text” yang kosong untuk setiap buku. 
Isi menu “text” yang kosong dengan link buku yang ingin ditampilkan.
Drag-and-drop  “when any Button Click” pada “Any component”.
Klik “Control” lalu drag-and-drop “if” yang berada paling atas. Letakkan “if” pada “when any Button Click”. 
Klik “Dictionaries” lalu drag-and-drop “is key in dictionary?”. Letakkan “is key in dictionary?” pada “if”. 
Isi “key” dengan “getcomponent”.
Isi  “dictionary” dengan “initialize global buku-buku” pada bagian “is key in dictionary?”.
Klik “ActivityStarter” lalu drag-and-drop “set ActivityStarter 1”. Letakkan “set ActivityStarter 1” pada “then” dari “if”. 
Ubah “DataUri” menjadi URL dengan cara klik “Dictionary” lalu drag-and-drop “get values for key”. Isi “key dengan “component” dan “Dictionary” dengan “initialize global buku-buku”.
Klik “ActivityStarter” lalu drag-and-drop “call ActivityStarter 1. StarActivity” dan letakkan di bawah “set ActivityStarter 1”. (baru sampai menit 10.44)

Langkah 4: Dilanjutkan pemrograman untuk halaman pertama dan kedua design: 
Halaman pertama:
klik “Button 1”
pilih “when button1” 
Pilih "Control" dan klik "Open another screen".
Pilih "screenName" dan atur ke "PILIH_KATEGORI".
Pindahkan aksi ini ke dalam "When button 1 clicked".
Pada "Screen 1", klik "PILIH_KATEGORI".
Halaman kedua:
Ulangi langkah 1 untuk "Button 1" pada "Screen 1".
Ganti "screenName" dengan "Fiksi" untuk membuka halaman buku fiksi.
Ulangi langkah 1 untuk "Button 2" pada "Screen 1".
Ganti "screenName" dengan "Non Fiksi" untuk membuka halaman buku non-fiksi.

Langkah 5: Dilanjutkan memprogram untuk tampilan pada halam buku Non fiksi
langkah pemrograman sama seperti pada pembuatan tampilan buku “fiksi”.

Langkah 6: Pembuatan “Button” untuk kembali pada halaman sebelumnya. 
membuat tombol “Button”
gunakan elemen “Text for Button” drag-and-drop ke bagian bawah tampilan buku “Fiksi” dan “Non Fiksi”. 
Lalu Width diubah menjadi “Fill Parent” dan kolom Text diisi dengan “Kembali”
Lalu beralih pada blocks untuk memprogram
Beralih ke blok "Pemrograman".
Klik pengaturan pada blok "if" dan tambahkan "else if".
Pilih menu "Logika" dan tarik-dan-lepas menu "=".
Isi bagian sebelum tanda "=" dengan "Component" dan isi bagian setelah tanda "=" dengan "Button2".
Buka menu "Kontrol" dan tarik-dan-lepas "buka layar lain" dan letakkan di "then".
Ubah "screen1" pada "buka layar lain" menjadi "PILIH_KATEGORI".

Langkah 7: Menambahkan cover buku yang akan dilayankan 
Pilih buku: Klik pada bagian buku yang ingin ditambahkan sampulnya.
Upload gambar: Buka menu "Media" dan pilih "Upload File".
Pilih gambar sampul: Pilih gambar yang ingin digunakan sebagai sampul buku yang sesuai dengan isi bukunya.
Ulangi: Ulangi langkah 1-3 untuk semua buku yang ingin ditambahkan sampulnya.
Selesai 

CARA PENGAKSESAN “PADLIB”
Pengguna dapat mengklik URL yang diberikan oleh grup kami untuk mengakses PADLIB.
Selanjutnya, pengguna akan diarahkan untuk mendownload aplikasi PADLIB setelah mengklik tautan tersebut.
Setelah aplikasi PADLIB diunduh, pengguna dapat langsung login pada aplikasi dan  dapat memilih jenis kategori koleksi yang diperlukan. 
Pengguna kemudian dapat memilih koleksi yang mereka sukai, dan aplikasi PADLIB akan menampilkan koleksi yang diperlukan.
