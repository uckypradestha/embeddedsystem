<h2>Menghidupkan LED Dengan Pin GPIO Arduino</h2>
<p>Pada kegiatan pembelajaran pertama ini, kita akan menggunakan Arduino untuk menyalakan sebuah LED. Kita belum akan menulis kode apa pun. Tujuan utama kegiatan ini adalah untuk mulai mengenal perangkat keras Arduino serta cara menghubungkan komponen ke pin-pin Arduino. Pemrograman akan diperkenalkan pada pelajaran berikutnya.</p>

<img src="../image/Turn on LED.png">

<h3>Alat dan Bahan</h3>
<p>Dalam percobaan sederhana ini, berikut alat dan bahan yang digunakan:</p>

<div align="center">
<table border="1" cellpadding="10" cellspacing="0" width="100%">
  <tr>
    <th>Arduino</th>
    <th>LED</th>
    <th>Resistor</th>
  </tr>

  <tr align="center">
    <td>
      <img src="../image/arduino_uno.png" width="260"><br>
    </td>
    <td>
      <img src="../image/RedLED_Fritzing.png" width="130"><br>
    </td>
    <td>
      <img src="../image/Resistor220_Fritzing.png" width="200"><br>
    </td>
  </tr>

  <tr align="center">
    <td>Arduino Uno, Leonardo, atau lainnya</td>
    <td>Red LED</td>
    <td>220Ω Resistor atau lainnya</td>
  </tr>
</table>
</div>

https://github.com/user-attachments/assets/f7cdb8a6-88bf-4d08-8d53-e44660e340a3

<h1>Pengenalan GPIO</h1>
<p>GPIO (General Purpose Input/Output) adalah salah satu fitur penting dalam pengembangan proyek elektronik dan pemrograman mikrokontroler. Pada Arduino, fungsi GPIO memungkinkan pengguna untuk melakukan interaksi langsung dengan lingkungan sekitar, seperti membaca data dari sensor, mengoperasikan motor maupun menyalakan LED. GPIO adalah pin pada mikrokontroler atau komputer papan tunggal (seperti Raspberry Pi) yang dapat dikonfigurasi sebagai input atau output sesuai kebutuhan pengguna. Pin-pin ini tidak memiliki fungsi khusus bawaan, sehingga disebut "general purpose" (serbaguna).</p>

<p>Pada tahap ini, kita mulai menyalakan LED menggunakan program dengan memberikan logika HIGH (5V) pada Pin 11. Selanjutnya, program tersebut akan diubah sehingga LED tidak hanya menyala terus, tetapi juga dapat berkedip. Untuk itu, kita perlu memahami konsep keluaran digital pada Arduino.</p>

<p>Arduino Uno memiliki 20 pin GPIO yang dapat digunakan untuk menerima atau mengirim sinyal digital, yaitu HIGH dan LOW. Sinyal ini dikendalikan melalui fungsi digitalRead() untuk membaca dan digitalWrite() untuk menulis nilai digital.</p>

<p>Walaupun pin digital lain juga bisa digunakan, Pin 11 dipilih agar konsisten dengan pelajaran selanjutnya, sehingga proses belajar menjadi lebih sederhana dan tidak membingungkan.</p>

<img src="../image/ArduinoUno_DigitalIOPins.png">

<p>Anda dapat mengendalikan salah satu dari 20 pin digital I/O tersebut dengan menggunakan tiga fungsi berikut:</p>
<ul>
  <li>pinMode(int pin, int mode). Fungsi ini digunakan untuk mengatur sebuah pin agar berfungsi sebagai INPUT atau OUTPUT. Dalam kasus ini, kita memilih OUTPUT karena kita ingin mengirimkan sinyal untuk menyalakan LED.</li>

<li>digitalRead(int pin). Fungsi ini digunakan untuk membaca sinyal digital dari pin tertentu, yaitu HIGH atau LOW. Fungsi digitalRead akan dibahas lebih lanjut pada seri pelajaran pengantar input.</li>

<li>digitalWrite(int pin, int value). Fungsi ini digunakan untuk mengirimkan sinyal digital ke pin tertentu, yaitu HIGH atau LOW. Pada pelajaran ini, kita akan menggunakan fungsi digitalWrite.</li>
</ul>

<h2>Bagaimana kita menghitung 20 pin I/O digital?</h2>
<p>Pada Arduino Uno dan Leonardo, tulisan dan label pada papan sering membuat kita mengira hanya ada 14 pin digital. Padahal, jika dilihat secara keseluruhan, terdapat 20 pin digital I/O yang bisa digunakan. Untuk memastikan hal ini, kita dapat melihat diagram pinout resmi Arduino Uno yang menunjukkan semua pin yang tersedia.</p>

<img src="../image/ArduinoUno_OfficialPinOutDiagram.png">

Untuk lebih jelasnya, berikut pin I/O digtial dan analog

<img src="../image/ArduinoUno_OfficialPinOutDiagram_DigitalIOPinsMarked.png">

<h2></h2>
<a href="https://komputer.ft.unsoed.ac.id/"><img src="../image/Footer.jpg"></a>
