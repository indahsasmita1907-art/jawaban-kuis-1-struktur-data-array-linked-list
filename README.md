# jawaban-kuis-1-struktur-data-array-linked-list
Jawaban Quis 1 Struktur Data: Array dan Linked List
1. Karakteristik Memori dan Akses Data
Array memiliki akses data dengan kompleksitas waktu O(1) karena data disimpan secara berurutan (kontinu) di memori. Setiap elemen memiliki indeks sehingga alamat memori dapat dihitung langsung. Karena itu, elemen dapat diakses tanpa menelusuri data lain.

Sedangkan pada Singly Linked List, data disimpan secara tidak berurutan (non-kontinu). Setiap node hanya memiliki data dan pointer ke node berikutnya. Untuk mencari elemen tertentu harus menelusuri node satu per satu dari awal sehingga kompleksitas waktunya O(n).

2. Analisis Efisiensi Operasi Manipulasi
Linked List lebih unggul dibandingkan Array pada operasi insertion dan deletion ketika data sering berubah atau penyisipan dilakukan di tengah data.

Pada Array, insertion dan deletion memerlukan pergeseran elemen sehingga membutuhkan waktu O(n). Sedangkan pada Linked List cukup mengubah pointer antar node tanpa memindahkan data lain. Jika posisi node sudah diketahui maka operasi dapat dilakukan dalam O(1).

3. Konsep Doubly Linked List
Node pada Doubly Linked List terdiri dari:

Data
Pointer next
Pointer prev
Pointer tambahan membuat penggunaan memori lebih besar dibandingkan Singly Linked List. Namun, penelusuran dapat dilakukan dua arah, maju dan mundur, sehingga lebih fleksibel dan mempermudah operasi deletion.

4. Mekanisme Circular Linked List
Circular Linked List memiliki node terakhir yang menunjuk kembali ke node pertama sehingga membentuk lingkaran. Berbeda dengan Linked List biasa yang node terakhirnya bernilai NULL.

Contoh penggunaan Circular Linked List adalah sistem Round Robin Scheduling karena proses dapat berjalan terus menerus secara bergiliran.

5. Array Dinamis di Python
Python list menggunakan Dynamic Array. Ketika kapasitas penuh saat append dilakukan, Python akan membuat array baru dengan ukuran lebih besar lalu menyalin seluruh data dari array lama ke array baru.

Proses ini membutuhkan waktu O(n) karena data harus disalin ulang, tetapi append tetap dianggap O(1) secara rata-rata (amortized).
