link deployment: [advprog-tutorial2-syauqi.koyeb.app/](advprog-tutorial2-syauqi.koyeb.app/)

# Reflection
## Code quality issue yang telah diperbaiki
1. Menghapus public modifier di ProductService interface \
   Sebelumnya, ProductService interface memiliki modifier public yang seharusnya tidak perlu ditulis lagi. Karena secara default, method yang dibuat pada interface akan bersifat public. Penghapusan modifier tersebut ditujukan untuk mengurangi redundancy. Oleh karena itu, setelah saya mengetahui isu tersebut, saya segera menghapus public modifier pada ProductService interface.

2. Menyimpan ke local variable kemudian melakukan return \
   Sebelumnya, terdapat unused local variable pada ProductServiceImpl. Seharusnya dapat langsung mereturn value tersebut tanpa menyimpannya terlebih dahulu ke sebuah local variable. Setelah mengetahui itu tersebut, saya langsung menghapus redundant local variable tersebut dan langsung mereturn value tersebut tanpa menyimpannya ke local variable terlebih dahulu.

3. Unused import all \
   Sebelumnya, terdapat import all, atau import bintang. Hal tersebut menyebabkan unused import karena tidak semua yang diimport akan digunakan. Setelah mengetahui hal tersebut, saya mengganti import bintang dengan import satu per satu.

## Apakah implementasi sekarang telah sesuai dengan definisi CI/CD
Implementasi CI/CD sekarang sudah lumayan cukup mewakili dari definisi CI/CD itu sendiri. Dengan bantuan github workflow, membantu kita untuk menjalankan unit test yang akan membantu menjaga kebenaran kode program. Selain itu, PMD membantu untuk mencari kesalahan yang mungkin terjadi pada kode kita. Setelah melalui kedua tahap tersebut, di mana program terlah berjalan dengan baik. Kita dapat melakukan merge branch ke main branch yang nantinya akan dibuild secara otomatis oleh koyeb sampai ke proses operasional. Di mana website dapat berjalan dan diakses oleh orang lain.

Dari semua langkah tersebut, kita telah melewati proses kode, test, review, dan operasional yang terotomisasi. Sebagaimana automation pada software development lifecycle.

## Coverage
![image](https://github.com/user-attachments/assets/963df8ea-7513-402c-a158-696fcad8c2d2)
