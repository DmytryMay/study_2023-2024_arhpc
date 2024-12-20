---
## Front matter
title: "Отчет по лаборатной работе №3"
subtitle: "Язык разметки Marckdown"
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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Задание

Сформировать отчет по лабораторной работе №2 с помощью Markdown.


# Выполнение лабораторной работы



![Переходим в каталог, привязанный к репозиторию Git и обновляем локальный репозиторий с помощью команды git pull. Далее переходим в каталог с шаблоном отчета по лабораторной работе № 3.](image/01.jpg)

![Проводим компиляцию шаблона с использованием Makefile. Открываем и проверяем корректность полученных файлов.](image/02.jpg)

![Удаляем полученные файлы. Проверяем корректность выполнения команды](image/03.jpg)

![Открываем файл report.md](image/04.jpg)

![Заполняем отчет](image/05.jpg)

![С помощью git отправлем файлы на github](image/06.jpg)


# Выполнение самостоятельной работы

Делаем отчет по лабораторной работе №2 в Marckown

![Заполняем отчет](image/07.jpg)

![Переходим в каталог arch-pc, используем команду make. Далле используем git add и git commit](image/08.jpg)

![Используем git push, отправляем файлы на сервер](image/09.jpg)

# Выводы

Я освоил процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Список литературы{.unnumbered}

::: {#refs}
:::
