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