# Reflection 1
## Prinsip-prinsip Clean Code dan Secure Coding yang diterapkan
- Nama variable yang bermakna

  Menggunakan variable seperti productId, productName, dan productQuantity. Variable tersebut dapat dengan mudah dimengerti sebagai id, nama, dan kuantitas dari sebuah produk.
- Nama function yang bermakna

  Menggunakan nama fungsi seperti create, edit, delete yang bermakna membuat, mengubah, dan menghapus.
- Membuat function sependek mungkin

  Membuat fungsi yang hanya memiliki satu tujuan saja. Contohnya create, edit, delete yang memiliki satu tujuan saja.
- Konsisten dalam formating dan indentasi

## Hal yang dapat dikembangkan
- Menggunakan UUID sebagai id product menggantikan integer untuk menghindari brute force
- Delete product diimplementasikan menggunakan method GET. Method dapat diganti menggunakan method POST/DELETE untuk menghapus produk
- Menggunakan struktur data yang lebih baik untuk menyimpan product, seperti AVL Tree.

# Reflection 2
1. - Setelah membuat unit test, saya menjadi lebih yakin ketika akan mengembangkan kode ini kembali tanpa takut terjadi kegagalan fungsionalitas yang telah ada.
   - Tidak terdapat aturan khusus seberapa banyak unit test harus dibuat. Semakin banyak skenario akan semakin baik untuk menjaga fungsionalitas kode tetap bekerja sebagaimana mestinya.
   - Membuatnya menjadi beberapa kasus-kasus tertentu, dengan demikian akan membuat unit test kita dapat memverifikasi kebenaran kode.
   - 100% code coverage belum tentu menjamin tidak adanya bug pada kode. Namun, memberi gambaran sejauh mana kode diuji.

2. - Kode functional test serupa akan terjadi duplikasi seperti setup dan inisialiasi variable-variable tertentu.
   - Kode baru tersebut dapat mengurangi kualitas kode karena akan terjadi duplikasi yang berulang kali. Di mana tidak sesuai dengan kaidah clean code sendiri. Untuk mengembangkannya, kita dapat membuat inisialisasi atau setup pada fungsi atau kelas tertentu yang dapat digunakan berulang kali. 