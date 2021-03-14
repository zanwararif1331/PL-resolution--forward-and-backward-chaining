PL RESOLUTION, BACKWARD CHAINING DAN FORWARD CHAINING

Terdapat 3 tugas, yaitu: Forward Chaining, Backward Chaining, dan Propositional Logic.

1) Forward Chaining: Di sini kita telah memberikan pengetahuan-pengetahuan dasar yang mencakup aturan dan fakta. Ide dasar dibalik rangkaian maju adalah itu
dari fakta kita mempelajari aturan dan melihat mana di antara mereka yang bisa dipecat. Aturan yang disalahkan atau dipecat (?), akan dimasukkan ke dalam list fakta. Kemudian list fakta yang telah dikumpulkan kemudian digunakan untuk membuat aturan baru yang lebih kompleks.

2) Rantai Mundur: Di sini kita memiliki kesimpulan dan kita harus membuktikan bahwa kesimpulan tsb terjadi, dengan cara menganalisa mundur, yaitu dari aturan ke fakta. Jadi, di setiap iterasinya, kita sudah punya sudah punya daftar goals (atau disini disebutkan sebagai tempat atau bagain pengantarnya) dan kita akan mencoba menggunakan hal ini kita untuk mendapat fakta dari dari kesimpulan tsb. Kalau bisa, berarti kesimpulannya bisa kita dapatkan dari fakta-fakta itu. Dan jika tidak, maka kesimpulannya tidak dapat kita buktikan dari fakta-fakta yang tersebut.

3) Logika Proposisional: Input-an akan diberikan pada kita dalam klausa HORN. Jadi, untuk mengimplementasikan logika proposisional, kita harus mengubah bentuk klausa klausa menjadi Conjunctive Normal Form (CNF). Aturan yang diterapkan untuk membentuk suatu resolved klausa dari dua klausa adalah sebagai berikut: -

(A v B) (-B v C) akan menghasilkan (A v C).
Saat mengikuti aturan ini, ada 2 hal yang perlu diperhatikan. Pertama adalah kita perlu menghapus duplikat literal yang mungkin akan muncul saat kita telah menyelesaikan klausa-nya. Kedua, dan yang paling penting, jika klausa memiliki literal sehingga ada tipe positif dan negatif dari literal tersebut (Misalnya, katakanlah A v B v C v -A), maka kami tidak menyertakan klausa ini. Ini karena, nilainya akan dihitung menjadi 1.

Kompilasi dan Instruksi Menjalankan
1) Compile program: javac pl.java
2) Jalankan program: java pl -t 1 -kb kb2.txt -q q2.txt -oe output.txt -ol logs.txt

Waktu yang dibutuhkan untuk menjalankan resolusi untuk kasus I: 35-40 detik pada mesin aludra
Waktu yang dibutuhkan untuk menjalankan resolusi untuk kasus II: 2:30 hingga 3 menit pada mesin aludra.

Persamaan / Perbedaan antara Tugas 1,2 dan 3

Dari log program, terbukti bahwa forward chaining adalah yang terbaik karena membutuhkan waktu yang lebih singkat dibandingkan dengan pendekatan lainnya. Dalam siklus forward chaining terdeteksi yang menyebabkan penundaan dalam output. Forward Chaining dan Backward Chaining hanya berfungsi untuk klausa. Tetapi resolusi dapat berfungsi untuk semua jenis klausa tetapi masalah utamanya adalah bahwa resolusi membutuhkan banyak waktu dibandingkan dengan apporach lainnya. Log resolusi jauh lebih besar dibandingkan dengan teknik Forward dan Backward Chaining. Subuset klausa menjadi lebih besar karena lebih banyak jumlah klausa yang diselesaikan.

