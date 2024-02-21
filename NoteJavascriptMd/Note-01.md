<link href="style.css" rel="stylesheet"></link>

# <center> Javascript [Source Learn](https://github.com/getify/You-Dont-Know-JS/tree/2nd-ed/get-started) </center>
Tiga pilar bahasa JS: cakupan/penutupan, prototipe/objek, dan tipe/paksaan JS.

Tiga pilar JS language: scope/cover, prototype/object, and type/compulsion  JS.

----------
Sumber berguna lainya.
1. [Perbandingan Kesetaraan Dan Kesamaan pdf
](./Equalty+Comparison+And+Sameness.pdf)

2. [Prioritas Operator Dalam Javascript pdf](./Operator+Precedence+In+Javascript.pdf)


----------
1. Keywords.

JavaScript memiliki berbagai kata kunci (keywords) yang memiliki peran dan fungsi tertentu dalam sintaksis dan struktur bahasa. Berikut adalah beberapa kata kunci JavaScript beserta penjelasannya:

|Keyword|Berguna |
|-------|----------|
|break|untuk menghentikan eksekusi loop atau switch statement.|
|case |dalam switch statement untuk memeriksa nilai yang sama dengan ekspresi switch.|
|catch  |bersamaan dengan try statement untuk menangkap kesalahan (error) yang terjadi dalam blok try. |
|continue |untuk melanjutkan ke iterasi berikutnya dalam loop. |
|const |untuk mendeklarasikan konstanta yang nilainya tidak dapat diubah setelah deklarasi. |
|class |untuk mendefinisikan sebuah kelas dalam JavaScript (fitur ES6). |
|debugger|Menyebabkan eksekusi JavaScript dihentikan dan menyisipkan titik henti (breakpoint) pada baris yang dieksekusi. |
|default|dalam switch statement sebagai nilai default jika tidak ada case yang sesuai.|
|delete|untuk menghapus properti dari objek.|
|do|Membuat sebuah loop yang akan terus berjalan selama kondisi yang diberikan tetap benar.|
|else|Digunakan dalam if statement untuk mengeksekusi blok kode jika kondisi yang diberikan adalah salah (false).|
|export|untuk mengekspor fungsi, objek, atau nilai dari sebuah modul.|
|extends|untuk membuat sebuah kelas yang merupakan turunan dari kelas lain (inheritance) (fitur ES6).|
|false| Mewakili nilai boolean false.|
|finally|bersamaan dengan try statement untuk menentukan blok kode yang akan selalu dieksekusi setelah blok try, terlepas dari hasilnya.|
|for|untuk membuat sebuah loop dengan Tiga bagian: inisialisasi, kondisi, dan ekspresi increment/decrement.|
|function|Digunakan untuk mendefinisikan sebuah fungsi.|
|if|untuk mengeksekusi blok kode jika kondisi yang diberikan adalah benar (true).|
|import| untuk mengimpor fungsi, objek, atau nilai dari sebuah modul.|
|in|untuk memeriksa apakah properti tertentu ada dalam objek yang diberikan.|
|instanceof|untuk memeriksa apakah sebuah objek merupakan instance dari kelas tertentu.|
|new|untuk membuat instance dari sebuah objek atau kelas.|
|null| Mewakili nilai null.|    
|return| Digunakan untuk mengembalikan nilai dari sebuah fungsi.|
|super| Digunakan untuk mengakses fungsi dari kelas induk dalam kelas turunan (fitur ES6).|
|switch| Digunakan untuk memilih salah satu dari banyak blok kode yang akan dieksekusi.|
|this| Digunakan untuk merujuk pada objek saat ini.|
|throw| Digunakan untuk melempar sebuah eksepsi (exception).|
|true| Mewakili nilai boolean true.|
|try| Digunakan untuk menguji blok kode untuk kesalahan.|
|typeof| Digunakan untuk mengembalikan tipe data dari suatu variabel.|
|var| Digunakan untuk mendeklarasikan variabel (fitur lama, direkomendasikan untuk menggunakan let atau const).|
|void| Digunakan untuk mengindikasikan bahwa sebuah ekspresi tidak mengembalikan nilai.|
|while| Digunakan untuk membuat sebuah loop yang akan terus berjalan selama kondisi yang diberikan tetap benar.|
-----
2. Reserved Words dalam JavaScript

