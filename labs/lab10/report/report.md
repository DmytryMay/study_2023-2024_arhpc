---
## Front matter
title: "Отчёт по лабораторной работе №10"
subtitle: "Работа с файлами средствами Nasm"
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

Приобретение навыков написания программ для работы с файлами.


# Выполнение лабораторной работы

![Создаем каталог для лабораторной работы №10 и файл в нем](image/01.png)

![Открываем файл и заполняем его в соответсвии с листингом](image/02.png)

![Создаем исполняемый файл и запускаем его](image/03.png)

![Изменяем права доступа кфайлу, запретив его выпонение. Запускаем файл.](image/04.png)

Отказано в доступе. Значит мы поставили правильный запрет на выполнение.

![Изменяем права доступа к файлу с исходным текстом программы, добавив права на исполнение. Запускаем файл](image/05.png)

lab10-1.asm является файлом с исходным кодом программы на языке ассемблера,искусственнодобавление права на исполнение недаст ожидаемого результата. Такие файлы нужно компилировать или ассемблировать в машинный код,а затем выполнять.

Вариант 20

![Предоставляем права доступа к двум файлам в символьном двоичном коде. Проверяем работу команд](image/06.png)

# Задание для самостоятельной работы

![Создаем новый файл](image/07.png)

![Пишем программу](image/08.png)

![Создаем исполняевый файл и запускаем его, после этого проверяем создался ли новый файл, затем смотрим, как он заполнен](image/09.png)



# Выводы

Мы научились писать программы для работы с файлам и научились предоставлять права доступа к файлам.

# Список литературы{.unnumbered}

::: {#refs}
:::
