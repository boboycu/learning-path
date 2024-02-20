<link href="style.css" rel="stylesheet"></link>

# <center> Javascript [Source Learn](https://github.com/getify/You-Dont-Know-JS/tree/2nd-ed/get-started) </center>
tiga pilar bahasa JS: cakupan/penutupan, prototipe/objek, dan tipe/paksaan JS.

tiga pilar JS language: scope/cover, prototype/object, and type/compulsion  JS.

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
|for|untuk membuat sebuah loop dengan tiga bagian: inisialisasi, kondisi, dan ekspresi increment/decrement.|
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
|Note|   |
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

|Separators| |
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
Link source

[Perbandingan Kesetaraan Dan Kesamaan pdf
](./Equalty+Comparison+And+Sameness.pdf)

[Prioritas Operator Dalam Javascript pdf](./Operator+Precedence+In+Javascript.pdf)



-  Nilai-nilai.

Unit informasi yang paling mendasar dalam suatu program adalah nilai. Nilai adalah data. Begitulah cara program mempertahankan status. Nilai hadir dalam dua bentuk di JS: primitif dan objek.
```javascript
greeting("My name is Kyle.");
```
Dalam program ini, nilainya "My name is Kyle."adalah string literal primitif; string adalah kumpulan karakter yang diurutkan, biasanya digunakan untuk mewakili kata dan kalimat.
```javascript
//kutip ganda
console.log("My name is ${ firstName }.");
// My name is ${ firstName }.

//kutip satu
console.log('My name is ${ firstName }.');
// My name is ${ firstName }.

//kutip backtick
let firstName = `Kyle`
console.log(`My name is ${ firstName }.`);
// My name is Kyle.
```
Pendekatan yang lebih baik adalah dengan menggunakan (") atau (') (sekali lagi, pilih satu dan pertahankan!) untuk string kecuali Anda memerlukan interpolasi; cadangan `hanya untuk string yang akan menyertakan ekspresi yang diinterpolasi.

- Array.

Selain primitif, tipe nilai lain di JS adalah nilai objek.
array adalah tipe objek khusus yang terdiri dari daftar data yang diurutkan dan diindeks secara numerik:
```javascript
var names = [ "Frank", "Kyle", "Peter", "Susan" ];

console.log(names.length)// 4

console.log(names[0])// Frank

console.log(names[1])// Kyle
```
Array JS dapat menampung tipe nilai apa pun, baik primitif atau objek (termasuk array lainnya).

- Objek.

Objek lebih umum: kumpulan nilai yang beragam dan tidak berurutan. Dengan kata lain, Anda mengakses elemen dengan nama lokasi string (alias "kunci" atau "properti") dan bukan berdasarkan posisi numeriknya (seperti halnya array).
```javascript
var me = {
    first: "Kyle",
    last: "Simpson",
    age: 39,
    specialties: [ "JS", "Table Tennis" ]
};
console.log(`My name is ${ me.first }.`);// My name is Kyle
console.log(`My name is ${ me.specialties[0] }.`);//My name is JS

console.log(`My name is ${me["first"]}.`);// My name is Kyle
console.log(`My name is ${me["specialties"] [1] }.`);
//My name is Table Tennis.
```
Di sini, `me` memewakili suatu objek, dan `first` mewakili nama lokasi informasi dalam objek tersebut (kumpulan nilai). Opsi sintaksis lain yang mengakses informasi dalam suatu objek berdasarkan properti/kuncinya menggunakan tanda kurung siku [ ], seperti me["first"].

- Penentuan Jenis Nilai.

Untuk membedakan nilai, typeofoperator memberi tahu Anda tipe bawaannya, apakah primitif, atau "object"sebaliknya:
```javascript
typeof 42;                  // "number"
typeof "abc";               // "string"
typeof true;                // "boolean"
typeof undefined;           // "undefined"
typeof null;                // "object" -- oops, bug!
typeof { "a": 1 };          // "object"
typeof [1,2,3];             // "object"
typeof function hello(){};  // "function"
```
|  warning  |
| :------------: |
| typeof null sayangnya kembali "object" bukan yang diharapkan "null". Selain itu, typeof mengembalikan fungsi spesifik "function", tetapi bukan "array" array yang diharapkan. |

Mengonversi dari satu tipe nilai ke tipe nilai lainnya, seperti dari string ke angka, di JS disebut sebagai "paksaan".

Nilai primitif dan nilai objek berperilaku berbeda saat ditetapkan atau diedarkan.