Reserved Words dalam JavaScript adalah kata kunci yang telah dipesan untuk digunakan dalam bahasa itu sendiri. Kata kunci ini tidak dapat digunakan sebagai nama variabel, fungsi, atau label dalam program JavaScript karena mereka memiliki peran atau makna khusus dalam sintaks dan struktur bahasa.

Berikut adalah daftar Reserved Words dalam JavaScript:
|Reserved Words|    |
|-------|-----|
|Keyword literals|   true, false, null|
|Primitive types|    undefined|
|Control flow|      if, else, switch, case, default, while, do, for, break, continue, return|
|Functions and classes|   function, class, constructor, extends, super|
|Try statement|       try, catch, finally, throw|
|Module import/export|    import, export, default|
|Miscellaneous|           this, typeof, instanceof, new, delete, void, in, with|

----------
3. Identifiers.

Case Sensitivity: JavaScript bersifat case sensitive, artinya huruf besar (uppercase) dan huruf kecil (lowercase) dianggap berbeda.
|Note| Keterangan |
|:-------|:----------|
|Penulisan | Identifiers dapat terdiri dari huruf (a-z, A-Z), angka (0-9), garis bawah (_) atau dollar ($). Contoh: namaVariabel, _nilai, $_variabel1.|
|Penggunaan Pertama| Identifiers tidak boleh dimulai dengan angka atau karakter khusus, kecuali garis bawah (_) atau dollar ($). Contoh yang valid: _nilai, $_variabel1, namaVariabel.|
|Kata Kunci| Identifiers tidak boleh menggunakan kata kunci atau reserved words dalam JavaScript sebagai nama. Contoh: var, function, if, else, dll.|
|Case Sensitivity| JavaScript bersifat case sensitive, artinya huruf besar (uppercase) dan huruf kecil (lowercase) dianggap berbeda. Contoh: namaVariabel dan namavariabel dianggap berbeda.|
|Pendekatan Penamaan| Disarankan untuk menggunakan pendekatan camelCase dalam penamaan identifiers, di mana huruf pertama dari setiap kata kecuali yang pertama ditulis dengan huruf kapital. Contoh: namaDepan, namaBelakang, alamatRumah.|
|Resolusi Unicode| JavaScript memungkinkan penggunaan karakter Unicode dalam identifiers. Namun, untuk konsistensi dan keterbacaan, sebaiknya gunakan karakter ASCII.|

Contoh penulisan identifiers yang valid dalam JavaScript:
```javascript
var namaVariabel;
var _nilai;
var $_variabel1;
var namaDepan;
var namaBelakang;
var alamatRumah;

```
------

4. Separators di javascript.

separators digunakan untuk memisahkan elemen-elemen dalam kode untuk membuatnya lebih mudah dibaca dan dipahami. 
Berikut adalah beberapa separator yang umum digunakan dalam JavaScript:

