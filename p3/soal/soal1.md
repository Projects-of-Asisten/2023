---
title: Slot Parkir
layout: home
parent: Soal
grand_parent: Praktikum 3
nav_order: 1
---

{: .highlight }
💡 _Last Update_: 21 Mei 2023

# Slot Parkir

## Deskripsi

Saat ini, Teknik Komputer sudah memiliki gedung tersendiri di Tower II dan sudah menggunakan sistem parkir yang canggih dimana sistem ini dapat memberitahu para pengunjung apakah mereka dapat memarkirkan kendaraan mereka di parkiran Tower II. Sistem ini mengecek terlebih dahulu kendaraan yang akan diparkirkan, waktu kedatangan dan kepergian kendaraan. Sistem akan menerima kendaraan yang waktu kedatangan dan perginya sesuai sehingga tidak membuat parkiran macet. Di antara pukul 24.00 dan 01.00, tidak boleh ada kendaraan yang parkir di parkiran karena akan dilakukan maitenance

## Input Format

Satu baris N (banyak kendaraan yang akan parkir) dan K (Kapasitas parkiran). Dilanjutkan N baris I (Waktu kedatangan kendaraan) dan O (Waktu pergi kendaraan)
Sample Input 0 :

```
3 2
1 10
2 5
6 9
```

Sample Input 1 :

```
3 2
1 5
2 5
3 7
```

## Constraints

1 < N < 100000

1 < K < 1000

I < 0

O < 24

## Output Format

Lancar jika parkiran tersebut memenuhi ketentuan dan tiap kendaraan dapat keluar sesuai dengan waktunya masing-masing Macet Jika terdapat kendaraan yang menghambat kendaraan lainnya

Sample Output 0

```
Lancar
```

Sample Output 1

```
Macet
```

## Template soal

Template soal bisa di-download / clone [di sini](https://github.com/wannn-one/template-praktikum-prolan)
