<h1>Komunikasi Serial</h1>

<p>Komunikasi serial digunakan oleh arduino untuk dapat berkomunikasi dengan komputer atau perangkat lain ( mikrokontroller lain, modul bluetooth, sensor berbasis serial, dll). Pada arduino, komunikasi serial terdapat pada pin TX/RX dan menggunakan tegangan logic TTL ( 5v atau 3.3v tergantung jenis arduinonya). Sedangkan pada komputer(RS232) tegangan logic yang dipakai adalah +12v dan -12v. Semua arduino sudah bisa melakukan komunikasi serial secara default ke komputer melalui USB.</p>

<p>Pin Serial pada arduino adalah pada Pin 0 (RX) dan Pin 1 (TX). So, Jika kita sudah menggunakannya sebagai alat komunikasi serial, maka kita tidak bisa lagi menggunakan Pin tersebut untuk keperluan lain.</p>

<h2>Debugging Dengan Serial</h2>
<p>Proses debugging kode memang selalu menantang, dan akan terasa lebih sulit lagi jika harus melakukan debugging pada kode sekaligus rangkaian elektronik. Meskipun kita baru memasuki pelajaran Arduino ketiga, sekarang saatnya mulai mengenal beberapa strategi debugging Arduino.</p>

<p>Untuk debugging perangkat keras (hardware), alat seperti multimeter dan osiloskop sangat membantu. Namun, karena tidak semua orang memiliki alat tersebut, alternatifnya adalah menggunakan software simulasi seperti Tinkercad Circuits yang menyediakan instrumen virtual, misalnya multimeter digital. Jika rangkaian yang dibuat secara fisik tidak berfungsi, Anda bisa mencoba mereplikasinya terlebih dahulu di Tinkercad atau simulator lainnya untuk menemukan sumber masalah.</p>

<p>Sementara itu, untuk debugging program (kode), metode yang umum digunakan adalah menambahkan perintah printline untuk memantau jalannya program. Saat ini, Arduino IDE belum menyediakan fitur debugging lanjutan seperti breakpoint, eksekusi kode langkah demi langkah, atau analisis memori. Namun, Tinkercad Circuits menyediakan fitur debugging sederhana, seperti menjalankan kode secara bertahap, yang dapat membantu dalam proses analisis kesalahan.</p>

<p>Komunikasi serial dan proses debugging merupakan bagian penting dalam penggunaan papan Arduino. Secara sederhana, komunikasi serial adalah cara yang digunakan Arduino untuk bertukar data atau berkomunikasi dengan perangkat lain, seperti komputer, sensor, atau perangkat tambahan lainnya. Dalam membahas komunikasi serial pada Arduino, penting untuk memahami dua aspek utama, yaitu komponen fisik dan komponen perangkat lunak. Komponen fisik mencakup bagian hardware seperti port serial pada Arduino, sedangkan komponen perangkat lunak berkaitan dengan penggunaan fitur seperti Serial Monitor pada Arduino IDE untuk melihat dan menganalisis data yang dikirim oleh Arduino.</p>

<h2>Buat program Serial.print “Hello World!” yang sederhana</h2>