|Separators| Penggunaan|
|---------|---------|
|Semicolon( ; )| Digunakan sebagai terminator untuk statement. Meskipun JavaScript menggunakan automatic semicolon insertion (ASI) untuk menambahkan titik koma secara otomatis dalam beberapa kasus, disarankan untuk selalu menggunakan titik koma secara eksplisit.|
|Curly Braces ( { } )| Digunakan untuk menandai awal dan akhir dari blok kode. Blok kode digunakan dalam struktur kendali seperti ` if, else, for, while,` dan untuk membuat objek literal.|
|Parentheses ( ( ) )| Digunakan untuk menandai awal dan akhir dari parameter dalam deklarasi fungsi, untuk mengelompokkan ekspresi, dan untuk memanggil fungsi.|
|Square Brackets ( [ ] )| Digunakan untuk membuat array literal, mengakses elemen dalam array, dan untuk membuat properti dinamis dalam objek.|
|Colon ( : )| Digunakan dalam objek literal untuk memisahkan nama properti dan nilai, dan juga dalam operator ternary (condition ? expr1 : expr2) untuk menentukan ekspresi yang akan dievaluasi berdasarkan kondisi.|
|Dot (  .  )| Digunakan untuk mengakses properti dari objek. Contoh: object.property.|
|Comma (,)| Digunakan untuk memisahkan beberapa ekspresi atau deklarasi dalam satu statement. Contoh penggunaan:  `var x = 1, y = 2, z = 3;`|
|Backslash ( \ )| Digunakan sebagai escape character untuk escape sequences dalam string literals|
-------
5. Escape Sequences for String Literals.

cara untuk menyisipkan karakter khusus ke dalam string dalam JavaScript. Karakter khusus ini tidak dapat dituliskan langsung dalam string karena mereka memiliki arti khusus dalam sintaks JavaScript. Untuk menyertakan karakter ini dalam string, Anda perlu menggunakan escape sequence yang dimulai dengan karakter backslash ( \ ).

1. \ ' : Menyisipkan karakter single quote (').
2. \ " : Menyisipkan karakter double quote (").
3. \\  : Menyisipkan karakter backslash ().
4. \n  : Menyisipkan karakter newline (baris baru).
5. \r  : Menyisipkan karakter carriage return.
6. \t  : Menyisipkan karakter tab.
7. \b  : Menyisipkan karakter backspace.
8. \f  : Menyisipkan karakter form feed.

Contoh penggunaan escape sequences dalam string:
```javascript
var str = 'Ini adalah string dengan newline\nIni baris baru';
var str2 = "Ini adalah string dengan tab\tIni teks setelah tab";
var str3 = 'String dengan single quote \' dalamnya';
var str4 = "String dengan double quote \" dalamnya";
var str5 = 'C:\\Users\\User\\Documents\\File.txt'; // Path file Windows
var strBacktick = `Ini adalah string dengan newline backtick\nIni baris baru`;
console.log(strBacktick);
//Ini adalah string dengan newline backtick
// Ini baris baru
console.log(str);
//Ini adalah string dengan newline
// Ini baris baru
console.log(str2);
// Ini adalah string dengan tab   Ini teks setelah tab
console.log(str3);
// String dengan single quote ' dalamnya
console.log(str4);
// String dengan double quote ' dalamnya
console.log(str5);
//C:\Users\User\Documents\File.txt
```
- Literals: Literal adalah nilai yang ditulis secara langsung ke dalam kode. Contoh:
```javascript
String literal: 'Hello, world!'
Numeric literal: 42
Boolean literal: true atau false
Array literal: [1, 2, 3]
Object literal: {key: 'value'}
```
- literal titik mengambang (floating-point literals).

adalah representasi literal untuk nilai-nilai bilangan desimal. Literal ini digunakan untuk merepresentasikan angka dengan desimal, seperti 3.14 atau -0.001. Literal titik mengambang dapat ditulis dalam notasi desimal atau eksponensial.

Contoh literal titik mengambang dalam JavaScript:
```javascript
//Notasi Desimal
var pi = 3.14;
var harga = 99.99;

// Notasi Eksponensial (Notasi Ilmiah):
var jarak = 1.2e6; // 1.2 x 10^6 = 1200000
var kecepatan = 3e8; // 3 x 10^8 = 300000000

```
Dalam notasi eksponensial, "e" digunakan untuk menunjukkan pangkat 10. Sebagai contoh, 1.2e6 berarti 1.2 dikalikan dengan 10 pangkat 6.

Penting untuk diingat bahwa literal titik mengambang dalam JavaScript merupakan representasi yang mendekati nilai sebenarnya dan memiliki keterbatasan dalam presisi, terutama ketika melakukan operasi matematika yang kompleks.

