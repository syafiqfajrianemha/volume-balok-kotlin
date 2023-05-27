# Menghitung Volume Balok
#### Latihan ini bertujuan untuk mengimplementasikan komponen Activity pada aplikasi pertama Android saya menggunakan Kotlin.
![alt text](https://github.com/syafiqfajrianemha/volume-balok-kotlin/blob/main/ui-hitung-volume-balok.png?raw=true)
## Rangkuman Activity
- **Activity** merupakan komponen penting Android yang berfungsi untuk menampilkan user interface ke layar pengguna dan mengelola interaksi yang ada di dalamnya.
- Setiap Activity harus terdaftar di **AndroidManifest.xml** supaya tidak terjadi error.
- **Lifecycle** merupakan urutan state yang menunjukkan posisi proses aplikasi mulai dari Activity diciptakan sampai dihancurkan.
- Anda dapat menambahkan kode pada setiap setiap state lifecycle dengan **override** fungsi yang ada pada Activity.
- Perhatikan bahwa dalam penulisan kode XML, ada dua cara dalam penulisan tag seperti berikut:
  - **Self-closing tag**: tag diawali dengan < dan diakhiri dengan />. Biasanya digunakan untuk View tanpa isi.
  - **Opening tag** dan **closing tag**: opening tag diawali dengan < dan diakhiri dengan > saja. Sebagai gantinya, ada closing tag dengan format </NamaView>. Biasanya digunakan untuk layout yang menampung View lain di dalamnya.
- Di dalam sebuah tag View, Anda bisa mengubah beberapa attribute dengan beberapa format berikut:
  - **android:<property_name>="@+id/view_id**" untuk penulisan id.
  - **android:<property_name>="<property_value>"** untuk attribute biasa.
  - **android:<property_name>="@<resource_type>/resource_id"** untuk attribute yang memanggil value dari folder res, seperti string, color, dan dimensi.
- Penulisan teks secara langsung (hardcoded) merupakan praktik yang kurang baik karena seharusnya kita menuliskan semua teks pada berkas **res/values/strings.xml** dan setelah itu baru memanggilnya.
- Dalam menentukan tinggi dan lebar suatu View, terdapat beberapa alternatif value yang bisa digunakan seperti berikut:
  - **wrap_content**: ukuran menyesuaikan dengan ukuran konten di dalamnya.
  - **match_parent**: ukurang menyesuaikan dengan ukuran parent (View induknya). Apabila di paling luar, berarti mengikuti ukuran layar device-nya.
  - **fixed size**: Anda bisa menentukan ukuran dengan nilai tetap dengan satuan dp.
- Berikut beberapa satuan ukuran yang bisa Anda gunakan dalam mendesain menggunakan XML:
  - **sp** (scale independent pixel): digunakan untuk ukuran teks, tetapi diskalakan berdasarkan preferensi ukuran font pengguna.
  - **dp** (density independent pixel): digunakan untuk semuanya selain ukuran teks.
  - **px**: ukuran piksel sebenarnya di layar. Penggunaan px tidak disarankan karena dapat menghasilkan ukuran yang berbeda.
- **onCreate()** merupakan fungsi yang pertama kali dipanggil ketika membuka sebuah Activity.
- **setContentView** digunakan untuk menampilkan XML pada sebuah Activity.
- **findViewById** digunakan untuk menginisialisasi variabel dengan komponen View yang ada di XML sesuai dengan id-nya.
- **setOnClickListener** digunakan untuk melakukan aksi tertentu ketika suatu komponen ditekan.
- Untuk mengambil suatu teks dari EditText, Anda bisa menggunakan fungsi **text.toString** pada Kotlin.
- Untuk mengatur teks suatu TextView, Anda bisa menggunakan fungsi **.text** pada Kotlin.
- **onSaveInstanceState** digunakan untuk mempertahankan data ketika terjadi configuration change.
- **Configuration change** terjadi karena perubahan yang signifikan pada aplikasi sehingga akan membuat Activity dihancurkan dan dibuat lagi. Contohnya seperti perubahan orientasi, perubahan bahasa, dan ukuran layar.
