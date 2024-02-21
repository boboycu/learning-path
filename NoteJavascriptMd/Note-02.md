<link href="style.css" rel="stylesheet"></link>

# <center>Link Javascript [Source Learn](https://hepunx.rl.ac.uk/~adye/jsspec11/jsrefspe.htm) </center>

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
