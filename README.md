# StrukturData-Q1-2501010237-HenryErsyaTryasPutra-A
1. Akses Elemen: Array vs Linked List
Array bisa mengakses elemen tertentu dengan cepat dalam waktu O(1) karena elemen-elemennya tersimpan berurutan di memori. Alamat elemen ke-n langsung dihitung dari alamat awal ditambah perkalian indeks dengan ukuran elemen, tanpa perlu mencari-cari. Berbeda dengan singly linked list, elemennya tersebar di memori dan hanya terhubung lewat pointer ke elemen berikutnya, sehingga harus dilalui satu per satu dari awal hingga target—ini yang membuatnya butuh waktu O(n).dte.telkomuniversity+1
2. Kelebihan Linked List untuk Insert dan Delete
Linked list lebih baik untuk menyisipkan atau menghapus data jika kita sudah tahu posisi pastinya, karena cukup mengubah pointer antar node tetangga, selesai dalam O(1). Array malah harus menggeser elemen-elemen lain agar tetap rapat di memori, yang memakan waktu O(n). Situasi idealnya adalah saat data sering berubah ukurannya di posisi tengah, seperti daftar tugas yang dinamis.scribd+1
3. Struktur Node Doubly Linked List
Setiap node di doubly linked list punya tiga bagian: data, pointer ke node berikutnya (next), dan pointer ke node sebelumnya (prev). Pointer tambahan ini menambah pemakaian memori sekitar satu pointer ekstra per node. Tapi manfaatnya besar, karena kita bisa menelusuri maju-mundur dengan mudah, tidak seperti singly linked list yang hanya satu arah.dte.telkomuniversity
4. Perbedaan Circular Linked List
Pada linked list biasa, pointer terakhir menunjuk ke null sebagai tanda akhir. Circular linked list menyambungkan pointer terakhir kembali ke node pertama, membentuk lingkaran penuh. Ini berguna untuk kasus seperti penjadwalan proses di sistem operasi, di mana elemen bisa diakses secara berulang tanpa harus kembali ke awal dari nol.dte.telkomuniversity
5. Cara Kerja Append di Python List
Python list dibuat sebagai dynamic array yang selalu menyediakan ruang lebih dari yang dibutuhkan. Saat append melebihi kapasitas, ia membuat array baru yang lebih besar, menyalin isi lama ke sana, lalu membuang yang lama—proses ini disebut resizing. Rata-rata tetap efisien O(1), meski sesekali butuh O(n) saat menyalin.dte.telkomuniversity
