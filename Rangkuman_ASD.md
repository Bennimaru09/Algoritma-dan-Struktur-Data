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
  Logs adalah kebalikan dari eksponensial. CTH: 10**2 = 100 <-> log10 100 = 2. 

Dalam buku ini, ketika kita berbicara mengenai Running time dalam Big O notatition dan ditemui adanya ekspresi log maka  ekspresi log ini selalu mengacu pada log basis2. Ketika kamu mencari sebuah element menggunakan simple search, dalam worst case kamu mungkin harus melihat satu per satu element yang ada. Jadi ketika ada list untuk 8 nomor, kamu harus mengecek sebanyak 8 kali. Sedangkan ketika kita menggunakan binary search kita hanya perlu mengecek sebanyak log n element dalam worst case. Untuk 8 element, log 8 = 3 dikarenakan 2**3 = 8. Untuk list dengan 1024 elements, log 1024 = 10, karena 2^10 = 1024.

	# Notes
	Binary search hanya bekerja jika list yang diberikan sudah terurut, seperti contohnya nama didalam kontak HP yang udah terurut secara alphabetical, jadi kamu bisa menggunakan binary search untuk mencari suatu nama.
 
# Binary Search in Python
	
