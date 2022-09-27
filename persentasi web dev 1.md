#### Sheha Luthfi Annisa | (Back-End Development)

# **Writing Web Development Basic Minggu 1**

### **----- Unix Command Line -----**

- **Shell** adalah program yang digunakan untuk berkomunikasi atau memerintah sistem
- **CLI (_Command Line Interface_)** adalah sebuah program yang memungkinkan user mengetik perintah atau command yang akan memerintahkan perangkat komputer untuk melakukan suatu tugas tertentu
- **Cara mengakses CLI di terminal** : User dan komputer dihubungkan dengan namanya terminal, yaitu tempat/aplikasi dimana user dapat mengetikan atau memberikan suatu perintah
- **File System** berfungsi untuk menyediakan mekanisme untuk penyimpanan data dan program yang dimiliki oleh sistem operasi serta seluruh pengguna dari sistem komputer

* Beberapa Command pada CLI beserta fungsinya :
  - Navigation
    - **ls** (_list_) yaitu command untuk melihat isi file yang ada di sebuah directory
  - File Manipulation
    - **touch** yaitu command untuk membuat sebuah file
    - **cp** (_copy_) yaitu command untuk mengcopy files atau directory
    - **mv** (_move_) yaitu command untuk memindahkan file atau directory. Bisa juga digunakan untuk rename file atau directory
    - **rm** (_remove_) yaitu command untuk menghapus file atau directory
  - Folder / Directory Manipulation
    - **mkdir** yaitu command untuk membuat sebuah directory
    - **cd** (_change directory_) yaitu command untuk berpindah directory
    - **pwd** (_Print working directory_) yaitu command untuk melihat current working directory
  - Text
    - **echo** yaitu command untuk menampilkan sesuatu kata atau kalimat dalam sebuah file
    - **cat** yaitu command untuk melihat isi sebuah file
    - **nano** yaitu command untuk menampilkan konten yang dapat diedit

### **----- Git & Github Dasar -----**

- **Git** merupakan aplikasi yang dapat melacak suatu perubahan yang terjadi di suatu folder ataupun file. Biasanya digunakan oleh programmer sebagai tempat untuk menyimpan file program mereka karena lebih efektif
- **Github** merupakan vendor penyedia layanan git yang dimiliki oleh microsoft atau secara definisi merupakan layanan hosting berbasis web sebagai repositori git
- **Alasan wajib menggunakan Git & Github**
  - Alasan utamanya adalah sepandai apapun programmer, tidak akan mampu untuk mengerjakan semuanya sendiri selamanya. Maka dari itu dengan menggunakan Git & Github akan memudahkan programmer untuk bisa bekerja sama dalam sebuah tim. Tujuan besarnya adalah programmer bisa berkolaborasi dengan programmer lainnya dengan mengerjakan proyek yang sama tanpa harus repot copy paste folder aplikasi yang terupdate
- **Command di dalam Git & Github**
  - **git init** <_nama_proyek_>, untuk membuat repositori baru
    - contoh : git init proyek01
  - **git commit** untuk melakukan commit atau menyimpan perubahan pada version control pada git. Bisa juga menambahkan pesan untuk memberikan checkout pada setiap perubahan
    - contoh : git commit
    - contoh : git commit -m "Commit Pertama"
  - **git push origin** untuk mempublish file atau aplikasi ke github
    - contoh : git push origin
  - **git clone** untuk melakukan cloning dari github ke komputer atau local
    - contoh : git clone https://github.com/shehaannisa/cobagit.git

### **----- HTML (_Hypertext Markup Language_) -----**

- **Definisi HTML** merupakan bahasa komputer yang digunakan untuk membuat kerangka atau struktur untuk Web pages (halaman website) di internet.
- **Bagaimana peran HTML pada web development?** : Web browser seperti Chrome, Firefox, Edge, Safari, atau Opera akan membaca dokumen HTML. Dokumen HTML yang berisi tag-tag HTML akan memberitahu browser bagaimana cara menampilkan sebuah konten
- **Kerangka HTML**
  - Syntax dibawah ini biasa disebut dengan kerangka bahasa pemrograman HTML. Didalam website selalu ada title untuk tiap-tiap web, untuk memasukkan title didalam web kamu harus mengetikkan diantara tag title (dapat diisikan dengan nama website kamu atau yang lainnya). Untuk memasukkan konten-konten, kamu dapat memasukkannya atau mengetikkannya didalam program tepat diantara tag body
 
``` 
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Belajar HTML</title>
  </head>
  <body>
    <h1>Hi.. I'm Sheha</h1>
    <h2> Track Back Ende Development </h2>
    <ol type="a">
      <li>Linkedin</li>
      <li>Twitter</li>
      <li>Instagram</li>
    </ol>
  </body>
</html> 
```
- **Tag HTML**
  Tag adalah sebuah penanda awalan dan akhiran dari sebuah elemen di HTML. Tag dibuat dengan kurung siku (<...>), lalu di dalamnya berisi nama tag dan kadang juga ditambahkan dengan atribut. Tag selalu ditulis berpasangan. Ada tag pembuka dan ada tag penutupnya. Namun, ada juga beberapa tag yang tidak memiliki pasangan penutup. Tag penutup ditulis dengan menambahkan garis miring (/) di depan nama tag.
