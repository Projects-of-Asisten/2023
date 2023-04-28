---
title: Access Specifiers
parent: Modul
grand_parent: Praktikum 3
layout: home
---
{: .highlight }
💡 _Last Update_: 29 April 2023

# Access Specifiers
Perhatikan syntax class c++ berikut!

```cpp
class MyClass {  // Class
  public:        // Access specifier
    // member suatu class ada di sini
};
```

Access Specifiers di C++ adalah bagaimana suatu method dan member suatu class diakses. Pada contoh di atas, member suatu class maupun method-nya bisa diakses secara public (Bisa diakses dari luar class secara langsung).

Lalu bagaimana caranya kita membuat member class agar hanya bisa diakses dari dalam class saja?

Dalam C++, terdapat 3 jenis access specifiers, yaitu:

| Modifier | Deskripsi |
|:----------|:------------------|
| Public | Member dapat diakses di luar class |
| Private | Member tidak dapat diakses di luar class |
| Protected | Sama seperti private, namun bisa diakses di class turunannya (Inherited Class, bab selanjutnya akan membahas inheritance) |

Berikut adalah contoh penggunaan dan perbedaan antara penggunaan access specifiers secara public dan private

```cpp
#include <iostream>

class MyClass {
    public:    // Public access specifier
        int x;   // Public attribute
    private:   // Private access specifier
        int y;   // Private attribute
};

int main() {
    MyClass myObj;
    myObj.x = 25;  // Diperbolehkan (public)
    myObj.y = 50;  // Tidak diperbolehkan (private)
    std::cout << myObj.x << std::endl; // Output = 25
    std::cout << myObj.y << std::endl; // Compilation error
    return 0;
}
```

