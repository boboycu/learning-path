# JAVSRIPT CLIENT SIDE

Fungsi yang sering di pakai debuging

`Fungsi  alert() menampilkan pesan kepada pengguna dalam  dialog dengan  tombol OK`

`Fungsi  console.log() mencetak pesan ke konsol JavaScript browser Anda`

---

Dalam JavaScript, Anda perlu menghubungkan sendiri fungsi Anda. Pertama, tentukan fungsi di dalam `<script>` Anda:

```javascript
<script>
  function showMessage() {
    alert('Hello!');
  }
</script>
```

Contoh pengguna click button akan menampilkan Hello di popup window

```javascript
<!DOCTYPE html>
<html>
	<head>
	<title>JS Callback Functions</title>
	</head>
	<body>
		<p>Click this button:</p>
    <button onclick="showMessage()">
      Click me!
    </button>
		<script>
      function showMessage() {
        alert('Hello!');
      }
    </script>
	</body>
</html>
```

---

1.  Manipulasi DOM

pertama-tama tambahkan elemen HTML dengan atribut: id
Selanjutnya, di JavaScript Anda, panggil document.getElementById() fungsi tersebut dan berikan ID elemen HTML, dan simpan hasilnya dalam sebuah variabel:
Fungsi ini document.getElementById() mengembalikan Element objek yang menunjuk ke elemen HTML dengan ID tersebut. Sekarang Anda sudah memilikinya dalam sebuah variabel, Anda dapat mengubahnya menggunakan kode JavaScript.

> Catatan atribut bisa class atau id

```javascript
<!DOCTYPE html>
<html>
	<head>
		<title>JS Callback Functions</title>
	</head>
	<body>
		<p>Click this button:</p>
    <button onclick="showMessage()">
      Click me!
    </button>
    <p id="output"></p>
		<script>
      function showMessage() {
        let outputElement = document.getElementById('output');
        outputElement.innerText = 'Hello!';
      }
    </scrip>
	</body>
</html>
```

> // memasukan [Hello!] ke element:p id:output

---

```javascript
<!DOCTYPE html>
<html>
	<head>
		<title>Happy Coding</title>
	</head>
	<body>
		<p>Happy coding!</p>
		<script>
			document.write('Hello world!');
		</script>
	</body>
</html>
```

> // document.write('Hello world!'); akan menampilkan [Hello world!] ke layar

---

- Memasukkan inputan dari pengguna
  Anda bisa mendapatkan elemen input [value] yang berisi apa pun yang diketik pengguna:

```javascript
<!DOCTYPE html>
<html>
  <head>
    <title>JS Callback Functions</title>
  </head>
  <body>
    <p>Type your name and then click the button:</p>
    <input id="nameInput" />
    <button onclick="showMessage()">Click me!</button>
    <p id="output"></p>
    <script>
      function showMessage() {
        let nameInputElement = document.getElementById("nameInput");
        let name = nameInputElement.value;

        let outputElement = document.getElementById("output");
        outputElement.innerText = "Hello " + name + "!";
      }
    </script>
  </body>
</html>
```

> // outputElement.innerText = "Hello " + name + "!"; di sebut concatination ["Hello " + name + "!"] penggabungan string
