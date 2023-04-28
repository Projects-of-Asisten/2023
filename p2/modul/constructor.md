---
title: Constructor
parent: Modul
grand_parent: Praktikum 2
layout: home
---
{: .highlight }
💡 _Last Update_: 29 April 2023

# Constructors
Constructors di C++ adalah metode khusus yang secara otomatis dipanggil saat objek kelas dibuat. Untuk membuat Constructors, gunakan nama yang sama dengan kelas, diikuti tanda kurung ():

```cpp
#include <iostream>
using namespace std;

class MyClass {     // Class
    public:           // Access specifier
    MyClass() {     // Constructor
      cout << "Hello World!";
    }
};

int main() {
  MyClass myObj;    // membuat object baru sMyClass 
                    //ini yang disebut dengan constructor
  return 0;
}
```

## Constructors Parameter
Constructors juga dapat mengambil parameter (seperti fungsi biasa), yang berguna untuk mengatur nilai awal suatu atribut. Kelas berikut memiliki atribut merek, model dan tahun, serta Constructors dengan parameter yang berbeda. Di dalam Constructors, dibuat atribut yang sama dengan parameter Constructors (merek=x, dll). Saat memanggil Constructors (dengan membuat objek kelas),  meneruskan parameter ke Constructors, yang akan dibuat dengan nilai atribut yang sesuai.

```cpp
#include <iostream>
using namespace std;
class Car {        // The class
  public:          // Access specifier
    string brand;  // Attribute untuk brand mobil
    string model;  // Attribute untuk model mobil
    int year;      // Attribute untuk tahun mobil
    Car(string x, string y, int z) { // Constructor with parameters
      brand = x;
      model = y;
      year = z;
    }
};

int main() {
  // Create Car objects and call the constructor with different values
  Car carObj1("BMW", "X5", 1999);
  Car carObj2("Ford", "Mustang", 1969);

  // Print values
  cout << carObj1.brand << " " << carObj1.model << " " << carObj1.year << "\n";
  cout << carObj2.brand << " " << carObj2.model << " " << carObj2.year << "\n";
  return 0;
}
```

Dapat dilihat pada codingan di atas pada bagian `int main()...`, dipanggil class yaitu Car dengan objek yaitu carObj1. Di dalem objek terdapat parameter brand atau x yang diisi dengan "BMW", model atau y yang diisi dengan "X5", dan year atau z yang diisi dengan "1999". Lalu pada print value, ditiap output parameter diberi spasi " ".