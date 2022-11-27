# praktikum 6

## Dictionary

### •	Membuat Dictionary

### a = {} # empty dict

### a = ['n1': 100, 'n2': 20, 'n3': 7] # dict with key:value

### •	Mengakses Dictionary

#### print(a['n2']) # print element with key 'n2'
#### print(a.keys()) # print all key from dict
#### print(a.values()) # print all value form dict
#### print(a.items()) # print list of tuple(key, value) form dict

### •	Mengubah elemen Dictionary


#### a['n2'] = 10 # change the item for key 'n2'

### •	Menambahkan elemen Dictionary
![6 1](https://user-images.githubusercontent.com/115569493/204135638-95b37d55-216c-4c7e-a425-3dcbab48b2b6.png)

#### a['n4'] # add item with key 'n4'

### •	Loop Dictionary

#### for item in a.items():
#### print(item) # print tuple (key, value)
#### print(item[0]) # print key item

## Latihan 1
Buat Dictionary daftar kontak
### •	Nama sebagai Key dan Nomor sebagai Value
telp = {}
telp['Ari'] = '081267888'
telp['Dina'] = '087677776'

### •	Tampilkan kontaknya Ari
print(telp['Ari'])
### •	Tambah kontak baru dengan nama Riko, nomor 087654544
telp['Riko'] = '087654544'
### •	Ubah kontak Dina dengan nomor baru 088999776
telp['Dina'] = '088999776'
### •	Tampilkan semua Nama
print(telp.keys())
### •	Tampilkan semua Nomor
print(telp.values())
### •	Tampilkan daftar Nama dan nomornya
print(telp.items())

![6 2](https://user-images.githubusercontent.com/115569493/204135813-c8a36177-5720-4d2a-9878-abbb6b049cac.png)

![6 3](https://user-images.githubusercontent.com/115569493/204135860-1a7dc7ff-906a-4e72-b0db-fc3c2cef1616.png)

# Tugas Praktikum

### Daftar Nilai Mahasiswa Menggunakan Dictionary
#### Pertama kita membuat sebuah dictionary kosong yang nantinya akan diinputkan data ketika program dijalankan.
#### Data = {}
#### Lalu kita membuat kondisi perulangan dan sebuah keterangan untuk pilihan menu yang akan menjalankan program.
#### while True:
   #### List = input("\n(T)ambah, (U)bah, (H)apus, (C)ari, (L)ihat, (K)eluar: ")
#### Membuat syntax untuk menambahkan data.
#### if List.lower() == 't':
        print("Tambah Data")
        nama = input("Nama           : ")
        nim = int(input("NIM            : "))
        tugas = int(input("Nilai Tugas    : "))
        uts = int(input("Nilai UTS      : "))
        uas = int(input("Nilai UAS      : "))
        akhir = tugas*30/100 + uts*35/100 + uas*35/100
        Data[nama] = nim, tugas, uts, uas, akhir
