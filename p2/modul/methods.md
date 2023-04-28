---
title: C++ Class Methods
parent: Modul
grand_parent: Praktikum 2
layout: home
---
{: .highlight }
💡 _Last Update_: 29 April 2023

# C++ Class Methods
Method adalah sebuah fungsi yang dimiliki oleh class. Ada dua cara untuk mendefinisikan fungsi yang dimiliki oleh class.
1. Di dalam definisi class
2. Di luar definisi class

Untuk mengakses method sama seperti mengakses atribut, yaitu dengan membuat objek di dalam class dan menggunakan sintaks titik (.).

Contoh di bawah ini mendefinisikan sebuah fungsi di dalam kelas yang dinamakan "myMethod".

```cpp
class MyClass {        // class
  public:              // Access specifier
    void myMethod() {  // Method / fungsi yang didefinisikan di dalam class
      cout << "Hello World!";
    }
};

int main() {
  MyClass myObj;     // Membuat objek di dalam class yang bernama MyClass
  myObj.myMethod();  // Panggil method
  return 0;
}
```

Untuk mendefinisikan fungsi di luar definisi class, deklarasikan di dalam class kemudian definisikan di luar class. Hal ini dapat dilakukan dengan menspesifikasikan nama dari class diikuti dengan operator (::) diikuti dengan nama dari fungsi.

```cpp
class MyClass {        // class
  public:              // Access specifier
    void myMethod();   // Deklarasi method / fungsi
};

// Definisi method / fungsi di luar class
void MyClass::myMethod() {
  cout << "Hello World!";
}

int main() {
  MyClass myObj;     // Membuat objek untuk MyClass
  myObj.myMethod();  // Memanggil method
  return 0;
}
```

Method juga dapat ditambahkan parameter.

```cpp
#include <iostream>
using namespace std;

class Car {
  public:
    int speed(int maxSpeed);
};

int Car::speed(int maxSpeed) {
  return maxSpeed;
}

int main() {
  Car myObj; // Membuat objek Car
  cout << myObj.speed(200); // Panggil method dengan sebuah argumen
  return 0;
}
```