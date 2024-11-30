---
## Front matter
title: "Отчёт по лабораторной работе №8"
subtitle: "Программирование цикла. Обработка аргументов командной строки."
author: "Майоров Дмитрий Андреевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Приобретение навыков написания программ с использованием циклов и обработкой аргументов командной строки

# Задание

Написать программы с использованием циклов и обработкой аргументов командной строки.


# Выполнение лабораторной работы

![Создаем каталог для лабораторной работы №8 и файл в нем](image/01.png)

![Открываем файл и заполянем его в соответсвии с листингом](image/02.png)

![Создаем исполняемый файл и запускаем его](image/03.png)

![Открываем файл и изменяем его. Добавляем изменение значения регистра в цикле](image/04.png)

![Создаем исполняемый файл и запускаем его](image/05.png)

Регистр ecx принимает значения 9,7,5,3,1(на вход подается число 10, в цикле label данный регистр уменьшается на 2 командой sub и loop).
Число проходов цикла не соответсвует числу N, так как уменьшается на 2
Снова открываем файл для редактирования и изменяем его, чтобы все корректно работало.

![Редактируем файл](image/06.png)

![Создаем исполняемый файл и запускаем его](image/07.png)

В данном случае число проходов цикла равна числу N.

![Создаем новый файл](image/08.png)

![Открываем файл и заполянем его в соответсвии с листингом](image/09.png)

![Создаем исполняемый файл и запускаем его](image/10.png)

Програмой было обработано 3 аргумента.

![Создаем новый файл](image/11.png)

![Открываем файл и заполянем его в соответсвии с листингом](image/12.png)

![Создаем исполняемый файл и запускаем его](image/13.png)

![Редактируем файл, чтобы вычислялось произведение вводимых значений](image/14.png)

![Создаем исполняемый файл и запускаем его](image/15.png)

# Задание для самостоятельной работы

Вариант 20

Напишите программу, которая находит сумму значений функции f(x) для x = x1, x2, ..., xn, т.е. программа должна выводить значение f(x1) + f(x2) + ... + f(xn). Значения xi передаются как аргументы. Вид функции f(x) выбрать из таблицы 8.1 вариантов заданий в соответствии с вариантом, полученным при выполнении лабораторной работы № 7. Создайте исполняемый файл и проверьте его работу на нескольких наборах x = x1, x2, ..., xn.

![Создаем новый файл](image/16.png)

![Пишем программу](image/17.png)

![Создаем исполняемый файл и запускаем его. Смотрим на работу программы при х1=5, х2=3, х1=4(все праивльно)](image/18.png)

![Создаем исполняемый файл и запускаем его. Смотрим на работу программы при х1=1, х2=3, х1=7(все праивльно)](image/18.png)

# Выводы

Мы научились решать программы с использованием циклов и обработкой
аргументов командной строки.

# Список литературы{.unnumbered}

::: {#refs}
:::
