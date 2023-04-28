---
title: C++ Classes/Objects
parent: Modul
grand_parent: Praktikum 1
layout: home
---
{: .highlight }
💡 _Last Update_: 29 April 2023

# C++ Classes/Objects
C++ adalah bahasa pemrograman yang berorientasi objek. Segala sesuatu dalam C ++ dikaitkan dengan kelas dan objek, bersama dengan atribut dan metodenya. Misalnya: dalam kehidupan nyata, mobil adalah objek. Mobil memiliki atribut, seperti berat dan warna, dan metode, seperti drive dan rem. Atribut dan metode pada dasarnya adalah variabel dan fungsi yang dimiliki kelas. Ini sering disebut sebagai "anggota kelas".
Kelas adalah tipe data yang ditentukan pengguna yang dapat kami gunakan dalam program kami, dan berfungsi sebagai konstruktor objek, atau "blueprint" untuk membuat objek. berikut adalah cara membuat sebuah class

```cpp
#include <iostream>
using namespace std;

class MyClass {       // The class
  public:             // Access specifier
    int myNum;        // Attribute (int variable)
    string myString;  // Attribute (string variable)
};
```

Penjelasan contoh di atas
1. Kata kunci class digunakan untuk membuat kelas bernama MyClass
2. Kata kunci publik adalah penentu akses, yang menetapkan bahwa anggota (atribut dan metode) kelas dapat diakses dari luar kelas. Anda akan mempelajari lebih lanjut tentang penentu akses nanti
3. Di dalam kelas, ada variabel integer myNum dan variabel string myString. Ketika variabel dideklarasikan dalam kelas, mereka disebut atribut
4. Terakhir, akhiri definisi kelas dengan titik koma (;)

## Membuat sebuah Object

Di C++, objek dibuat dari kelas. Kami telah membuat kelas bernama MyClass, jadi sekarang kami dapat menggunakan ini untuk membuat objek. Untuk membuat objek MyClass, tentukan nama kelas, diikuti dengan nama objek. Untuk mengakses atribut kelas (myNum dan myString), gunakan sintaks titik (.) pada objek:

```cpp
#include <iostream>
using namespace std;


class MyClass {       // The class
  public:             // Access specifier
    int myNum;        // Attribute (int variable)
    string myString;  // Attribute (string variable)
};

int main() {
  MyClass myObj;  // Create an object of MyClass

  // Access attributes and set values
  myObj.myNum = 15; 
  myObj.myString = "Some text";

  // Print attribute values
  cout << myObj.myNum << "\n";
  cout << myObj.myString;
  return 0;
}
```

Anda dapat membuat banyak objek dari satu kelas:
```cpp
#include <iostream>
using namespace std;

// Create a Car class with some attributes
class Car {
  public:
    string brand;   
    string model;
    int year;
};

int main() {
  // Create an object of Car
  Car carObj1;
  carObj1.brand = "BMW";
  carObj1.model = "X5";
  carObj1.year = 1999;

  // Create another object of Car
  Car carObj2;
  carObj2.brand = "Ford";
  carObj2.model = "Mustang";
  carObj2.year = 1969;

  // Print attribute values
  cout << carObj1.brand << " " << carObj1.model << " " << carObj1.year << "\n";
  cout << carObj2.brand << " " << carObj2.model << " " << carObj2.year << "\n";
  return 0;
}
```