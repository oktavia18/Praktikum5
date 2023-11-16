# Praktikum5
| Nama           |  *NIM*           | *Kelas*      |
|:---------------|:----------------:|-------------:|
|*Oktavia Rizkha.k.*  | *312310509*      |  *TI.23.A5*  |

# Latihan 1

## Input

`

# Membuat list dengan 5 elemen
my_list = [1, 2, 3, 4, 5]

#AKSES LIST
# Mengakses dan menampilkan elemen ke-3
print("Elemen ke-3:", my_list[2])

# Mengambil nilai elemen ke-2 sampai elemen ke-4
subset_list = my_list[1:4]
print("Nilai elemen ke-2 sampai elemen ke-4:", subset_list)

# Mengambil elemen terakhir
last_element = my_list[-1]
print("Elemen terakhir:", last_element)

#UBAH ELEMENT LIST
#ubah elemen ke 4 dengan nilai lainnya
my_list[3] = 60
print("Setelah mengubah elemen ke-4:", my_list)

#ubah elemen ke 4 sampai dengan elemen terakhir
my_list[3:] = [60, 70]
print("Setelah mengubah nilai elemen ke-4 sampai elemen terakhir:", my_list)

#TAMBAH ELEMENT LIST
# Buat list pertama (A)
A = [1, 2, 3, 4, 5]
# Ambil 2 bagian dari list pertama (A) dan jadikan list kedua (B)
B = A[:2]
print("List B:", B)

# Tambahkan list B dengan nilai string
B.append("Hello")
print("List B:" , B)

# Tambahkan list B dengan 3 nilai
B.extend([3, 4, 5])
print("List B:", B)

# Gabungkan list B dengan list A
C = B + A
print("List C (gabungan A dan B):", C)

`

## Output

![alt text](https://github.com/oktavia18/Praktikum5/blob/master/ss/output%20latihan%201.png?raw=true)


## Penjelasan

1. List pertama (list_A) diinisialisasi dengan nilai [1, 2, 3, 4, 5].
2. Dua bagian pertama dari list_A diambil dan disalin ke list_B menggunakan slicing (list_A[:2]).
3. Tiga nilai string ("string1" dan "string2") ditambahkan ke list_B menggunakan metode append.
4. Tiga nilai (3, 4, dan 5) ditambahkan ke list_B menggunakan metode extend.
5. List B (list_B) sekarang berisi dua bagian pertama dari list A, dua nilai string, dan tiga nilai tambahan.
6. List B (list_B) kemudian digabungkan ke list A (list_A) menggunakan metode extend.
7. Hasilnya dicetak untuk dilihat.

# Praktikum 4

## Input


`
# LIST

nama = []
nim = []
nilaiTugas = []
nilaiUTS = []
nilaiUAS = []
nilaiAkhir = []

print()

# Input

while True:
nama.append(input("Masukan nama : "))
nim.append(input("Masukan NIM : "))
Tugas = int(input("Nilai Tugas : "));
nilaiTugas.append(Tugas)
UTS = int(input("Nilai UTS : "));
nilaiUTS.append(UTS)
UAS = int(input("Nilai UAS : "));
nilaiUAS.append(UAS)

    nilaiAkhir.append(Tugas * 30/100 + UTS * 35/100 + UAS * 35/100)

    print()
    _tanya = input("Tambah data ? [y/t]: ")
    print()
    if(_tanya == "t"):
        break

# Output

print("+----+-----------------------+--------+--------+-------+-------+---------+")
print("| {0:^2} | {1:^18} | {2:^9} | {3:^6} | {4:^5} | {5:^5} | {6:^7} |".format("No", "Nama", "NIM", "Tugas", "UTS", "UAS", "Akhir"))
print("-----+-----------------------+--------+--------+-------+-------+---------+")

no = 0
for nama, nim, Tugas, UTS, UAS, nilaiAkhir in zip(nama, nim, nilaiTugas, nilaiUTS, nilaiUAS, nilaiAkhir):
no += 1  
 print("| {0:>2} | {1:<18} | {2:>8} | {3:>6} | {4:>5} | {5:>5} | {6:>7} |".format(no, nama, nim, Tugas, UTS, UAS, nilaiAkhir))
print("+----+-----------------------+--------+--------+-------+-------+---------+")

`

## Output

![alt text](https://github.com/oktavia18/Praktikum5/blob/master/ss/output%20tugas%202.png?raw=true)


## Flowchart

![alt text](https://github.com/oktavia18/Praktikum5/blob/master/FLOWCHART%20PERTEMUAN%209.pdf?raw=true)


## Penjelasan

1. Program dimulai dengan menginisialisasi list data_mahasiswa untuk menyimpan data mahasiswa.
2. Didefinisikan fungsi hitung_nilai_akhir untuk menghitung nilai akhir berdasarkan proporsi yang diberikan.
3. Program menggunakan perulangan while True untuk terus meminta input data.
4. Pengguna diminta untuk memasukkan nama, nilai tugas, nilai UTS, dan nilai UAS.
5. Nilai akhir dihitung menggunakan fungsi hitung_nilai_akhir dan data dimasukkan ke dalam list.
6. Program menanyakan apakah pengguna ingin menambahkan data lagi, dan perulangan berlanjut jika jawabannya 'y'.
7. Setelah selesai memasukkan data, program menampilkan daftar data mahasiswa dalam format tabel sederhana.
