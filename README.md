# Ujian Akhir Semester 
<br>Mata Kuliah  : Dasar Pemrograman
<br>Nama  : Muhammad Arkan Raihan
<br>NIM		:	1227050085
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
	Array adalah koleksi data dimana setiap elemen memakai nama yang sama dan bertipe sama dan setiap elemen diakses dengan membedakan indeks arraynya.
Untuk Deklarasi Array, Untuk Variabel array dideklarasikan dengan mencantumkan tipe dan nama variable yang diikuti dengan banyaknya lokasi memori yang ingin dibuat. 
Contoh :  
- int a[4];    = array 1 dimensi
- int b[2][3]; = array 2 dimensi

<b> Array dua dimensi merupakan array yang terdiri dari m buah baris dan n buah kolom.
Bentuknya dapat berupa matriks atau tabel. Sebenarnya array dua dimensi adalah sebuah array yang ada di dalam array.
Misalnya: ada sebuah array dua dimensi dengan ukuran 2 x 2 maka pada sebuah tempat sel pertama akan ada sebuah array satu dimensi di dalamnya.
  Sehingga gambaran secara lebih mudah untuk merepresentasikan array dua dimensi sebagai berikut.
Menampilkan elemen matriks dapat dilakukan dengan menggunakan pengulangan.
Syaratnya: matriks harus sudah diisi agar dapat ditampilkan isinya.
  Pada UAS Dasar Pemrograman Semester 1 UIN SGD Bandung 2022, Saya diberikan 2 soal antara lain :
1. Membuat Program Tukar Colom, Baris & Menjadi Baris, Colom.
2. Program Menampilkan Bilangan Yang Habis Dibagi Angka 3,5,dan 7.

## Source Code
No.1 Membuat Program Tukar Colom, Baris & Menjadi Baris, Colom
      #include <iostream>
      using namespace std;

      int main()
      {
          cout << endl;
          cout << " Nama  : Muhammad Arkan Raihan " << endl;
          cout << " NIM   : 1227050085 " << endl;
          cout << " Kelas : IF-B " << endl
               << endl;
          cout << " ===== Program Perkalian Matrix Ordo 2 ===== " << endl;
          cout << endl;
          double a[100][100];
          int i, j, k, baris, colom;
          cout << " - Masukan Baris = ";
          cin >> baris;
          cout << " - Masukan Colom = ";
          cin >> colom;
          cout << endl;
          cout << " Elemen matriks A : " << endl;
          for (i = 0; i < baris; i++)
          {
              for (j = 0; j < colom; j++)
              {
                  cout << " Elemen matrik A baris ke-" << i << " kolom ke-" << j << ": ";
                  cin >> a[i][j];
              }
          }
          cout << endl;
          cout << " Element matriks A adalah : " << endl;
          for (i = 0; i < baris; i++)
          {
              for (j = 0; j < colom; j++)
              {
                  cout << "    " << a[i][j];
              }
              cout << endl;
          }
          cout << endl;
          cout << " Matriks yang di balik :" << endl;
          for (i = 0; i < colom; i++)
          {
              // if ()
              for (j = 0; j < baris; j++)
              {
                  cout << "    " << a[j][i];
              }
              cout << endl;
          }
          cout << endl;
          return 0;
      }

No.2 Program Menampilkan Bilangan Yang Habis Dibagi Angka 3,5,dan 7
	
	#include <iostream>
	#include <iomanip>
	using namespace std;
	int main(){
	    cout << endl;
	    cout << " Nama  : Muhammad Arkan Raihan " << endl;
	    cout << " NIM   : 1227050085 " << endl;
	    cout << " Kelas : IF-B " << endl;
	    cout << endl <<" === Program Menampilkan Bilangan Yang Habis Dibagi Angka 3,5,dan 7 === " <<endl;
		int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;
	    cout << endl <<" Input jumlah baris: "; 
		cin >> jumlahBaris;
	    cout << " Input jumlah kolom: "; 
		cin >> jumlahKolom;
	    cout << endl;
	    for(i = 0; i < jumlahBaris; i++){
		for(j = 0; j < jumlahKolom; j++){
		    cout << " Baris " <<i+1<<", Kolom "<<j+1<< " = ";
		    cin >> arr[i][j];
		}
		cout << endl;
	    }
	    cout << " Hasil input nilai : " << endl;
	    for(i = 0; i < jumlahBaris ; i++){
	    for(j = 0; j < jumlahKolom; j++){
		cout << setw(3) << arr[i][j] << " ";
	    }
	    cout << endl;
	    }
	    cout << " Hasil bilangan yang habis dibagi 3,5,7 : " << endl;
	    for(i = 0; i < jumlahBaris ; i++){
	    for(j = 0; j < jumlahKolom; j++){
		if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
		cout << setw(3) << arr[i][j] << " ";
		}
	    }
	    cout << endl;
	    }
	    cout << endl;
	}

## Output
Output No 1
![Screenshot (36)](https://user-images.githubusercontent.com/121001016/208374773-4d7bd76a-6205-4b64-aaa8-d1eeb39ca88d.png)

Output No 2
![Screenshot (38)](https://user-images.githubusercontent.com/121001016/208378291-47e2f1e3-4a37-400d-ac70-a8d0dbf1be02.png)

	
