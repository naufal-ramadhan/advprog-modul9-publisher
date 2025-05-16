# Refleksi

Nama: Muhammad Naufal Ramadhan <br>
NPM: 2306241700 <br>
Kelas: B
<hr>

a. How much data your publisher program will send to the message broker in one run? <br>
Program publisher mengirimkan 5 data pesan ke message broker dalam satu kali menjalankan program. Setiap pesan berisi struktur UserCreatedEventMessage yang memiliki dua field: user_id dan user_name. Data yang dikirim adalah informasi untuk 5 pengguna berbeda (Amir, Budi, Cica, Dira, dan Emir) dengan ID berurutan dari 1 hingga 5, dan setiap nama pengguna diawali dengan NPM "2306241700-".

b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? <br>
URL tersebut merupakan connection string yang digunakan untuk menghubungkan aplikasi dengan message broker RabbitMQ. Ketika URL yang sama digunakan di program publisher dan subscriber, ini berarti keduanya terhubung ke server RabbitMQ yang sama. Komponen dari URL tersebut pada bagian pertama yaitu guest merupakan username yang digunakan untuk autentikasi ke server AMQP, sementara guest kedua adalah password untuk autentikasi tersebut. Bagian localhost menunjukkan bahwa server AMQP berjalan di mesin lokal, sedangkan 5672 adalah nomor port yang digunakan oleh protokol AMQP untuk komunikasi.

Dengan menggunakan URL yang sama, publisher dan subscriber dapat berkomunikasi melalui message broker yang sama, memungkinkan terjadinya pertukaran pesan antara kedua aplikasi tersebut.