- Literal null dalam JavaScript.

digunakan untuk merepresentasikan nilai kosong atau non-ada. Ini berbeda dengan `undefined`, yang menunjukkan bahwa suatu variabel belum diberikan nilai. Ketika suatu variabel atau ekspresi memiliki nilai `null`, itu berarti variabel atau ekspresi tersebut secara eksplisit diberikan nilai kosong.

Contoh penggunaan literal null dalam JavaScript:
```javascript
var data = null;
console.log(data); // Output: null

var obj = {
    name: 'John',
    age: null
};
console.log(obj.age); // Output: null
```
Nilai `null` digunakan ketika Anda ingin menyatakan bahwa suatu variabel atau properti tidak memiliki nilai atau tidak valid. Ini dapat digunakan untuk membersihkan referensi ke objek atau nilai sebelumnya.

Perlu diingat bahwa `null` adalah tipe data sendiri dalam JavaScript (yaitu, bukan objek atau array), dan digunakan untuk menyatakan "tidak ada nilai". Ini juga dapat digunakan dalam perbandingan atau pengecekan kondisi untuk menunjukkan bahwa suatu nilai tidak ada atau kosong.

---------
6. Types, Values, and Variables/Jenis, Nilai, dan Variabel.

- type primitif.
String,Number,Boolean,Null,Undefine.

Nilai-nilai dari tipe data primitif ini bersifat immutable (tidak dapat diubah). Ketika Anda mengubah nilai dari variabel dengan tipe data primitif, sebenarnya Anda membuat variabel baru dengan nilai yang baru.

-------

Type/jenis cek menggunakan Operator typeof dalam JavaScript digunakan untuk mengembalikan tipe data dari suatu operan dalam bentuk string. Operator ini berguna untuk memeriksa tipe data dari suatu nilai atau variabel.

Contoh penggunaan operator typeof:
```javascript
var nilai = 42;
console.log(typeof nilai); // Output: "number"

var nama = "John";
console.log(typeof nama); // Output: "string"

var benar = true;
console.log(typeof benar); // Output: "boolean"

var kosong = null;
console.log(typeof kosong); // Output: "object" (ini adalah keanehan dalam JavaScript, null seharusnya memiliki tipe "null")

var tidakTerdefinisi;
console.log(typeof tidakTerdefinisi); // Output: "undefined"

var fungsi = function() {};
console.log(typeof fungsi); // Output: "function"

var array = [1, 2, 3];
console.log(typeof array); // Output: "object"

var obJect = {'hai':'hu'};
console.log(typeof obJect);// Output: "object"
```
Perlu diperhatikan bahwa ada beberapa keanehan dalam penggunaan operator typeof:

typeof null mengembalikan "object", padahal seharusnya mengembalikan "null".

 Ini adalah kekurangan dari implementasi awal JavaScript dan tetap dipertahankan untuk menjaga kompatibilitas dengan kode lama.

typeof array mengembalikan "object", karena dalam JavaScript, array dianggap sebagai jenis khusus dari objek. Namun, kita bisa menggunakan metode Array.isArray() untuk memeriksa apakah suatu variabel adalah array.

Meskipun memiliki beberapa keanehan, operator typeof sangat berguna dalam pemrograman JavaScript untuk melakukan pengecekan tipe data sebelum melakukan operasi tertentu terhadap variabel atau nilai.

- Type konversi.

Terdapat dua jenis konversi data yang sering digunakan: konversi tipe data eksplisit (explicit type conversion) dan konversi tipe data implisit (implicit type conversion).

1. Konversi Tipe Data Eksplisit (Explicit Type Conversion atau Type Casting):

Dilakukan secara manual dengan menggunakan fungsi atau metode yang disediakan JavaScript, seperti `Number()`, `String()`, atau `Boolean()`.

```javascript
var x = "10"; // string
var y = Number(x); // konversi ke number
console.log(y); // Output: 10
```
2. Konversi Tipe Data Implisit (Implicit Type Conversion atau Coercion):

