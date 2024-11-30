---
## Front matter
title: "Отчет по лаюораторной работе №5"
subtitle: "Основы работы с Midnight Commander"
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

Приобретение практических навыков работы в Midnight Commander. Освоение инструкций
языка ассемблера mov и int.

# Задание

Написать 2 программы по примеру и впоследствии изменить их по условию.


# Выполнение лабораторной работы

![Открываем Midnight Commander](image/01.png)

![Переходим в каталог, созданный при выполнении 4 ЛБ](image/02.png)

![Создаем каталог lab05](image/03.png)

![Создаем файл lab5-1.asm](image/04.png)

![Открываем файл, заполняем по листингу и сохраняем](image/05.png)

![Открываем файл и убеждаемся что текст сохранился](image/06.png)

![Транслируем текст программы и запускаем исполняемый файл. Проверяем, как работает данная программа.](image/07.png)

![Скачиваем нужный файл](image/08.png)

![Копируем файл в нужную директорию](image/09.png)

![Создаем копию файлф lab5-1.asm](image/10.png)

![Проверяем, скопировался ли файл](image/11.png)

![Открываем новый файл и зполянем его](image/12.png)

![Транслируем и запускаем новый файл](image/13.png)

![Снова открываем файл и меняем SprintLF на sprint](image/14.png)

![Транслируем и запускаем файл](image/15.png)

Можем сделать вывод, что команда sprint выводит текст в той же строке, а sprintLF переносит на новую строку

Задание для самостоятельной работы

![Создаем копию файла lab5-1.asm](image/16.png)

![Открываем и редактируем файл](image/16.png)

![Транслируем файл и запускаем программу](image/18.png)

![Создаем копию файла lab5-2.asm](image/19.png)

![РЕдактируем файл](image/20.png)

![Транслируем файл и запускаем программу](image/21.png)


# Выводы

Мы приобрели навыки работы с Midnight Commander

# Список литературы{.unnumbered}

::: {#refs}
:::