``` Tag Pembuka <h1> Tag Penutup </h1> ```
    - **Single Tag**
    ``` contoh : </br> ```
    - **HTML Double Tag**
    ``` contoh : <p> </p> ```
    - **HTML Comment**
    ``` contoh : <!-- --> ```
    - **HTML Attributes** : properties dari sebuah element HTML
    ``` contohnya : id, class, name ```
- **Membuat Tabel**
``` <table border="1">
       <thead>
           <tr>
               <td>Nama</td>
               <td>Umur</td>
               <td>Jurusan</td>
           </tr>
       </thead>
       <tbody>
           <tr>
               <td>Sheha Annisa</td>
               <td>20 Tahun</td>
               <td>Teknik Informatika</td>
           </tr>
       </tbody>
   </table>
</html> 
```
  - **Penjelasan** :
  ``` - <thead> : membungkus konten bagian judul atau kepala tabel
      - <tr> : membuat baris pada tabel
      - <td> : membuat kolom di setiap baris pada tabel
      - <tbody> : membungkus konten bagian isi atau tubuh dari tabel 
  ```
### **----- CSS (_Cascading Style Sheets_) -----**

- **CSS** adalah bahasa yang digunakan untuk mendesain halaman website
- **Beberapa cara menyisipkan CSS kedalam HTML**

1. **Inline Styles** : menambahkan CSS pada atribute element HTML dengan menggunakan tag < style > pada file HTML
2. **Internal CSS** : menggunakan element < style > untuk menyisipkan kode CSS. Element < style > tersebut diletakkan di dalam element
3. **External CSS** : sebuah file CSS terpisah yang disambungkan dengan file HTML dengan menggunakan element < link >

- **Syntax Dasar CSS**
  - **Selektor**  :
  - Contoh : 
    ``` h1 {
          color: red;
      } ```
  **Selektor dapat berupa nama tag, class, id, dan atribut
  - Contoh :
  - **Selektor dengan nama tag
```
  h2 {
      color: blue
  } 
 ```
  - **Selektor dengan class
```
.bg-yellow {
      backgound-color: yellow;
  }
```
  - **Selektor dengan ID elemen
 ```
 #header {
      background: grey;
  }
```
   - **Selektor dengan Atribut
