Nama  : Febri Tri Arei Sakti

Nim   : 312210542

Kelas : TI22B2

Tugas : Praktikum 5


1. Membuat dictionary data

2. Membuat menu pilihan (A)dd (E)dit (D)elete (S)earch (L)ist (Q)uit

A. Untuk pilihan A meninput Nama, Nim, Tugas, Uts dan Uas. jika nilai nama, nim, tugas, uts, dan uas kosong maka program ValueError dan meminta untuk input ulang. dan untuk data yg sudah di tambahkan menggunakan key nama.

Kode Program :

```
    elif c.lower() == 'a':
        print ("\nMasukan Data Mahasiswa")

        while (True):
            nama = input("NAMA : ")
            if nama == '':
                print ('Nama tidak boleh kosong')
            else:
                break
        while (True):
            try:
                nim  = int(input("NIM  : "))
                if nim == '':
                    print ('Masukan Nim dengan Angka')
            except ValueError:
                print ('Masukan Nim dengan Angka')
            else:
                break
        while (True):
            try:
                tugas  = int(input("TUGAS  : "))
                if tugas == '':
                    print ('Masukan TUGAS dengan Angka')
            except ValueError:
                print ('Masukan TUGAS dengan Angka')
            else:
                break
        while (True):
            try:
                uts  = int(input("UTS  : "))
                if uts == '':
                    print ('Masukan UTS dengan Angka')
            except ValueError:
                print ('Masukan UTS dengan Angka')
            else:
                break
        while (True):
            try:
                uas  = int(input("UAS  : "))
                if uas == '':
                    p('Masukan UAS dengan Angka')
            except ValueError:
                print ('Masukan UAS dengan Angka')
            else:
                break
        akhir = round((float(tugas) * 0.3)+(float(uts) * 0.35)+(float(uas) * 0.35),2)
        data[nama] = [nama,nim,tugas,uts,uas,akhir]
        ```
        Hasli program :

![image]![image](https://user-images.githubusercontent.com/115480501/204195327-41275356-6f0d-41cb-ad73-9af688493ff8.png)

