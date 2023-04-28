---
title: Polymorphism
parent: Modul
grand_parent: Praktikum 4
layout: home
---
{: .highlight }
💡 _Last Update_: 29 April 2023

# Polymorphism
Polymorphism berarti "banyak bentuk", dan itu terjadi ketika kita memiliki banyak class yang terkait satu sama lain melalui inheritance.

Seperti yang kita pelajari di bab sebelumnya, Inheritance memungkinkan class untuk mewarisi attribute dan method dari class lain. Polymorphism menggunakan metode tersebut untuk melakukan hal yang berbeda. Hal ini memungkinkan kita untuk melakukan satu tindakan dengan cara yang berbeda.

Semisal terdapat base class yang disebut Animal yang memiliki method yang disebut animalSound(). Derived class dari Animal dapat berupa Pig, Cat, Dog, Bird - Dan mereka juga memiliki penerapan suara binatang sendiri (suara babi, dan kucing mengeong, dll.):

```cpp
// Base class
class Animal {
  public:
    void animalSound() {
      cout << "The animal makes a sound \n";
    }
};

// Derived class
class Pig : public Animal {
  public:
    void animalSound() {
      cout << "The pig says: wee wee \n";
    }
};

// Derived class
class Dog : public Animal {
  public:
    void animalSound() {
      cout << "The dog says: bow wow \n";
    }
};
```

Dengan polymorphism ini, kita dapat membuat method yang memiliki nama serupa, dan kita dapat 'menimpa' method animalSound() milik class Animal.

```cpp
// Base class
class Animal {
  public:
    void animalSound() {
      cout << "The animal makes a sound \n";
    }
};

// Derived class
class Pig : public Animal {
  public:
    void animalSound() {
      cout << "The pig says: wee wee \n";
    }
};

// Derived class
class Dog : public Animal {
  public:
    void animalSound() {
      cout << "The dog says: bow wow \n";
    }
};

int main() {
  Animal myAnimal;
  Pig myPig;
  Dog myDog;

  myAnimal.animalSound(); // Output : The animal makes a sound
  myPig.animalSound(); // Output : The pig says: wee wee
  myDog.animalSound(); // Output : The dog says : bow bow
  return 0;
}
```