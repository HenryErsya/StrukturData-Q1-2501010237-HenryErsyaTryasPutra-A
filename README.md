# StrukturData-Q1-2501010237-HenryErsyaTryasPutra-A

1. Karakteristik Memori dan Akses Data
Jelaskan mengapa operasi akses elemen pada Array dapat dilakukan dalam waktu konstan
O(1), sedangkan pada Singly Linked List membutuhkan waktu linear O(n). Hubungkan
jawaban Anda dengan konsep alamat memori (kontinu vs non-kontinu).

Jawaban : 

Array bisa mengakses elemen tertentu dengan cepat dalam waktu O(1) karena elemen-elemennya tersimpan berurutan di memori. Alamat elemen ke-n langsung dihitung dari alamat awal ditambah perkalian indeks dengan ukuran elemen, tanpa perlu mencari-cari. Berbeda dengan singly linked list, elemennya tersebar di memori dan hanya terhubung lewat pointer ke elemen berikutnya, sehingga harus dilalui satu per satu dari awal hingga target—ini yang membuatnya butuh waktu O(n).

2. Analisis Efisiensi Operasi Manipulasi
Dalam kondisi apa sebuah Linked List lebih diunggulkan dibandingkan Array untuk ope
rasi penyisipan (insertion) dan penghapusan (deletion) data? Berikan alasan teoritisnya.

Jawaban :

Linked list lebih baik untuk menyisipkan atau menghapus data jika kita sudah tahu posisi pastinya, karena cukup mengubah pointer antar node tetangga, selesai dalam O(1). Array malah harus menggeser elemen-elemen lain agar tetap rapat di memori, yang memakan waktu O(n). Situasi idealnya adalah saat data sering berubah ukurannya di posisi tengah, seperti daftar tugas yang dinamis.scribd+1

3. Konsep Doubly Linked List
Jelaskan struktur anatomi dari sebuah node pada Doubly Linked List. Apa dampak kebe
radaan pointer tambahan tersebut terhadap penggunaan memori serta fleksibilitas pene
lusuran dibandingkan dengan Singly Linked List?

Jawaban :

Setiap node di doubly linked list punya tiga bagian: data, pointer ke node berikutnya (next), dan pointer ke node sebelumnya (prev). Pointer tambahan ini menambah pemakaian memori sekitar satu pointer ekstra per node. Tapi manfaatnya besar, karena kita bisa menelusuri maju-mundur dengan mudah, tidak seperti singly linked list yang hanya satu arah

4. Mekanisme Circular Linked List
Apa yang membedakan Circular Linked List dari Linked List biasa secara teoritis? Se
butkan satu contoh skenario penggunaan (use case) di mana struktur melingkar ini lebih
efektif digunakan.

Jawaban :

Pada linked list biasa, pointer terakhir menunjuk ke null sebagai tanda akhir. Circular linked list menyambungkan pointer terakhir kembali ke node pertama, membentuk lingkaran penuh. Ini berguna untuk kasus seperti penjadwalan proses di sistem operasi, di mana elemen bisa diakses secara berulang tanpa harus kembali ke awal dari nol.

5. Array Dinamis di Python
Python list secara internal diimplementasikan sebagai Dynamic Array. Jelaskan meka
nisme yang terjadi ”di balik layar” ketika sebuah Dynamic Array kehabisan kapasitas saat
melakukan operasi append.

Jawaban :

Python list dibuat sebagai dynamic array yang selalu menyediakan ruang lebih dari yang dibutuhkan. Saat append melebihi kapasitas, ia membuat array baru yang lebih besar, menyalin isi lama ke sana, lalu membuang yang lama—proses ini disebut resizing. Rata-rata tetap efisien O(1), meski sesekali butuh O(n) saat menyalin.

