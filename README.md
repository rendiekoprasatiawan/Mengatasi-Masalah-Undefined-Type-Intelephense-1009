# Mengatasi Masalah Undefined Type Intelephense (1009)

* Intelephense memiliki opsi konfigurasi untuk mengaktifkan/menonaktifkan setiap kategori simbol yang tidak ditentukan untuk disesuaikan dengan gaya pengkodean

* Pada pembaruan terbaru dari PHP Intelephense, intelephense terus menunjukkan kesalahan untuk simbol yang tidak terdefinisi untuk rute (dan kelas lainnya juga), tidak ada           kesalahan seperti ini sebelumnya dan itu mengganggu

* Kebanyakan orang tidak terlalu suka melihat warna Error merah dimana-mana

* Maka dari itu solusinya :

* Pada Visual Studio Code -> Masuk ke File > Preferences > Settings

* Bisa dengan cara melakukan pencarian :

  ```
  intelephense.diagnostics
  ```
  
* Spesifiknya cari intelephense dibawah ini dan ubah nilainya menjadi false :
  ```
  - intelephense.diagnostics.undefinedTypes
  - intelephense.diagnostics.undefinedFunctions
  - intelephense.diagnostics.undefinedConstants
  - intelephense.diagnostics.undefinedClassConstants
  - intelephense.diagnostics.undefinedMethods
  - intelephense.diagnostics.undefinedProperties
  ```
* Singkatnya dapat menghilangkan centang enablenya

* Bisa dicentang enable lagi jika ingin mengembalikan intelephense seperti semula
