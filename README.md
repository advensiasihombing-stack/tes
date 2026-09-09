NIM : 260530911069
Nama : Advensia Natalin Sihombing
Divisi : Cyber Security

CHALLENGE UNDO
<img src="Screenshot 2026-09-06 231307.png" alt="Teks Alternatif" width="500"/>
<img src="Screenshot 2026-09-06 231315.png" alt="Teks Alternatif" width="500"/>
LANGKAH PENYELESAIAN
Langkah 1: Menggunakan perintah base64 -d untuk mengembalikan string CHARACTER ke bentuk string sumber dengan cara melakukan proses decoding Base64.

Langkah 2: Menggunakan command rev untuk membalik urutan teks, sehingga karakter yang berada di awal menjadi berada di bagian akhir, dan sebaliknya.

Langkah 3: Menggunakan command tr '-' '_' untuk mengganti seluruh simbol - yang terdapat pada teks menjadi simbol _.

Langkah 4: Menggunakan command tr '()' '{}' untuk mengubah karakter ( dan ) menjadi { dan }.

Langkah 5 (terakhir): Menggunakan command tr 'a-zA-Z' 'n-za-mN-ZA-M' untuk melakukan proses enkripsi atau dekripsi menggunakan metode ROT13 (Rotate 13). Metode ini bekerja dengan menggeser setiap huruf alfabet sebanyak 13 posisi. Karena alfabet terdiri dari 26 huruf, penerapan ROT13 sebanyak dua kali pada teks yang sama akan mengembalikannya ke bentuk semula.


CHALLENGE INTRO TO BURP
<img src="Screenshot 2026-09-06 213810.png" alt="Teks Alternatif" width="500"/>
<img src="Screenshot 2026-09-06 232300.png" alt="Teks Alternatif" width="500"/>
LANGKAH PENYELESAIAN
Langkah 1: Pertama, kita menyalin link atau URL website yang akan digunakan. Setelah itu, buka tools Burp Suite yang akan digunakan untuk memantau dan mengatur request dari browser.
Langkah 2: Setelah Burp Suite terbuka, aktifkan fitur “Intercept On” pada bagian Proxy. Selanjutnya, pilih opsi Open Browser untuk membuka browser yang sudah terhubung dengan Burp Suite.
Langkah 3: Setelah browser berhasil terbuka, masukkan atau akses website yang sebelumnya sudah disiapkan. Kemudian, kembali ke Burp Suite dan periksa request yang masuk. Jika sudah sesuai, gunakan opsi “Forward All” agar seluruh request dapat diteruskan ke website.
Langkah 4: Setelah request berhasil diteruskan, kembali ke halaman website. Selanjutnya, lakukan proses registrasi dengan mengisi data yang diperlukan pada form pendaftaran, kemudian lanjutkan ke tahap berikutnya.
Langkah 5: Setelah proses registrasi dilakukan, kembali lagi ke Burp Suite untuk melihat request yang dikirim oleh website. Kemudian, gunakan kembali opsi “Forward All” untuk meneruskan request tersebut. Setelah itu, kembali ke browser untuk melanjutkan proses pada website.
Langkah 6: Pada tahap berikutnya, website akan meminta pengguna untuk memasukkan kode OTP. Masukkan kode OTP yang diberikan pada kolom yang tersedia, kemudian lanjutkan proses sesuai dengan halaman website.
Langkah 7: Setelah kode OTP dikirim, kembali ke Burp Suite dan periksa request yang berisi data OTP tersebut. Pada bagian request, kode OTP kemudian dihapus atau dikosongkan sebelum request diteruskan ke tahap berikutnya.
Langkah 8: Setelah perubahan dilakukan, lanjutkan dengan memilih “Forward All” agar request diteruskan. Setelah proses selesai, kembali ke browser dan periksa respons yang diberikan oleh website. Dari proses tersebut, kita dapat melihat hasil yang diperoleh setelah request diproses oleh server.
