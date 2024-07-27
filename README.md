# SMART CHAIR
Kursi Pintar Berbasis AI dan IoT sebagai Pemantau Kesehatan di Kantor

## Deskripsi Proyek
SMART CHAIR adalah kursi kantor pintar yang mengintegrasikan teknologi AI dan IoT untuk memantau dan meningkatkan kesehatan di tempat kerja. Kursi ini memberikan data dan umpan balik secara real-time untuk membantu pengguna menjaga postur tubuh yang baik dan mengelola kesehatan selama bekerja.

## Fitur
- Pemantauan Postur dengan AI: Mendeteksi dan memperbaiki postur tubuh yang buruk secara otomatis.
- Konektivitas IoT: Menghubungkan dengan perangkat Anda untuk memberikan analisis kesehatan dan pengingat.
- Metrik Kesehatan: Melacak dan melaporkan berbagai indikator kesehatan seperti waktu duduk, kualitas postur, dan lainnya.
- Antarmuka Ramah Pengguna: Aplikasi yang mudah digunakan untuk mengakses data kesehatan Anda dan menerima tips yang dipersonalisasi.

## Instruksi 
### Langkah 1: Pengambilan Data Sensor dengan Timestamp dan Mengirim ke Server Flask

Gunakan kode Arduino untuk membaca data sensor, menambahkan timestamp, mengirim data ke server Flask, dan menampilkan peringatan di LCD 16x2 I2C jika suhu atau kadar CO2 melebihi batas yang telah ditentukan.

### Langkah 2: Penerimaan Data di Server Flask dan Pengolahan Data

Buat server Flask yang menerima data dari ESP32, menyimpan data ke CSV, dan mendeteksi outlier menggunakan Isolation Forest.

### Langkah 3: Pelatihan Model Isolation Forest

Pelatihan model Isolation Forest untuk mendeteksi outlier dan menyimpannya ke file.

### Langkah 4: Penambahan Noise ke Data

Tambahkan noise ke data untuk mensimulasikan kondisi dunia nyata dan kemudian melatih kembali model.

### Langkah 5: Visualisasi Data

Visualisasi data asli dan data yang telah diberi noise.

### Langkah 6: Penggunaan Model Isolation Forest dalam Real-time

Gunakan model yang telah dilatih untuk mendeteksi outlier dalam data yang diterima secara real-time dan memberikan peringatan kepada pengguna.
