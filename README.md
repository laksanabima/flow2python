# Flow2Python

Flow2Python adalah aplikasi desktop pembelajaran yang membantu mahasiswa menyusun algoritma secara visual menggunakan flowchart, lalu melihat hasil konversinya dalam bentuk kode Python. Aplikasi ini dibuat dengan React.js dan dikemas sebagai aplikasi desktop, sehingga alur algoritma dapat dirancang melalui kanvas tanpa harus langsung menulis seluruh kode secara manual.

Menurut saya, nilai utama Flow2Python adalah menjembatani cara berpikir algoritmis dengan sintaks pemrograman. Mahasiswa dapat melihat hubungan antara simbol, alur keputusan, dan kode yang dihasilkan. Aplikasi ini paling cocok digunakan sebagai media latihan dan pendamping pembelajaran—bukan pengganti latihan membaca, memahami, dan menulis kode Python sendiri.

## Fitur

- **Kanvas flowchart:** susun diagram dengan menyeret simbol dari palet dan menghubungkan titik koneksinya.
- **Simbol algoritma:** Start, End, Process, Input, Output, Decision, dan Loop.
- **Konversi ke Python:** panel *Python Code* menampilkan kode berdasarkan flowchart.
- **Edit properti:** pilih simbol dan gunakan panel *Properties* untuk mengubah isinya.
- **Jalankan dan lihat hasil:** tombol **Run** menjalankan program dan menampilkan hasil atau pesan di panel **Console**.
- **Kelola diagram:** buat diagram baru, Undo/Redo, atau mulai dari contoh melalui **Load Example...**.
- **Simpan dan bagikan:** **Export JSON** menyimpan diagram ke berkas JSON dan **Import JSON** memuatnya kembali.
- **Gunakan kode di luar aplikasi:** **Copy Python** menyalin kode, sedangkan **Download .py** mengunduhnya sebagai berkas Python.
- **Navigasi kanvas:** kontrol zoom dan minimap membantu melihat diagram yang besar; tombol tema dapat mengganti tampilan.

## Unduh dan instal di Windows

Rilis yang tersedia di folder distribusi ini adalah **Flow2Python 1.0.0** untuk Windows 64-bit. Pilih salah satu berkas berikut:

- **`Flow2Python Setup 1.0.0.exe`** — installer yang disarankan. Berkas ini berukuran sekitar 137 MB.
- **`Flow2Python 1.0.0.exe`** — versi portable; jalankan langsung tanpa melalui proses instalasi.

### Instalasi dengan installer

1. Unduh `Flow2Python Setup 1.0.0.exe` dari sumber distribusi resmi yang diberikan pengajar atau pembuat aplikasi.
2. Buka berkas installer. Jika Windows menampilkan konfirmasi keamanan, lanjutkan hanya apabila berkas berasal dari sumber yang tepercaya.
3. Ikuti langkah-langkah pada jendela instalasi. Anda dapat memilih lokasi pemasangan.
4. Setelah selesai, buka **Flow2Python** dari shortcut Desktop atau menu Start.

Untuk memakai versi portable, simpan `Flow2Python 1.0.0.exe` di komputer lalu buka berkas tersebut. Jangan menghapus atau memindahkan berkas ketika aplikasi sedang berjalan.

## Tutorial penggunaan

### 1. Membuat flowchart

1. Buka Flow2Python. Kanvas berada di bagian tengah, palet simbol di sebelah kiri, dan panel kode di sebelah kanan.
2. Seret **Start** ke kanvas sebagai awal algoritma.
3. Tambahkan simbol yang diperlukan. Contohnya, gunakan **Input** untuk menerima data, **Process** untuk perhitungan, **Decision** untuk percabangan, **Output** untuk menampilkan hasil, dan **End** untuk mengakhiri alur.
4. Klik simbol yang ingin diubah, lalu sesuaikan nilainya di panel **Properties**.
5. Hubungkan titik koneksi antarsimbol agar alur dapat diikuti. Untuk **Decision**, hubungkan kedua cabang sesuai kondisi benar dan salah; pastikan keduanya menuju langkah yang tepat.
6. Atur tampilan dengan kontrol zoom atau minimap bila diagram terlalu besar. Periksa indikator validasi di atas kanvas dan benahi alur jika diagram belum valid.

### 2. Melihat dan menjalankan kode

1. Perhatikan panel **Python Code**. Kode diperbarui berdasarkan flowchart yang dibuat.
2. Klik **Run** untuk menjalankan program. Lihat pesan atau hasilnya di panel **Console**; masukkan nilai jika program meminta input.
3. Jika hasil tidak sesuai, periksa kembali nilai pada simbol, sambungan, dan arah cabang keputusan, lalu jalankan lagi.

### 3. Contoh latihan: menentukan bilangan genap atau ganjil

1. Pilih **Load Example...** dan muat contoh yang tersedia, jika contoh tersebut ada.
2. Ikuti pola algoritma: **Start → Input** bilangan `n` → **Decision** dengan kondisi `n % 2 == 0`.
3. Hubungkan cabang kondisi benar ke keluaran **"Genap"**, dan cabang salah ke keluaran **"Ganjil"**. Hubungkan kedua cabang kembali ke **End**.
4. Periksa kode yang tampil. Secara konsep, kondisi tersebut menjadi `if n % 2 == 0`, dengan hasil berbeda untuk cabang benar dan salah.
5. Klik **Run**, masukkan sebuah bilangan, dan amati hasil di **Console**.

### 4. Menyimpan atau membagikan pekerjaan

- Klik **Export JSON** untuk menyimpan diagram agar bisa dibuka atau dilanjutkan nanti dengan **Import JSON**.
- Klik **Copy Python** untuk menyalin kode ke clipboard, atau **Download .py** untuk menyimpan kode sebagai berkas `.py`.
- Berkas JSON menyimpan diagram untuk dibuka kembali di Flow2Python; berkas `.py` berisi kode untuk dipelajari atau digunakan di lingkungan Python.

### 5. Mengedit diagram

- **New** memulai diagram baru.
- **Undo** membatalkan perubahan terakhir, sedangkan **Redo** mengulangi perubahan yang dibatalkan.
- Pilih simbol pada kanvas untuk mengedit propertinya atau menyusun ulang alurnya.

## Tips untuk mahasiswa dan pengajar

- Mulai dari algoritma sederhana: urutan langkah, input-output, kemudian percabangan dan perulangan.
- Pastikan setiap alur memiliki **Start** dan **End**, dan setiap cabang keputusan memiliki tujuan yang jelas.
- Bandingkan flowchart dengan kode Python, bukan hanya menyalin kode yang dihasilkan. Perhatikan bagaimana kondisi dan urutan proses diterjemahkan.
- Uji beberapa nilai input, termasuk nilai di batas kondisi, agar cabang yang berbeda ikut diperiksa.
- Simpan diagram JSON sebagai bahan tugas atau untuk melanjutkan latihan. Bagikan berkas `.py` jika yang dibutuhkan adalah kode hasilnya.

## Catatan rilis

- Versi: **1.0.0**
- Platform paket saat ini: **Windows 64-bit**
- Installer menyediakan pilihan lokasi pemasangan serta shortcut Desktop dan menu Start.