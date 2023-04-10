# Latihan2-XAMPP

#### Nama  : Muhamad Abdul Anas
#### Nim   : 312210269
#### Kelas :TI.22.A2

1. Buat sebuah database dengan nama latihan2!
CREATE DATABASE latihan2;

![image](https://user-images.githubusercontent.com/115569493/230861992-247724e5-23fd-4fa2-a020-c501a602065e.png)

2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan1!
CREATE TABLE siswa (nama VARCHAR(100), alamat TEXT);

![image](https://user-images.githubusercontent.com/115569493/230862316-5606347f-6cf3-4a93-98e8-61f1a5204a1a.png)

3. tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom trakhir.
untuk menambahkan kolom terakhir yaitu deangan sering digunakan kata after, contoh:

alter table biodata add column keterangan varchar (15) after phone;

![image](https://user-images.githubusercontent.com/115569493/230863415-86dece5c-cee0-476a-83fb-c636caf18751.png)

4. tambahkan kolom id(int11) di awal (sebagai kolom pertama).
untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut:

alter table biodata add column id(int11) first;

![image](https://user-images.githubusercontent.com/115569493/230863620-55ea3fd8-522c-40bf-a77b-863dea8cca28.png)

5. sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat.
untuk menambahkan kolom setelah kolom lain yaitu dengan perintah after

![image](https://user-images.githubusercontent.com/115569493/230864032-d1f9bffc-0571-42cb-8e1f-7fe7898ee59c.png)

6. ubah tipe data kolom id menjadi char(11).
untuk mengubah type data yaitu dengan perintah sebagai berikut:

alter table [nama_table] modify nama_field tipe_data_baru(ukuran);

![image](https://user-images.githubusercontent.com/115569493/230864174-2ad9a579-55de-4efb-b926-b0c83efae3e4.png)

7. ubah nama kolom phone menjadi hp(varchar20).
untuk mengubah kolom yaitu dengan perintah sebagai berikut:

ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);

![image](https://user-images.githubusercontent.com/115569493/230864776-98d28e36-166f-413f-af6a-f8a095b89c83.png)

8. tambahkan kolom email setelah kolom hp

![image](https://user-images.githubusercontent.com/115569493/230864859-71491baf-98f8-4f76-809d-004f1ed506a7.png)

9. hapus kolom keterangan dari table.
untuk menghapus kolom dari dable yaitu dengan perintah sebagai beri
kut:

alter table [nama_table] drop_field;

![image](https://user-images.githubusercontent.com/115569493/230865094-c422a1d7-f88b-44e0-980d-6464e729ab29.png)

10. ganti nama table menjadi data_mahasiswa.
untuk mengganti nama table yaitu dengan perintah sebagai berikut:

alter table [nama_table] rename [nama_table_baru]

![image](https://user-images.githubusercontent.com/115569493/230865183-b1e89e7d-08d6-4c53-bf82-43facaafb0ea.png)

11. ganti nama field id menjadi nim

![image](https://user-images.githubusercontent.com/115569493/230865302-ea362cbb-6e5f-4bee-8dbe-7cd6d871b393.png)

12. jadikan nim sebagai primary key.
untuk menambahkan index atau key, gunakan perintah sebagai berikut: -tipe -primary key -unique key -fulltext

ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);

![image](https://user-images.githubusercontent.com/115569493/230865530-632ea5f2-892c-4b23-83d6-329592bb4dd3.png)

13. jadikan kolom email sebagai
perintahnya sama seperti diatas, hanya saja diganti menjadi unique key.

![image](https://user-images.githubusercontent.com/115569493/230865840-de7717b9-87ef-4b32-8fb8-58b2dcf7f20e.png)

Evaluasi dan pertanyaan
Apa maksud dari int (11)?
int (11) nunjukkan bahwa kolom memiliki tipe data bilangan bulat (integer) dengan ukuran 11 digit 
Ketika kita melihat struktur tabel dengan perintah desc, ada kolom Null yang berisi Yes dan No. Apa maksudnya ?
Jika kolom "Null" adalah "YES", itu berarti kolom tersebut diizinkan untuk memiliki nilai NULL.

Jika kolom "Null" adalah "NO", maka kolom tersebut tidak diizinkan untuk memiliki nilai NULL





