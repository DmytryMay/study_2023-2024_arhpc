---
## Front matter
title: "Отчет по лабораторной работе №4"
subtitle: "Создание и процесс обработки программ на языке ассемблера NASM"
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

Освоение процедуры компиляции и сборки программ, написанных на ассемблере NASM.

# Задание

Написать 2 программы ("Hello world!", "Имя Фамилия")



# Выполнение лабораторной работы

##3.1 Программа Hello world!

![Создаем каталог для работы с программами на языке ассемблера NASM](image/14.png)

![Переходим в созданный каталог](image/01.png)

![Создаем текстовый файл с именем hello.asm и открываем его](image/02.png)

![Вводим нужный текст](image/03.png)

##Транслятор NASM

![Используем команду nasm и проверяем, создался ли обьектный файл](image/04.png)

##Расширенный синтаксис командной строки NASM

![Компилируем исходный файл и проверяем как сработала команда](image/05.png)

##Компоновщик LD

![Передаем обьектный файл на обработку компоновщику и проверяем, создался ли файл hello](image/06.png)

![Передаем обьектный файл на обработку компоновщику и проверяем, создался ли файл main](image/07.png)

##Запуск исполняемого файла

![Запускаем исполняемый файл](image/08.png)

##Задание для самостоятельной работы

![Создаем копию файла hello.asm и открываем его](image/09.png)

![Редактируем файл](image/10.png)

![Прописываем те же команды что и в первой программе](image/11.png)

![Копируем файлы в локальный репозиторий](image/12.png)

![Переходим в каталог лабораторных работ и отправляем на GitHub](image/13.png)

# Выводы

Я освоил процедуры компиляции и сборки программ, написал 2 программы.

# Список литературы{.unnumbered}

::: {#refs}
:::