```
input[type=text]{
      background: yellow;
  } 
```
- **CSS Flexbox** adalah cara untuk mengatur layout, memiliki kemampuan untuk menyesuaikan layout secara otomatis

  - **Ordering & Orientation**

    - **flex-direction** : digunakan untuk mengatur letak item child
      ![1](https://css-tricks.com/wp-content/uploads/2018/10/flex-direction.svg)
      1. row (default): secara default letak item child membentuk sebuah baris dari kiri ke kanan.
      2. row-reverse: letak item child membentuk sebuah baris dari kanan ke kiri
      3. column: letak item child membentuk sebuah baris dari atas ke bawah
      4. column-reverse: letak item child membentuk sebuah baris dari bawah ke atas
    - **flex-wrap** : flex secara default akan membuat tata letak item children dalam 1 line saja. flex akan menyesuaikan space yang ada. Namun jika kamu ingin membatasi jumlah item children dalam 1 line lalu item children yang lain akan pindah ke posisi line yang baru, maka kita bisa menggunakan flex-wrap
      ![2](https://css-tricks.com/wp-content/uploads/2018/10/flex-wrap.svg)
      1. no-wrap (default): secara default , flex tidak menggunakan flex-wrap
      2. wrap: flex item akan memiliki beberapa line dari atas ke bawah jika space dalam 1 line sudah full width.
      3. wrap-reverse: kebalikan dari wrap yaitu flex item akan memiliki beberapa line dari bawah ke atas jika space dalam 1 line sudah full width
    - **flex-flow** : digunakan sebagai shortcut untuk set up flex-direction dan flex-wrap bersamaan
    - **order** : berfungsi untuk ordering item mana yang ingin kita atur posisinya berdasarkan urutan order
      ![3](https://css-tricks.com/wp-content/uploads/2018/10/order.svg)
      1. -1 : Item child yang di set order -1, maka item child tersebut akan berada di ordering paling awal atau paling kiri
      2. 0 (default) : Flex secara default memiliki order 0 pada setiap item child. Ini berarti 0 akan membuat item child sesuai urutan pada html
      3. 1: Item child yang di set order 1, maka item child tersebut akan berada di ordering paling akhir atau paling kanan

  - **Alignment**
    - **justify-content** digunakan untuk mengatur tata letak dan space antar item child secara horizontal atau main axis
      ![4](https://css-tricks.com/wp-content/uploads/2018/10/justify-content.svg)
    - **align-items** digunakan untuk mengatur align dari item child secara vertikal atau cross axis
      ![5](https://css-tricks.com/wp-content/uploads/2018/10/align-items.svg)
    - **align-self** digunakan untuk mengatur align item pada masing-masing item
      ![6](https://css-tricks.com/wp-content/uploads/2018/10/align-self.svg)
    - **align-content** properti align-content memiliki konsep yang sama seperti justify-content. align-content digunakan untuk mengatur tata letak dan space antar item child secara vertikal atau cross axis. align-content akan berjalan jika item lebih dari 1 line/baris. align-content memiliki value yang sama dengan justify-content. bedanya ada 1 tambahan value yaitu stretch
      ![6](https://css-tricks.com/wp-content/uploads/2018/10/align-content.svg)
  - **Flexibility**
    - **flex-grow** properti flex-grow dapat mengatur size suatu item child pada flexbox. Value dari properti flex-grow adalah number dan tidak boleh negatif
      ![7](https://css-tricks.com/wp-content/uploads/2018/10/flex-grow.svg)
    - **flex-shrink** flex-shrink adalah properti yang membuat size suatu item child mengecil secara relatif terhadap item child yang lainnya. value dari properti flex-shrink adalah number. Number negatif dianggap tidak valid. semakin besar value number dari properti ini, maka semakin kecil size dari suatu item child
    - **flex-basis** flex-basis adalah properti yang sama fungsinya seperti width. flex-basis mengatur width dari setiap item child. jika kita telah menggunakan width, maka flex-basis akan melakukan override properti width. Namun flex-basis tidak akan berjalan jika kita telah menggunakan min-width dan max-width.
      ![8](https://www.w3.org/TR/css-flexbox-1/images/rel-vs-abs-flex.svg)

### **----- Algoritma -----**

- **Algoritma** adalah langkah-langkah yang dilakukan untuk menyelesaikan masalah, sedangkan struktur data untuk mengelola/memanajemen sebuah data
- **Jenis Proses Algoritma**
  - Sequence : Instruksi yang dijalankan secara berurutan
  - Selection : Instruksi yang dijalankan jika memenuhi suatu kondisi
  - Iteration : Instruksi yang berulang kali dijalankan selama memenuhi suatu kondisi
  - Concurrent : Instruksi yang dijalankan secara bersamaan
- **Penyajian Algoritma**
  - Deskriptif
  - Flow Chart
  - PseudoCode adalah menuliskan algoritma dengan umumnya bahasa inggris sebelum kita implementasikan ke bahasa pemograman tertentu.
- **Big-O Notation** adalah sebuah cara atau metode untuk melakukan analisa terhadap sebuah algoritma pemrograman terhadap waktu eksekusi. Tentang seberapa efisien dan kompleksitas barisan kode dalam dimensi waktu

### **----- JavaScript -----**

1. **Intro to JavaScript**
   - Javascript dapat membuat website menjadi interaktif dan dinamis
   - Menjalankan JavaScript : Javascript dijalankan melalui browser pada device setiap user. misalnya chrome dan Mozilla firefox
   - Syntax dan Statement : menggunakan syntax tertentu untuk membuat statement program, instruksi untuk djalankan/dieksekusi oleh web browser, compiler, ataupun intrepreter
   - **Contoh Sytax JavaScript**
     - Alert()
     - Prompt()
     - Confirm()
     - Console.log
     - Console log juga tempat kita untuk melakukan debugging (mengetahui error pada code) pada pemograman web
   - **Tipe data** adalah klasifikasi yang kita berikan untuk berbagai macam data yang di gunakan dalam programing ada 6 yaitu
     - number
     - string
     - boolean
     - null
     - undefined
     - object
   - **Operator**.
     Assignment Operator (=). Assignment operator digunakan untuk menyimpan sebuah nilai pada variabel.
2. **Conditional**.
   Conditional digunakan saat dibutuhkan percabangan kasus. Komputer akan melakukan suatu tindakan jika suatu kondisi terpenuhi

   - If statement
   - If ... Else Statement
   - If ... Else if Statement
   - Truthy and Falsy : digunakan untuk mengecek apakah variabel telah terisi namun tidak mementingkan nilainya
   - Switch Case Conditional
     - Gunakan Switch case jika kondisi dan percabangan terlalu banyak
   - Ternary Operator : short-syntax dari statement if … else

3. **Looping**.
   Komputer dapat melakukan sebuah proses yang sama berulang-ulang. Jika membutuhkan perulangan dalam kasus tertentu, kita bisa menggunakan Looping.
   - **Manual Looping**
   - **for loop**. Gunakan FOR LOOP jika kita tahu seberapa banyak nilai pasti untuk pengulangannya. For loop akan terus berjalan selama kondisi ini terpenuhi. Selama kondisi bernilai TRUE
   - **While loop**. Gunakan WHILE LOOP jika kita tidak mengetahui jumlah pasti pengulangan. WHILE LOOP akan menjalankan instruksi pengulangan kondisi bernilai TRUE
   - **Do while**
   - **Nested Loop**. Jika kita membuat looping didalam looping. Maka ini dinamakan Nested Loop. Looping pertama dianalogikan sebagai baris. Looping kedua dianalogikan sebagai kolom
