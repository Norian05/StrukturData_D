# TUGAS STRUKTUR DATA 01

## 📄 PENJELASAN TENTANG KONSEP ARRAY
Array merupakan struktur data yang digunakan untuk menyimpan beberapa nilai dalam satu variabel yang sama. Data di dalam array tersusun secara berurutan di dalam memori dan setiap nilai memiliki posisi tertentu yang disebut dengan indeks. Dengan menggunakan indeks tersebut, program dapat mengambil atau mengubah data secara cepat tanpa harus mencari satu per satu. Umumnya array digunakan untuk menyimpan sekumpulan data yang memiliki tipe yang sama, seperti angka, karakter atau huruf, dan nilai lainnya.

Array memiliki 3 pendeklarasian, diantaranya :

## 1. Array 1 Dimensi
Array yang hanya memiliki satu indeks untuk mengakses elemennya yang biasa digunakan untuk menyimpan daftar data yang tersusun dalam satu baris.

Contoh Array:
```python
import numpy as np

nilai = np.array[75, 65, 80, 90]
print(nilai)
```

## 2. Array 2 Dimensi
Memiliki pengertian sama seperti array 1 dimensi hanya saja array ini memiliki dua indeks. Biasanya direpresentasikan dalam bentuk baris dan kolom (row and column) seperti tabels atau matriks.

Contoh Array:
```python
import numpy as np

table = np.array([[20, 40, 45],
                  [55, 60, 65]])
print(table)
```

## 3. Array Multi-dimensi
Seperti namanya, array ini memiliki jumlah indeks yang lebih atau sama dari dua indeks dengan struktur yang biasa digunakan untuk menyimpan data yang lebih kompleks dan memiliki beberapa tingkat pengelompokan.

Contoh Array:
```python
import numpy as np

angka = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]],
                  [[10, 11, 12], [13, 14, 15], [16, 17, 18]]])
print(angka)
```

## 📷 SCREENSHOT HASIL EKSEKUSI
1. Input 10 nilai
<img width="758" height="483" alt="image" src="https://github.com/user-attachments/assets/910b8b7d-697c-4298-b5ec-9106386ef3ae" />
<br></br>
2. Menampilkan nilai tertinggi, terendah, dan menghitung nilai rata-rata
<img width="758" height="483" alt="image" src="https://github.com/user-attachments/assets/2cabf4ac-8664-4233-95b8-662fde861085" />
<br></br>
3. Menghitung jumlah yang lulus dan tidak lulus
<img width="758" height="483" alt="image" src="https://github.com/user-attachments/assets/3ccaa9f0-c520-410e-a4b0-f5db79039dcc" />
<br></br>
4. Menampilkan bar chart dari nilai tertinggi dan nilai terendah
<img width="758" height="733" alt="image" src="https://github.com/user-attachments/assets/7d849872-a132-4e9c-abfb-044b192d91f0" />
<br></br>
5. Menampilkan bar chart dari mahasiswa yang lulus dan tidak lulus
<img width="758" height="733" alt="image" src="https://github.com/user-attachments/assets/60cd9a4d-61ac-4c58-a0db-5786718eb254" />

## 👀 ANALISIS KOMPLEKSITAS
1. Program yang dibuat menggunakan array(list) untuk menyimpan nilai-nilai mahasiswa yang diinput melalui perulangan. Proses menyimpan data memakai **_.append()_** yang dilakukan sebanyak jumlah data, yang membuat kompleksitas waktunya adalah **O(n)** dan kompleksitas ruang adalah **O(n)**.
<br></br>
2. Program selanjutnya adalah mencari nilai tertinggi, terendah, dan rata-rata menggunakan fungsi **_max()_** untuk nilai tertinggi, **_min()_** untuk nilai terendah, dan **_sum()_** untuk nilai rata-rata yang akan memeriksa seluruh elemen array. Proses ini memiliki kompleksitas waktu **O(n)** dan kompleksitas ruang **O(1)** karena tidak membuat struktur baru.
<br></br>
3. Program kemudian menghitung jumlah mahasiswa yang lulus dan tidak lulus dengan melakukan iterasi pada setiap nilai yang ada dalam array dan mengecek apakah nilai itu lebih besar atau sama dengan (>=) 60, sehingga memerlukan pemeriksaan setiap nilai secara satu per satu, maka kompleksitas waktunya adalah **O(n)** dan karena hanya menggunakan dua variabel penghitung maka kompleksitas ruangnya adalah **O(1)**.
<br></br>
4. Untuk menampilkan grafik nilai tertinggi dan terendah, program dibuat menggunakan **Matplotlib** yang dimana proses ini akan membaca semua elemen dalam array sehingga membuat kompleksitas waktu dan ruangnya adalah **O(n)**.
<br></br>
5. Pada penampilan grafik terakhir, untuk menampilkan jumlah mahasiswa yang lulus dan tidak lulus sama-sama menggunakan **Matplotlib** tetapi karena hanya menggunakan dua data saja, maka kompleksitas waktu dan ruangnya adalah **O(1)**.

## 📚 REFLEKSI PEMBELAJARAN
Melalui pembelajaran tentang struktur data, khususnya list dan array, saya mulai memahami bagaimana data dapat disimpan, diorganisasi, dan diolah secara lebih terstruktur. Materi ini membantu saya menyadari bahwa struktur data memiliki peran penting dalam menentukan efisiensi suatu program. Saya mempelajari bahwa array menyimpan elemen dengan tipe data yang sama secara berurutan di memori, sehingga memungkinkan proses akses data dilakukan secara langsung dengan kompleksitas waktu O(1). Namun, saya juga memahami bahwa beberapa operasi seperti penambahan atau penghapusan elemen di tengah array dapat memerlukan proses pergeseran data sehingga kompleksitasnya menjadi O(n).
