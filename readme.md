# Asynchronus

## Fetch
Sebuah API modern yang bertugas mengambil tugas secara asynchronus

alat komunikasi yang digunakan frontend dengan backend biasanya disebut dengan **HTTP REQUEST**

Berikut ini merupakan method dari HTTP request
- Get : Mengambil data
- Post : Mengirim data
- Put : Memperbaharui suatu data
- delete : menghapus data


contoh pengunaan fetch http request dari alamat ("https://pokeapi.co/api/v2/pokemon/pikachu/) dengan menggunakan method "get"


    fetch("https://pokeapi.co/api/v2/pokemon/pikachu/", {
     method: "GET"
    })
    .then((response) => {
    return response.json();
    })
    .then((data) => {
    console.log(data);
    })
    .catch((error) => {
     console.log(error);
    });


contoh penggunaan fetch http request dari alamat ("https://pokeapi.co/api/v2/pokemon/pikachu/) dengan menggunakan method "delete"


    fetch("https://pokeapi.co/api/v2/pokemon/pikachu/", {
     method: "DELETE"
    })
    .then((response) => {
    return response.json();
    })
    .then((data) => {
    console.log(data);
    })
    .catch((error) => {
     console.log(error);
    });


# RESPONSIVE WEB DESIGN

- Responsive Web Desin yaitu suatu tampilan website yang dapat menyesuikan dengan perangkat yang digunakan seperti laptop,pc maupun handpone.

- Tools yang biasa digunakan untuk membuat sebuah web lebih responsive ialah **Chrome Dev Tools**. Chrome Dev Tools sendiri merupakan tools dar google chrome yang digunakan sebagai tools Responsive Web Design.

- Untuk membuat suatu gambar pada halaman website agar menjadi responsive dapat dilakukan dengan menambahkan atribut **Max - width = 100%** pada bagian gambar di file css

- Penggunaan media query yang umum digunakan adalah min-width dan max-width

Contoh breakpoint dapat ditulis seperti ini

    @media screen and (min-width: 520px) and (max-width: 1000px) {
    body {
    background-color: red 
     }
    }

- Cara mengkondisikan Media Query ada 2 cara yaitu:
1. Memisahkan beberapa file css sesuai dengan tampilan device yang ingin dibuat
2. Menggabungkan semua styling css device menjadi 1

# BOOSTRAP

- **Bootstrap** adalah sebuah framework HTML, CSS, dan JavaScript yang berfokus untuk menyederhanakan pengembangan halaman web atau website. 

- Pada umumnya, *Bootstrap* digunakan untuk mengimplementasikan berbagai pilihan warna, ukuran, font, dan layout yang ada dalam framework tersebut ke dalam sebuah website.

- Grid System pada bootstrap yang terdiri dari 12 kolom default.

- Grid system pada bootstrap menggunakan container,baris dan kolom untuk menata dan menyelaraskan konten,yang dibangun menggunakan flexbox dan itu sudah responsive.

contoh penggunaan grid system

    <div class="container text-center">
    <div class="row">
    <div class="col">
        Column
    </div>
    <div class="col">
        Column
    </div>
    <div class="col">
         Column
    </div>
    </div>
    </div>