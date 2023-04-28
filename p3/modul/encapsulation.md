---
title: Encapsulation
parent: Modul
grand_parent: Praktikum 3
layout: home
---
{: .highlight }
💡 _Last Update_: 29 April 2023

# Encapsulation
Encapsulation adalah cara untuk memastikan data "sensitif" disembunyikan dari pengguna. Agar data tersebut dapat disembunyikan, variabel/atribut dideklarasikan sebagai private(tidak dapat diakses dari luar kelas). Untuk mengubah atau melihat nilai dari variabel/atribut private dapat menggunakan metode get dan set public.

```cpp
#include <iostream>
using namespace std;

class Employee {
  private:
    // Private attribute
    int salary;

  public:
    // Setter
    void setSalary(int s) {
      salary = s;
    }
    // Getter
    int getSalary() {
      return salary;
    }
};

int main() {
  Employee myObj;
  myObj.setSalary(50000);
  cout << myObj.getSalary();
  return 0;
}
```

Penjelasan contoh di atas:
1. atribut "salary" merupakan atribut private, yang memiliki akses terbatas
2. fungsi setSalary() menggunakan paramater (s) yang mengarah ke atribut "salary"
3. fungsi getSalary() mengeluarkan nilai dari atribut "salary" yang merupakan atribut private
4. didalam main(), dibuat sebuah objek didalam class Employee. Fungsi setSalary() digunakan untuk mengisi nilai atribut "salary" dengan nilai 50000. Kemudian nilai dari "salary" dapat dikeluarkan dengan fungsi getSalary().