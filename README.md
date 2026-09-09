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


<img src="Screenshot 2026-09-06 213810.png" width="500"/>
<img src="Screenshot 2026-09-06 231315.png" alt="Teks Alternatif" width="500"/>
