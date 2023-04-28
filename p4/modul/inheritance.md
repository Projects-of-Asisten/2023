---
title: Inheritance
parent: Modul
grand_parent: Praktikum 4
layout: home
---
{: .highlight }
💡 _Last Update_: 29 April 2023

# Inheritance
Inheritance atau pewarisan merupakan merupakan salah satu konsep pada C++ dimana suatu class mampu "mewariskan" atribut atau isi dari class tersebut untuk class yang lain. Konsep inheritance ini dapat diimplementasikan untuk mengurangi pengulangan kode pada program yang dibuat. Terdapat dua kategori class pada inheritance ini, yaitu derived class dan base class. Derived class yang bertindak sebagai child akan mewarisi isi dari base class. Sedangkan base class yang bertindak sebagai parent akan memberi warisan kepada child class nya.

```cpp
// Base class
class Vehicle {
  public:
    string brand = "Ford";
    void honk() {
      cout << "Tuut, tuut! \n" ;
    }
};

// Derived class
class Car: public Vehicle {
  public:
    string model = "Mustang";
};

int main() {
  Car myCar;
  myCar.honk();
  cout << myCar.brand + " " + myCar.model;
  return 0;
}
```

Penjelasan contoh di atas:
1. class Car mewarisi isi dari class Vehicle, sehingga class Car akan memiliki string brand dan method honk yang sama dengan class Vehicle.
2. public merupakan penentu akses, yang berarti isi dari class tersebut dapat diakses oleh class luar.
3. disamping mewarisi atribut string brand dari induknya (class Car), class Vehicle juga memiliki atributnya sendiri yaitu string model.