Dilakukan secara otomatis oleh JavaScript saat terjadi operasi antara tipe data yang berbeda.
```javascript
var x = "10"; // string
var y = 5; // number
var z = x + y; // string + number -> operasi ini akan mengubah nilai y menjadi string dan hasilnya adalah string "105"
console.log(z); // Output: "105"
```
Konversi tipe data implisit dapat berguna dalam beberapa kasus, tetapi juga dapat menyebabkan kebingungan atau bug dalam kode jika tidak diperhatikan dengan baik. Sebaiknya gunakan konversi tipe data eksplisit ketika Anda ingin mengontrol proses konversi dengan jelas.
|Note|
|----|
|Penting di ingat inputan dari form browser selalu bertype string walaupun kita input angka `10`|

Dalam JavaScript, "Type Conversion" mengacu pada proses mengubah nilai dari satu tipe data ke tipe data lain. Terdapat beberapa fungsi bawaan (built-in functions) yang dapat digunakan untuk melakukan konversi tipe data, tergantung pada tipe data yang ingin dikonversi. Berikut adalah penjelasan singkat tentang fungsi konversi untuk masing-masing tipe data:

- Function:

Number(): Mengonversi nilai menjadi tipe data number.

String(): Mengonversi nilai menjadi tipe data string.

Boolean(): Mengonversi nilai menjadi tipe data boolean.
```javascript
var x = "10";
var y = Number(x); // y = 10 (number)
var z = String(y); // z = "10" (string)
var a = Boolean(x); // a = true (boolean)

// Object() atau kurung kurawal {}: Membuat objek dari nilai tertentu.
var obj = Object("Hello"); // obj = { "0": "H", "1": "e", "2": "l", "3": "l", "4": "o" }
```
- Number:
parseInt(): Mengonversi string menjadi bilangan bulat (integer).

parseFloat(): Mengonversi string menjadi bilangan desimal (floating-point).
```javascript
var x = "10.5";
var y = parseInt(x); // y = 10 (integer)
var z = parseFloat(x); // z = 10.5 (float)

```
- Boolean:
Boolean(): Mengonversi nilai menjadi tipe data boolean.

type Bolean javascript 0 false 1 true. 
```javascript
var x = 0;
var y = Boolean(x); // y = false
console.log(y)
var x = 1;
var y = Boolean(x); // y = true
console.log(y)
```
- String:
String(): Mengonversi nilai menjadi tipe data string.
```javascript
var x = 10;
var y = String(x); // y = "10"

```
Dengan menggunakan fungsi konversi ini, Anda dapat dengan mudah mengubah tipe data dari nilai-nilai JavaScript sesuai kebutuhan Anda dalam program.

- String Types and Operations/Jenis dan Operasi String.

Di JavaScript, tipe data string digunakan untuk merepresentasikan teks. String dapat berisi satu karakter atau lebih, dan dapat dibuat dengan mengapit teks dengan tanda kutip tunggal (') atau tanda kutip ganda (").

```javascript
var namaDepan = "John";
var namaBelakang = "Doe";
var namaLengkap = namaDepan + " " + namaBelakang; // Penggabungan string
console.log(namaLengkap); // Output: "John Doe"

var panjangNama = namaLengkap.length; // Panjang string
console.log(panjangNama); // Output: 8

var karakterPertama = namaLengkap[0]; // Karakter pertama
console.log(karakterPertama); // Output: "J"

var indexSpasi = namaLengkap.indexOf(" "); // Posisi spasi
console.log(indexSpasi); // Output: 4

var belakang = namaLengkap.substring(indexSpasi + 1); // Substring
console.log(belakang); // Output: "Doe"
```
JavaScript memiliki banyak metode bawaan untuk memanipulasi string, seperti toUpperCase() untuk mengubah string menjadi huruf besar, toLowerCase() untuk mengubah string menjadi huruf kecil, dan split() untuk memisahkan string menjadi array berdasarkan separator tertentu.