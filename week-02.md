#### Sheha Luthfi Annisa | (Back-End Development)

# **Writing Web Development Basic Minggu 1**

## **Javascript Dasar - Scope and FunctionJavaScript**

- ### SCOPE
  Scope adalah konsep dalam flow data variabel.
  Menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.
  Analoginya seperti ini:
  Kita semua bisa melihat bintang-bintang dilangit karena bumi bersifat global.
  Namun jika kamu tinggal di Bandung, kamu tidak akan bisa melihat monas yang berada di jakarta. Monas bersifat local yaitu hanya berada di Jakarta.

### Blocks

Blocks adalah code yang berada didalam curly braces {}.
Conditional, function, dan looping menggunakan blocks.

### Global Scope

Global scope berarti variabel yang kita buat dapat diakses dimanapun dalam suatu file.
Agar menjadi Global Scope, suatu variabel harus dideklarasikan diluar Blocks.
![nama bebas](https://github.com/Adimas88888/MSIB/blob/7581cff4245260d9ba8ef047773ec69d84f3c451/Screenshot_43.png)

### Local

Local scope berarti kita mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping.
Maka variabel hanya bisa diakses didalam blocks saja. Tidak bisa diakses diluar blocks.

![nama bebas](https://github.com/Adimas88888/MSIB/blob/7581cff4245260d9ba8ef047773ec69d84f3c451/Screenshot_44.png)

### JAVASCRIPT - FUNCTION

Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur.

- ## Membuat Function

- ## Memanggil Function

- ## Parameter dan Argumen
- Dengan parameter, function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas.
- Saat membuat function/fitur, kita harus tahu data-data yang dibutuhkan.
- Misalnya saat membuat function penambahan 2 buah nilai. Data yang dibutuhkan adalah 2 buah nilai tersebut.
- Argumen adalah nilai yang digunakan saat memanggil function.
- Jumlah argumen harus sama dengan jumlah parameternya
  Jadi jika di function penambahan ada 2 parameter nilai saat membuat function.
- Saat memanggil function kita gunakan 2 buah nilai argumen.

- ## Function Helper

  Kita bisa menggunakan function yang sudah dibuat pada function lain.

- ## Arrow Function
  Arrow function adalah cara lain menuliskan function. Ini adalah fitur terbaru yang ada pada ES6 (Javascript Version)

## **Javascript Dasar - Data Type Built in Prototype and Method**

### Data Type

- Data Primitive

1. **string** - deretan karakter yang diapit oleh sepasang tanda kutip (" ")
   <br> berguna untuk menyimpan data yang dapat direpresentasikan dalam bentuk teks

   - Properti

     1. Constructor
        <br> Mengembalikan fungsi yang dibuat string prototipe objek
     2. Length
        <br> Mengembalikan panjang string JavaScript

        ```
        const str = 'Skilvul Back End Development. Total kata:';
        console.log(`${str} ${str.length}`);
        // expected output: "Skilvul Back End Development. Total kata: 42"

        ```

     3. Prototype
        <br> Menambah metode dan properti ke dalam sebuah objek

   - Method
     1. charAt()
        <br> Mengembalikan karakter pada index yang spesifik (posisi)
     2. charCodeAt()
        <br> Mengembalikan unicode karakter pada indeks yang ditentukan
     3. concat()
        <br> Menggabungkan satu atau beberapa string dan kembalikan salinan string yang digabungkan
     4. fromCharCode()
        <br> Ubah nilai unicode menjadi karakter
     5. indexOf()
        <br> Kembalikan posisi kemunculan pertama yang ditemukan dari teks yang ditentukan dalam sebuah string
     6. lastIndexOf()
        <br> Kembalikan posisi kemunculan terakhir yang ditemukan dari teks yang ditentukan dalam sebuah string
     7. localeCompare()
        <br> Bandingkan dua string di lokal saat ini
     8. match()
        <br> Cari string untuk kecocokan dengan ekspresi reguler, dan kembalikan kecocokan
     9. replace()
        <br> Cari string untuk nilai dan kembalikan string baru dengan nilai yang diganti
     10. search()
         <br> Cari string untuk nilai dan kembalikan posisi kecocokan
     11. slice()
         <br> Ekstrak bagian dari string dan kembalikan string baru
     12. split()
         <br> Pisahkan string ke dalam array substring
     13. substr()
         <br> Ekstrak bagian dari string mulai dari indeks tertentu melalui sejumlah karakter tertentu
     14. substring()
         <br> Ekstrak bagian dari string antara dua posisi yang ditentukan
     15. toLocaleLowerCase()
         <br> Ubah string menjadi huruf kecil, sesuai dengan lokal host
     16. toLocaleUpperCase()
         <br> Ubah string menjadi huruf besar, sesuai dengan lokal host
     17. toLowerCase()
         <br> Ubah string menjadi huruf kecil
     18. toString()
         <br> Kembalikan nilai objek string
     19. toUpperCase()
         <br> Ubah string menjadi huruf besar
     20. trim()
         <br> Hapus spasi dari kedua ujung string
     21. valueOf()
         <br> Kembalikan nilai primitif objek string

2. number - bilangan bulat, pecahan, dan lain-lain;
3. boolean - nilai benar dari sebuah pernyataan yang dituliskan sebagai true atau false;
4. null - sebuah nilai yang berarti kosong atau menunjuk pada nilai yang tidak ada;
5. undefined - berbeda dari null, undefined menandakan kondisi variabel yang belum diberi sebuah nilai. Jadi pernyataan "nilai variabel itu adalah undefined" sebenarnya kurang tepat, sebab variabelnya memang tidak mempunyai sebuah nilai;
6. symbol - sebuah nilai unik yang dihasilkan tiap kali kita memanggil fungsi Symbol(). Nilai unik ini memiliki beberapa kegunaan seperti memberi nomor identifikasi unik dan berperan sebagai nama properti unik sebuah objek;

- Non Primitive

1. object - sebuah kumpulan pasangan properti dan nilai. Seperti objek dalam kehidupan sehari-hari saja. Misalnya objek Apel memiliki properti warna dengan nilai merah.
