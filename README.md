# Ujian Akhir Semester 
<br>Mata Kuliah     : Dasar Pemrograman
<br> Nama           : Moohammad Putra Fauzan Fatah
<br>NIM		          :	1227050075
<br>Jurusan		      :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
   Program kali ini saya membuat array. Apa itu array? Array adalah larik yang berisi kumpulan data dengan tipe serupa. Teknologi ini dapat digunakan untuk mempermudah penghitungan data karena mengelompokkan data-data berdasarkan kesamaannya. Untuk mempermudah pemahaman Anda mengenai hal ini, simak analogi berikut.

Misalnya, sebuah kereta terdiri dari beberapa gerbong yang menyimpan barang bawaan di dalamnya. Barang bawaan tersebut sama artinya dengan sekelompok data dengan tipe yang sama, sedangkan kereta tersebut adalah apa yang disebut dengan array itu sendiri. Kereta menampung barang-barang yang memiliki kesamaan nilai, sama seperti array yang memuat data-data dengan kemiripan tertentu.

Saya membuat 2 program yaitu program transpose array dan program bilangan yang habis dibagi 3.
<br> Berikut adalah code atau syntax nya.
## Source Code

<b>PROGRAM TRANSPOSE ARRAY<b>

```
#include <iostream>
<br> #include <iomanip>
<br> using namespace std;

int main() {
	
	cout<<endl;
	cout<<"---------------------------------------------"<<endl;
	cout<<"Nama 		: Mohammad Putra Fauzan Fatah"<<endl;
	cout<<"NIM		: 1227050075 "<<endl;
	cout<<"Jurusan 	: Teknik Informatika"<<endl;
	cout<<"---------------------------------------------"<<endl;
	cout<<endl;
	cout<<"Program Transpose Array 2 Dimensi"<<endl;
	int arr[100][100], transpose[100][100], baris, kolom;
	
	cout << "Masukan jumlah baris: "; cin >> baris;
	cout << "Masukan jumlah kolom: "; cin >> kolom;
	
	for(int i=0; i<baris; i++){
		for(int j=0; j<kolom; j++){
			cout << "arr ke["<<i<<j<<"]: "; cin >> arr[i][j];
		}
	}
	
	cout << endl;
	
	for(int i=0; i<baris; i++){
		for(int j=0; j<kolom; j++){
			cout << arr[i][j] << " ";
			if(j == kolom - 1);
		}
		cout << endl;
	}
	
	cout << endl;
	
	for(int i=0; i<baris; i++){
		for(int j=0; j<kolom; j++){
			transpose[j][i] = arr[i][j];
		}
	}
	
	cout << "Hasil transpose " << endl;
	for(int i=0; i<kolom; i++){
		for(int j=0; j<baris; j++){
			
			cout << transpose[i][j] << " ";
			if(j == baris - 1);
		}
		cout << endl;
	}
	
	
}
```
	
<b>PROGRAM ARRAY HABIS DI BAGI 3,5,7<b>
```
<br>#include <iostream>
<br>#include <iomanip>
<br>using namespace std;
	
int main(){

    cout<<endl;
	cout<<"---------------------------------------------"<<endl;
	cout<<"Nama 		: Mohammad Putra Fauzan Fatah"<<endl;
	cout<<"NIM		: 1227050075 "<<endl;
	cout<<"Jurusan 	: Teknik Informatika"<<endl;
	cout<<"---------------------------------------------"<<endl;
	cout<<endl;
	cout<<"Program Transpose Array 2 Dimensi"<<endl;
 	int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

    cout<<"Input jumlah baris: "; cin>>jumlahBaris;
    cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
    cout << endl;

    for(i = 0; i < jumlahBaris; i++){
        for(j = 0; j < jumlahKolom; j++){
            cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
            cin >> arr[i][j];
        }
        cout << endl;
    }

    cout << "Hasil input nilai : " << endl;

    for(i = 0; i < jumlahBaris ; i++){
    for(j = 0; j < jumlahKolom; j++){
        cout << setw(3) << arr[i][j] << " ";
    }
    cout << endl;
    }

    cout << "\nHasil bilangan yang tidak bisa dibagi 3,5,7 : " << endl;

    for(i = 0; i < jumlahBaris ; i++){
    for(j = 0; j < jumlahKolom; j++){
        if(arr[i][j] % 3 == 0 || arr[i][j] % 5 || arr[i][j] % 7 == 0){
        cout << setw(3) << arr[i][j] << " ";
        }
    }
    cout << endl;
    }

    
    cout << endl;
    return 0;
}
```	

## Output
<b>PROGRAM TRANSPOSE ARRAY<b>
	
<img width="675" alt="Transpose" src="https://user-images.githubusercontent.com/90183052/208379003-99597e9a-cd15-445b-b856-7b4c82409e53.PNG">

<b>PROGRAM ARRAY HABIS DI BAGI 3,5,7<b>

