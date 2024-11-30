---
## Front matter
title: "Отчёт по лабораторной работе №7"
subtitle: "Команды безусловного и условного переходов в Nasm. Программирование ветвлений."
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

Изучение команд условного и безусловного переходов. Приобретение навыков написания
программ с использованием переходов. Знакомство с назначением и структурой файла
листинга

# Задание

Освоить условного и безусловного перехода. Ознакомиться с назначением и
структурой файла листинга.


# Выполнение лабораторной работы


![Создаем каталог лабораторной работы №7 и файл в нем](image/01.png)

![Открываем файл и заполняем его в соотвествии с листингом](image/02.png)

![Создаем исполнительный файл и запускаем его](image/03.png)

![Снова открываем файл и редактируем его в сотвествии с листиногм](image/04.png)

![Создаем исполнительный файл и запускаем его](image/05.png)

![Снова открываем файл и редактируем его, чтобы произошел нужный вывод](image/06.png)

![Создаем исполнительный файл и запускаем его. Проверяем, правильный ли вывод](image/07.png)

![Создаем новый файл](image/08.png)

![Открываем файл и заполняем его в соотвествии с листингом](image/09.png)

![Создаем исполнительный файл и запускаем его. Вводим разные значения В](image/10.png)

# Изучение структуры файлы листинга

![Создаем файл листинга для программы lab7-2.asm](image/11.png)

![Открываем файл листинга и изучаем его](image/12.png)

Строка 33: 0000001D-адрес в сегменте кода, BB01000000-машинный код, mov ebx,1-присвоение переменной ecx значения 1

Строка 34: 00000022-адрес в сегменте кода, B804000000-машинный код, mov eax,4-присвоение переменной eax значения 4

Строка 35: 00000027-адрес в сегменте кода, CD80-машинный код, int 80h-вызов ядра.

![ОТкрываем файл и удаляем один операнудм](image/13.png)

![Транслируем файл](image/14.png)

При трансляции файла, выдается ошибка, но создаются файлы lab7-2 и lab7-2.lst

![Открываем файл с ошмбкой и изучаем его](image/15.png)

# Задание для самостоятельной работы (Вариант 20)

Напишите программу нахождения наименьшей из 3 целочисленных переменных a,b и . Значения переменных выбрать из табл. 7.5 в соответствии с вариантом, полученным при выполнении лабораторной работы № 7. Создайте исполняемый файл и проверьте его работу.

![Создаем новый файл](image/16.png)

![Открываем файл и пишем программу](image/17.png)

![Танслируем файл и смотрим на его работу](image/18.png)

Напишите программу, которая для введенных с клавиатуры значений 𝑥 и 𝑎 вычисляет значение заданной функции f(x) и выводит результат вычислений. Вид функции f(x) выбрать из таблицы 7.6 вариантов заданий в соответствии с вариантом, полученным при выполнении лабораторной работы № 7. Создайте исполняемый файл и проверьте его работу для значений x и a из 7.6.

![Создаем новый файл](image/19.png)

![Открываем файл и пишем программу](image/20.png)

![Транслируем файл и проверяем его работу при x=1 и а=2](image/21.png)

![Транслируем файл и проверяем его работу при x=2 и а=1](image/22.png)

# Выводы

Мы познакомились с структурой файла листинга, изучили команды условного и безусловного перехоа.

# Список литературы{.unnumbered}

::: {#refs}
:::
