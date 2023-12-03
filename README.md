# tugaspraktikum7

Inisialisasi Dictionary:

python
Copy code
daftar_nilai = {}
Dictionary daftar_nilai digunakan untuk menyimpan data nilai mahasiswa, di mana kunci adalah nama mahasiswa dan nilai adalah nilai yang diperoleh.

Fungsi tambah(nama, nilai):

python
Copy code
def tambah(nama, nilai):
    daftar_nilai[nama] = nilai
    print(f"Data mahasiswa dengan nama {nama} dan nilai {nilai} telah ditambahkan.")
Fungsi ini memungkinkan penambahan data baru ke dalam daftar_nilai. Data baru ditambahkan dengan menggunakan nama sebagai kunci dan nilai sebagai nilainya ke dalam dictionary. Kemudian, pesan konfirmasi akan dicetak.

Fungsi tampilkan():

python
Copy code
def tampilkan():
    if daftar_nilai:
        print("Daftar Nilai Mahasiswa:")
        for nama, nilai in daftar_nilai.items():
            print(f"{nama}: {nilai}")
    else:
        print("Daftar nilai mahasiswa kosong.")
Fungsi ini digunakan untuk menampilkan semua data nilai mahasiswa yang ada dalam daftar_nilai. Jika daftar_nilai tidak kosong, maka akan mencetak nama dan nilai setiap mahasiswa. Jika kosong, akan mencetak pesan bahwa daftar nilai kosong.

Fungsi hapus(nama):

python
Copy code
def hapus(nama):
    if nama in daftar_nilai:
        del daftar_nilai[nama]
        print(f"Data mahasiswa dengan nama {nama} telah dihapus.")
    else:
        print(f"Tidak ditemukan data mahasiswa dengan nama {nama}.")
Fungsi ini memungkinkan penghapusan data mahasiswa berdasarkan nama. Jika nama mahasiswa ditemukan dalam daftar_nilai, data mahasiswa tersebut akan dihapus dari dictionary. Jika tidak ditemukan, akan mencetak pesan bahwa nama mahasiswa tidak ditemukan.

Fungsi ubah(nama, nilai_baru):

python
Copy code
def ubah(nama, nilai_baru):
    if nama in daftar_nilai:
        daftar_nilai[nama] = nilai_baru
        print(f"Data mahasiswa dengan nama {nama} telah diubah menjadi nilai {nilai_baru}.")
    else:
        print(f"Tidak ditemukan data mahasiswa dengan nama {nama}.")
Fungsi ini memungkinkan perubahan nilai mahasiswa berdasarkan nama. Jika nama mahasiswa ditemukan dalam daftar_nilai, nilai mahasiswa tersebut akan diubah sesuai dengan nilai baru yang diberikan. Jika tidak ditemukan, akan mencetak pesan bahwa nama mahasiswa tidak ditemukan.

Contoh Penggunaan Fungsi-fungsi:

python
Copy code
tambah("Alice", 85)
tambah("Bob", 90)
tambah("Charlie", 78)

tampilkan()

hapus("Bob")

ubah("Alice", 95)

tampilkan()
Di bagian ini, contoh penggunaan fungsi-fungsi tersebut diberikan. Data ditambahkan untuk tiga mahasiswa, kemudian daftar nilai ditampilkan. Setelah itu, data untuk mahasiswa "Bob" dihapus, nilai mahasiswa "Alice" diubah, dan akhirnya, daftar nilai diperbarui dan ditampilkan kembali.
