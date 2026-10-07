# Pre-processing Data
## Identitas
Kelas 2025C

Program Studi S1 Sains Data

Universitas Negeri Surabaya

Nama Anggota:

Namira Rachmi Andini (25031554153)

Syahira Nanda Raihanna (25031554199)

## Deskripsi

Repository ini berisi proses preprocessing data teks pada dataset film. Dataset yang digunakan berupa file CSV yang memiliki beberapa atribut, dengan kolom `description` digunakan sebagai sumber utama data teks. Preprocessing dilakukan untuk membersihkan dan menyeragamkan data teks sehingga menghasilkan data yang lebih terstruktur dan siap digunakan pada tahap feature engineering maupun text similarity.

## Langkah-Langkah Preprocessing

Tahapan preprocessing yang dilakukan pada data teks meliputi:

1. **Mempersiapkan Data Teks**
   Kolom `description` digunakan sebagai sumber teks utama. Data yang kosong ditangani agar tidak menyebabkan kesalahan pada proses preprocessing.

2. **Menghapus HTML**
   Tag HTML yang terdapat pada teks dihapus sehingga hanya menyisakan isi teks yang dapat digunakan untuk analisis.

3. **Lowercase**
   Seluruh teks diubah menjadi huruf kecil untuk menyeragamkan bentuk penulisan. Dengan demikian, kata yang sama tetapi memiliki perbedaan huruf kapital tidak dianggap sebagai kata yang berbeda.

4. **Menghapus Tanda Baca**
   Tanda baca seperti titik, koma, tanda seru, tanda tanya, dan karakter tanda baca lainnya dihapus dari teks.

5. **Menghapus Angka**
   Angka yang terdapat dalam teks dihapus karena tidak digunakan sebagai informasi utama dalam proses analisis teks.

6. **Menghapus Spasi Berlebih**
   Spasi yang berlebihan atau tidak diperlukan dihapus dan dirapikan sehingga setiap kata dipisahkan dengan spasi yang sesuai.

7. **Menghapus Emoji**
   Emoji yang terdapat dalam teks dihapus agar data hanya berisi teks yang digunakan dalam proses analisis.

8. **Menghapus Stopwords**
   Kata-kata umum dalam bahasa Inggris yang dianggap kurang memberikan informasi penting terhadap analisis, seperti kata penghubung dan kata bantu, dihapus menggunakan daftar stopwords dari NLTK.

9. **Stemming**
   Setiap kata diubah ke bentuk dasarnya menggunakan Porter Stemmer. Tahap ini bertujuan untuk mengurangi variasi bentuk kata yang memiliki akar kata yang sama.

10. **Menghasilkan Teks Bersih**
    Setelah seluruh tahapan selesai, data menghasilkan teks yang telah dibersihkan dan disimpan sebagai data hasil preprocessing. Data tersebut selanjutnya digunakan untuk tahap feature engineering dan text similarity.
