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

   - Properti

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
     2. charCodeAt()
        <br> Mengembalikan unicode karakter pada indeks yang ditentukan
     3. concat()
        <br> Menggabungkan satu atau beberapa string dan kembalikan salinan string yang digabungkan
     4. fromCharCode()
        <br> Ubah nilai unicode menjadi karakter
     5. indexOf()
        <br> Kembalikan posisi kemunculan pertama yang ditemukan dari teks yang ditentukan dalam sebuah string
        ```
        const str = 'saya sedang belajar javascript';
        console.log(str.indexOf('a')); // 1 :: s(a)ya ... 
        console.log(str.indexOf('ja')); // 16 :: ... bela(ja)r javascript
        ```
     6. lastIndexOf()
        <br> Kembalikan posisi kemunculan terakhir yang ditemukan dari teks yang ditentukan dalam sebuah string
        ```
        const str = 'saya sedang belajar javascript';
        console.log(str.lastIndexOf('a')); // 23 :: ... belajar jav(a)script
        console.log(str.lastIndexOf('ja')); // 20 :: ... belajar (ja)vascript
        console.log(str.lastIndexOf('ja', 19)); // 16 :: ... bela(ja)r javascript
        ```
     7. localeCompare()
        <br> Bandingkan dua string di lokal saat ini
     8. match()
        <br> Cari string untuk kecocokan dengan ekspresi reguler, dan kembalikan kecocokan
     9. replace()
        <br> Cari string untuk nilai dan kembalikan string baru dengan nilai yang diganti
        ```
        const str = 'aku sedang belajar javascript';
        console.log(str.replace('aku', 'saya')); // saya sedang belajar javascript
        ```
     10. search()
         <br> Cari string untuk nilai dan kembalikan posisi kecocokan
     11. slice()
         <br> Ekstrak bagian dari string dan kembalikan string baru
         <br> Sintaks : slice(indeksAwal, indeksAkhir);
         ```
         const str = 'saya sedang belajar javascript';
         console.log(str.slice(5, 11)); // sedang
         console.log(str.slice(5)); // sedang belajar javascript
         ```
     12. split()
         <br> Memisahkan string ke dalam array substring
         <br> Sintaks : split(separator, limit);
         ```
         const str = 'saya sedang belajar javascript';
         console.log(str.split()); // ["saya sedang belajar javascript"]
         console.log(str.split(' ')); // ["saya", "sedang", "belajar", "javascript"]
         console.log(str.split(' ', 2)); //  ["saya", "sedang"]
         ```
     13. substr()
         <br> Ekstrak bagian dari string mulai dari indeks tertentu melalui sejumlah karakter tertentu
     14. substring()
         <br> Ekstrak bagian dari string antara dua posisi yang ditentukan
         ```
         const str = 'saya sedang belajar javascript';
         console.log(str.substring(1, 3)); // ay
         console.log(str.substring(5)); // sedang belajar javascript
         ```
     15. toLocaleLowerCase()
         <br> Ubah string menjadi huruf kecil, sesuai dengan lokal host
     16. toLocaleUpperCase()
         <br> Ubah string menjadi huruf besar, sesuai dengan lokal host
     17. toLowerCase()
         <br> Ubah string menjadi huruf kecil
         ```
         const str = 'Skilvul';
         console.log(str.toLowerCase()); //Output: skilvul
         ```
     18. toString()
         <br> Kembalikan nilai objek string
     19. toUpperCase()
         <br> Ubah string menjadi huruf besar
         ```
         const str = 'skilvul';
         console.log(str.toUpperCase()); //Output: SKILVUL
         ```
     20. trim()
         <br> Hapus spasi dari kedua ujung string
         ```
         const str = '     skilvul      ';
         console.log(str.trim()); // "skilvul"
         ```
     21. valueOf()
         <br> Kembalikan nilai primitif objek string

2. **number** - bilangan bulat, pecahan, dan lain-lain yang berbentuk angka
```
const a = 19;
console.log(a); // 19
console.log(typeof a); // number
console.log(a instanceof Number); // false    
```
   - Method Number
     1. toExponential()
        <br> mengonversi angka ke notasi eksponensial dan mengembalikannya sebagai string
        ```
        (2).toExponential(3); // 2.000e+0
        ```
     2. 
3. boolean - nilai benar dari sebuah pernyataan yang dituliskan sebagai true atau false
```

```
4. null - sebuah nilai yang berarti kosong atau menunjuk pada nilai yang tidak ada;
5. undefined - berbeda dari null, undefined menandakan kondisi variabel yang belum diberi sebuah nilai. Jadi pernyataan "nilai variabel itu adalah undefined" sebenarnya kurang tepat, sebab variabelnya memang tidak mempunyai sebuah nilai;
6. symbol - sebuah nilai unik yang dihasilkan tiap kali kita memanggil fungsi Symbol(). Nilai unik ini memiliki beberapa kegunaan seperti memberi nomor identifikasi unik dan berperan sebagai nama properti unik sebuah objek;

- Non Primitive

1. object - sebuah kumpulan pasangan properti dan nilai. Seperti objek dalam kehidupan sehari-hari saja. Misalnya objek Apel memiliki properti warna dengan nilai merah.
