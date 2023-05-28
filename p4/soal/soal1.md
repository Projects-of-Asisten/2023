---
title: 異世界を旅するブディ [Isekai wo tabi suru Budi] (Inheritance)
layout: home
parent: Soal
grand_parent: Praktikum 4
nav_order: 1
---

{: .highlight }
💡 _Last Update_: 28 Mei 2023

# 異世界を旅するブディ [Isekai wo tabi suru Budi] (Inheritance)

![](../../images/isekai.png)

Download the project template here

[Download](https://github.com/Projects-of-Asisten/2023/raw/main/p4/soal/template_inheritance.zip){: .btn }

## Description

You have arrived in Lock World, where an unceasing war rages on between the Demons and Humans. The Humans are unable to gauge the strength of the Demons, leading to countless soldiers being sacrificed in fruitless attacks. The ongoing war is depleting the kingdom's resources and causing widespread poverty. To combat this, the ArchMages have decided to summon a Hero from another world using a Summoning Circle. Budi, a former overworked Computer Engineer who collapsed and woke up in Lock World, was summoned as the Hero. Budi intends to develop a simulation system for battling Demons to determine the minimum number of troops required to defeat one. This system must also ensure that the number of troops used falls within the kingdom's budget. However, Budi is NOT proficient in programming, so he needs assistance in creating this simulation.

Create a program to calculate the minimum cost combination of troops needed to attack the Demons. If the cost is above the budget of the Council, then the kingdom will surrender.

You are allowed to create an additional class for the program. However, Knight, Demon, and Council classes are mandatory. You will receive an additional 10 points for every other class you create.

Basic system with Knight, Demon, Council -- 70 point

Archer, Berserker, Golem, Mage -- 10 point each per-apply

Max at 100 point

## Expected Output

```
0A 0B 0G 10K 0M
90 Gold left
```

I takes only 10 Knight to beat the Demon, and council still has 90 Gold left

```
0A 0B 0G 50K 10M
0 Gold Left, We Surrender
```

Surrender if the kingdom can't beat the Demon with all their budget
