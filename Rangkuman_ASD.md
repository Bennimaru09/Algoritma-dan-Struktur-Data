# Algoritma-dan-Struktur-Data
# simple search dan binary search
  Algoritma bisa didefenisikan sebagai sekumpulan instruksi untuk menyelesaikan suatu task atau tugas tertentu. 
  
# Binary seacrh
  Mencari suatu kata dalam suatu dictionary. Cara mencarinya ialah dengan mencari dari halaman awal dengan menngecek lembar per lembar. Kamus akan menyimpan sekumpulan kata secara terurut sesuai dengan alfabet. Binary search adalah algoritma yang inputnya ialah suatu list yang terdiri dari sejumlah elemen yang terurut. Ketika elemen yang kita cari ada didalam list, binary search akan mengembalikan posisi dari kata tadi, tetapi jika kata yang dicari tidak ditemukan maka binary search akan mengembalikan NULL. 
  
# Simple search
  Simple search dikatakan stupid search oleh penulis buku dikarenakan disetiap tebakan kita hanya mengeliminasi satu angka, jika angka yang dimaksud adalah 99, maka itu akan membuat kita untuk menebak 99 kali sampai mendapatkan jawaban yang tepat. 
  
# A Better Way to Search (Binary Search)
  Dengan menggunakan metode ini kita sudah bisa mengeliminasi setengah dari angka yang tersisa (1-100| dimulai menebak dari angka 50 atau setengah dari panjang angka tersebut dan walaupun salah, kita sudah bisa mengeliminasi setengah angka tersebut, dan kita akan terus menebak angka tengah dari range angka tersebut).  
  
# Binary Search Performance Explained
  dengan menggunakan simple search jumlah tahapan terbanyak yang mungkin kita lakukan adalah sebanyak 240.000 steps, jika kata yang kamu cari berada di halaman paling belakang dari buku. Sedangkan dengan menggunakan binary search kita bisa mengeliminasi setengahnya hingga ketemu kata tersebut. Jadi binary search akan membutuhkan total 18 steps saja. Secara umum untuk setiap list secara N, binary search akan mengambil log2N steps untuk menjalankan worst case, dimana simple search akan mengambil N steps.

# Logaritma
  Logs adalah kebalikan dari eksponensial. CTH: 10^2 = 100 <-> log10 100 = 2. 
Dalam buku ini, ketika kita berbicara mengenai Running time dalam Big O notatition dan ditemui adanya ekspresi log maka  ekspresi log ini selalu mengacu pada log basis2. Ketika kamu mencari sebuah element menggunakan simple search, dalam worst case kamu mungkin harus melihat satu per satu element yang ada. Jadi ketika ada list untuk 8 nomor, kamu harus mengecek sebanyak 8 kali. Sedangkan ketika kita menggunakan binary search kita hanya perlu mengecek sebanyak log n element dalam worst case. Untuk 8 element, log 8 = 3 dikarenakan 2^3 = 8. Untuk list dengan 1024 elements, log 1024 = 10, karena 2^10 = 1024.

	# Notes
	Binary search hanya bekerja jika list yang diberikan sudah terurut, seperti contohnya nama didalam kontak HP yang udah terurut secara alphabetical, jadi kamu bisa menggunakan binary search untuk mencari suatu nama.
 
# Binary Search in Python
  Pada Python, setiap elemen dalam list memiliki sebuah index yang dimulai dari 0. Index ini digunakan untuk mengakses atau memanipulasi elemen dalam list. Untuk mengakses elemen dalam list, kita dapat menggunakan index dengan menuliskan nama list diikuti dengan kurung siku ([]) yang berisi index dari elemen yang ingin diakses. Fungsi binary_search akan mengambil array yang sudah terurut. Jika item yang ada didalam array, fungsi akan mengembalikan posisi item tersebut.


# Running Time
  Running Time adalah jumlah waktu yang digunakan untuk mengeksekusi seluruh operasi di dalam suatu algoritma. Running time dari sebuah algoritma adalah fungsi dari jumlah inputnya, cth: ketika kita memiliki 100 element maka kita akan melakukan pengecekan sebanyak 100 kali. Linear Time adalah ketika runtime dari fungsi kita berbanding lurus dengan jumlah input yang diberikan. Dalam analisis sistem, sistem linear time-invariant (sistem LTI) adalah sistem yang menghasilkan sinyal keluaran dari setiap sinyal input yang tunduk pada kendala linearitas dan waktu-invarians. Dalam istilah yang lebih sederhana, algoritma linear memiliki kompleksitas waktu yang berhubungan secara langsung dengan ukuran input yang diberikan. Binary search berjalan di dalam logarithmic time(atau log time). 

# Big O Notation
  Big O Notation adalah spesial notasi yang bisa mendeskripsikan seberapa cepat sebuah algoritma itu. Big O Notation adalah cara untuk mengkonversi keseluruhan langkah-langkah suatu algoritma kedalam bentuk Aljabar. Notasi ini merepresentasikan banyaknya langkah suatu algoritma dengan menghiraukan konstanta yang lebih kecil dan koefisien yang tidak berdampak besar terhadap keseluruhan kompleksitas dari algoritma tersebut. Big O Notation digunakan untuk melakukan analisa terhadap sebuah algoritma pemrograman terhadap waktu eksekusi dan untuk menentukan seberapa efisien dan kompleksitas barisan kode dalam dimensi waktu. 

# Algorithm running times grow at different rates
  Kita tahu bahwa di satu sisi binary search lebih cepat dibandingkan dengan simple search, namun disisi yang lain simple search lebih mudah untuk ditulis, dan simple search hanya memiliki kemungkinan kecil untuk menghasilkan suatu bug.
  Simple Search dan Binary Search adalah dua algoritma yang digunakan untuk mencari elemen dalam kumpulan data terurut. Mari kita bahas perbedaan di antara keduanya:
Simple Search : Simple Search menelusuri elemen satu per satu dalam kumpulan data hingga menemukan elemen yang dicari.

Kelebihan:
- Sederhana: Implementasi sederhana karena hanya memerlukan iterasi melalui seluruh elemen.
- Tidak Memerlukan Data Terurut: Bekerja pada kumpulan data apa pun, tidak harus terurut.

Kekurangan:
- Waktu Eksekusi: Pada skenario terburuk, memerlukan banyak langkah (misalnya, jika elemen yang dicari berada di akhir kumpulan data).
- Efisiensi: Tidak efisien untuk kumpulan data besar.
  
Binary Search : Binary Search membagi kumpulan data menjadi dua bagian dan memeriksa elemen tengah. Jika elemen tengah lebih besar dari elemen yang dicari, maka hanya perlu mencari di setengah kiri. -Jika lebih kecil, hanya perlu mencari di setengah kanan. Proses ini berlanjut hingga elemen ditemukan.

Kelebihan:
- Efisien: Pada skenario terburuk, memerlukan logaritma basis 2 dari jumlah elemen (O(log n)).
- Hanya Bekerja pada Data Terurut: Memerlukan data terurut sebelumnya.
  
Kekurangan:
- Pra-Pengurutan: Memerlukan pengurutan data sebelum pencarian.
- Tidak Cocok untuk Data Tidak Terurut: Tidak dapat digunakan pada data yang tidak terurut.
  
