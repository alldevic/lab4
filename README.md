# Лабораторная работа №4

[![Build status](https://ci.appveyor.com/api/projects/status/21whd359i7sfr91t?svg=true)](https://ci.appveyor.com/project/alldevic/lab4)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/2c5cbbec5f77424a930e1b485ad4db7b)](https://www.codacy.com/app/alldevic/lab4?utm_source=github.com&utm_medium=referral&utm_content=alldevic/lab4&utm_campaign=badger)

Реализовать перечисление перестановок методом Дейкстры.

## Дано
строка 1: перестановка P, содержащая от 1 до 10 символов из набора 0123456789

строка 2: целое неотрицательное N - сколько перестановок генерировать, начиная с P

## Вывод программы
Если первая строка не является перестановкой символов из набора 0123456789, то одна строка "bad input". Иначе - первые N (или сколько есть) перестановок после P в лексикографическом порядке, по одной перестановке в строке. Если P - последняя перестановка в лексикографическом порядке, то ничего не выводить

## Пример 1
#### Вход:
214

2
#### Выход:
241

412

## Пример 2
#### Вход:
111

1
#### Выход:
bad input

## Пример 3
#### Вход:
321

1
#### Выход:
<пустая строка>

## Литература
1. Цикоза В.А., Чурина Т.Г. Методы программирования: перестановки, поиск и сортировка / Новосибирск, 2006. -- С. 5-7.

