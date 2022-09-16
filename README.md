# Writing-and-Presentation-3
Javascript Intermediate

## Javascript Array
Array merupakan wadah pengorganisasian dan tempat penyimpanan data. array juga merupakan variabel yang memiliki banyak data. array dapat digolongkan sebagai tipe data yang dapat menyimpan tipe data apapun didalamnya seperti tipe data number, string boolean dll. array yang demikian hanya berlaku pada bahasa pemograman javascript. 

- cara mendeklarasikan erray di js.

let arrayData = [1, 2, 3, 4, 5]

- cara memanggil/akses data di array. (data pertama di array dimulai dari index ke 0).

1.  Memanggil 1 data di dalam array

let kota = ['Sumbawa', 'Mataram', 'Bogor'];

   console.log (kota[0]) -------> maka index 0 akan menampilkan Sumbawa
   
2.  memanggil seluruh data array

let kota = ['Sumbawa', 'Mataram', 'Bogor'];

   console.log (kota)
   
- update array bisa jamak dan tunggal.

// update data tunggal

kota[0]= 'Malang'
console.log(kota[0]);

// update data jamak

kota=['Malang', 'Manado', 'Makassar', 'Kalimantan']
console.log('sesudah di update', kota)

//array yang didefinisikan dengan const tidak akan bisa diupdate dikarenakan data bersifat mutlak.

//array properties. array memiliki 5 properties (constructor, length, index, input dan prototype). pembahasan pertemuan kali ini tentang length untuk melihat atau menghitung berapa length pada array tersebut. penggunaannyya menggunakan .length. contoh:

cara melihat jumlah array dari suatu variable array.

.length

let panjangarrayData = kota.length

console.log("jumlah data array", panjangarrayData)

// array memiliki method yang disebut built-in methods untuk memudahkan progremer saat memanipulasi suatu data. contoh built-in method dari array sebagai berikut:
1.  .push() memiliki kemampuan mengubah data secara global atau keseluruhan, baik data sebelum maupun sesudah update. push berguna untuk menambah data array.

let dara =["A", "B", "C", "D"]

console.log("sebelum di push", data)

data.push("H")

console.log("sesudah di push", data)

2.  .pop() merupakan method yang menghapus data array terakhir.

3.  .shift() merupakan pengambilan data diurutan awal. contohnya:

let antrianMinyak = [];

antrianMinyak.push("Agus");

antrianMinyak.push("Asep");

antrianMinyak.push("Didin");

antrianMinyak.push("Dede");

antrianMinyak.push("Siti");

console.log(antrianMinyak);


// Contoh Shift:
console.log(antrianMinyak.shift());


// Contoh Unshift (method untuk menambahkan data diurutan depan.)

antrianMinyak.unshift("Ujang");


// Contoh Sort (untuk membuat data berurutan)

let number = [1, 45, 0, -2, 29, 11];

console.log(number);

console.log(number.sort());


// Perulangan Array menggunakan Foreach
// Tidak memiliki nilai balikan atau return

antrianMinyak.forEach((item, index) => {

  antrianMinyak[index] = item + " " + index;
  
});

console.log(antrianMinyak);


// Perulangan Array menggunakan Map

let antrianMinyakAsep = antrianMinyak.map((item) => {

  if (item === "Asep") {
  
    return true;
    
  } else {
  
    return false;
    
  }

});

console.log(antrianMinyakAsep);
