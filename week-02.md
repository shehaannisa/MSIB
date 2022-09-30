#### Sheha Luthfi Annisa | (Back-End Development)

# **Writing Web Development Basic Minggu 2**

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

   - Properties

     1. Constructor
        <br> Mengembalikan fungsi yang dibuat string prototipe objek
     2. Length
        <br> Mengembalikan panjang string JavaScript
        ```
        const str = 'skilvul';
        console.log(str.length); // Output: 7
        ```
     3. Prototype
        <br> Menambah metode dan properti ke dalam sebuah objek

   - Method
     1. charAt()
        <br> Mengembalikan karakter pada index yang spesifik (posisi)
        ```
        let hewan = 'Dinosaurus';
        console.log(hewan.charAt(4)); //Output : s
        ```
     2. indexOf()
        <br> Kembalikan posisi kemunculan pertama yang ditemukan dari teks yang ditentukan dalam sebuah string
        ```
        const str = 'saya sedang belajar javascript';
        console.log(str.indexOf('a')); // 1 :: s(a)ya ... 
        console.log(str.indexOf('ja')); // 16 :: ... bela(ja)r javascript
        ```
     3. lastIndexOf()
        <br> Kembalikan posisi kemunculan terakhir yang ditemukan dari teks yang ditentukan dalam sebuah string
        ```
        const str = 'saya sedang belajar javascript';
        console.log(str.lastIndexOf('a')); // 23 :: ... belajar jav(a)script
        console.log(str.lastIndexOf('ja')); // 20 :: ... belajar (ja)vascript
        console.log(str.lastIndexOf('ja', 19)); // 16 :: ... bela(ja)r javascript
        ```
     4. replace()
        <br> Cari string untuk nilai dan kembalikan string baru dengan nilai yang diganti
        ```
        const str = 'aku sedang belajar javascript';
        console.log(str.replace('aku', 'saya')); // saya sedang belajar javascript
        ```
     5. slice()
         <br> Ekstrak bagian dari string dan kembalikan string baru
         <br> Sintaks : slice(indeksAwal, indeksAkhir);
         ```
         const str = 'saya sedang belajar javascript';
         console.log(str.slice(5, 11)); // sedang
         console.log(str.slice(5)); // sedang belajar javascript
         ```
     6. split()
         <br> Memisahkan string ke dalam array substring
         <br> Sintaks : split(separator, limit);
         ```
         const str = 'saya sedang belajar javascript';
         console.log(str.split()); // ["saya sedang belajar javascript"]
         console.log(str.split(' ')); // ["saya", "sedang", "belajar", "javascript"]
         console.log(str.split(' ', 2)); //  ["saya", "sedang"]
         ```
     7. substring()
         <br> Ekstrak bagian dari string antara dua posisi yang ditentukan
         ```
         const str = 'saya sedang belajar javascript';
         console.log(str.substring(1, 3)); // ay
         console.log(str.substring(5)); // sedang belajar javascript
         ```
     8. toLowerCase()
         <br> Ubah string menjadi huruf kecil
         ```
         const str = 'Skilvul';
         console.log(str.toLowerCase()); //Output: skilvul
         ```
     9. toUpperCase()
         <br> Ubah string menjadi huruf besar
         ```
         const str = 'skilvul';
         console.log(str.toUpperCase()); //Output: SKILVUL
         ```
     10. trim()
         <br> Hapus spasi dari kedua ujung string
         ```
         const str = '     skilvul      ';
         console.log(str.trim()); // 'skilvul'
         ```
     11. includes()
         <br> mengembalikan nilai true or false apalah dalam variabel ada string tersebut
         ```
         let hewan = "Dinosaurus"
         console.log(hewan.includes("saur"); // Output : true
         ```     
2. **number** - bilangan bulat, pecahan, dan lain-lain yang berbentuk angka
   ```
   const a = 19;
   console.log(a); // 19
   console.log(typeof a); // number
   console.log(a instanceof Number); // false    
   ```
     - Properties (jarang digunakan, kebanyakan menggunakan methods number)
     - Methods
        1. isNan()
        <br> mengecek apakah ini bukan angka. Mengembalikan nilai Boolean, true jika nilai yang diuji NaN(bukan angka), false jika angka
        ```
        isNan("hallo") //true
        isNan(12345) //false, karena ini angka
        isNan(true) //false, karena boolean true dianggap sebagai 1, dan 1 itu termasuk angka
        isNan("12345") //false, karena ada angka didalam string
        ```
        2. toString()
        <br> untuk mengubah angka menjadi string
        ```
        let angka = 25
        angka.toString() //Output: '25'
        ```
        3. toFixed()
        <br> dapat menentukan jumlah angka dibelakang tanda koma. Return nilainya berupa string
        ```
        let pi = 3.14159265
        pi.toFixed() //Output: '3'
        pi.toFixed(1) //Output: '3.1'
        pi.toFixed(4) //Output: '3.1415'
        ```
        4. 
3. boolean - nilai benar dari sebuah pernyataan yang dituliskan sebagai true atau false
```

```
4. null - sebuah nilai yang berarti kosong atau menunjuk pada nilai yang tidak ada;
5. undefined - berbeda dari null, undefined menandakan kondisi variabel yang belum diberi sebuah nilai. Jadi pernyataan "nilai variabel itu adalah undefined" sebenarnya kurang tepat, sebab variabelnya memang tidak mempunyai sebuah nilai;
6. symbol - sebuah nilai unik yang dihasilkan tiap kali kita memanggil fungsi Symbol(). Nilai unik ini memiliki beberapa kegunaan seperti memberi nomor identifikasi unik dan berperan sebagai nama properti unik sebuah objek;

- Non Primitive

1. object - sebuah kumpulan pasangan properti dan nilai. Seperti objek dalam kehidupan sehari-hari saja. Misalnya objek Apel memiliki properti warna dengan nilai merah.
