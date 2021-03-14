PL RESOLUTION, BACKWARD CHAINING DAN FORWARD CHAINING

Terdapat 3 tugas, yaitu: Forward Chaining, Backward Chaining, dan Propositional Logic.

1) Forward Chaining: Di sini kita telah memberikan pengetahuan-pengetahuan dasar yang mencakup aturan dan fakta. Ide dasar dibalik rangkaian maju adalah itu
dari fakta kita mempelajari aturan dan melihat mana di antara mereka yang bisa dipecat. Aturan yang disalahkan atau dipecat (?), akan dimasukkan ke dalam list fakta. Kemudian list fakta yang telah dikumpulkan kemudian digunakan untuk membuat aturan baru yang lebih kompleks.

2) Rantai Mundur: Dalam hal ini kita memiliki kesimpulan dan kita harus membuktikan bahwa kesimpulan tsb terjadi dengan cara menganalisa mundur, yaitu dari aturan ke fakta. Jadi, pada setiap iterasi, kami memperoleh daftar tujuan (yang merupakan daftar tempat) dan menggunakan tempat ini kami mencoba untuk mencapai fakta. Kalau bisa, berarti kesimpulannya bisa diturunkan dari fakta-fakta itu. Jika tidak, maka kesimpulan tidak dapat dibuktikan dari fakta-fakta yang ada.

3) Logika Proposisional: Masukan diberikan kepada kita dalam klausa HORN. Jadi, untuk mengimplementasikan logika proposisional agar berfungsi, kita harus mengubah bentuk klausa klausa menjadi Conjunctive Normal Form (CNF). Aturan yang diterapkan untuk membentuk klausa terselesaikan dari dua klausa adalah sebagai berikut: -

(A v B) (-B v C) akan menghasilkan (A v C).
Saat mengikuti aturan ini, ada dua hal yang perlu diperhatikan. Pertama adalah kita harus menghapus duplikat literal yang mungkin muncul saat kita menyelesaikan file
ayat. Kedua, dan yang paling penting, jika klausa memiliki literal sehingga ada tipe positif dan negatif dari literal tersebut (Misalnya, katakanlah A v B v C v -A), maka kami tidak menyertakan klausa ini. Ini karena, nilainya akan dihitung menjadi 1.

Kompilasi dan Instruksi Menjalankan
1) Kompilasi program: javac pl.java
2) Jalankan program: java pl -t 1 -kb kb2.txt -q q2.txt -oe output.txt -ol logs.txt

Waktu yang dibutuhkan untuk menjalankan resolusi untuk kasus I: 35-40 detik pada mesin aludra
Waktu yang dibutuhkan untuk menjalankan resolusi untuk kasus II: 2:30 hingga 3 menit pada mesin aludra.

Persamaan / Perbedaan antara Tugas 1,2 dan 3

Dari log program, terbukti bahwa forward chaining adalah yang terbaik karena membutuhkan waktu yang lebih singkat dibandingkan dengan pendekatan lainnya. Dalam siklus rantai mundur terdeteksi yang menyebabkan penundaan dalam output. Perangkaian maju dan mundur hanya berfungsi untuk klausa klausa. Tetapi resolusi dapat berfungsi untuk semua jenis klausa tetapi masalah utamanya adalah bahwa resolusi membutuhkan banyak waktu dibandingkan dengan apporach lainnya. Log resolusi jauh lebih besar dibandingkan dengan teknik perangkaian maju dan mundur. Subuset klausa menjadi lebih besar karena lebih banyak jumlah klausa yang diselesaikan.

