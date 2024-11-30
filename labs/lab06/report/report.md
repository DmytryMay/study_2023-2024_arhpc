---
## Front matter
title: "Отчет по лабораторной работе №6"
subtitle: "Арифметические операци в NASM"
author: "Майоров Дмитрий Андреечи"

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

Освоить арифметических инструкций языка ассемблера NASM и написать программы для вычисления арифметических выражений с неизвестной.

# Задание

Написать программы для решения выражений.


# Выполнение лабораторной работы



![Создаем каталог и файл в нем](image/01.png)

![Открываем файл и заполняем его в соотвествии с листингом](image/02.png)

![Создаем исполняемый файл и запускаем его](image/03.png)

![Изменяем файл: убираем кавычки с числовых значений](image/04.png)

![Запускаем файл](image/05.png)

![Создаем новый файл в каталоге](image/06.png)

![Открываем файл и заполняем его в соотвествии с листингом](image/07.png)

![Создаем исполняемый файл и запускаем его](image/08.png)

![Изменяем файл: убираем кавычки с числовых значений](image/09.png)

![Запускаем файл](image/10.png)

![Изменяем файл: меняем iprintLF на iprint](image/11.png)

![Создаем исполняемый файл и запускаем его](image/12.png)

![Создаем файл](image/13.png)

![Открываем файл и заполняем его в соотвествии с листингом](image/14.png)

![Создаем исполняемый файл и запускаем его](image/15.png)

![Открываем файл и редактируем его для вычисления выражения f(x) = (4*6+2)/5 ](image/16.png)

![Создаем исполняемый файл и запускаем его](image/17.png)

![Создаем файл](image/18.png)

![Открываем файл и заполняем его в соотвествии с листингом](image/19.png)

![Создаем исполняемый файл и запускаем его](image/20.png)

# Ответы на вопросы

1 Строка “mov eax,rem” и строка “call sprint” отвечают за вывод на экран сообщения ‘Ваш вариант:’.

2 Эти инструкции используются для чтения строки с вводом данных от пользователя. Начальный адрес строки сохраняется в регистре ecx, а количество символов в строке (максимальное количество символов, которое может быть считано) сохраняется в регистре edx. Затем вызывается процедура sread, которая выполняет чтение строки.

3 Инструкция “call atoi” используется для преобразования строки в целое число. Она принимает адрес строки в регистре eax и возвращает полученное число в регистре eax.

4 Строка “xor edx,edx” обнуляет регистр edx перед выполнением деления. Строка “mov ebx,20” загружает значение 20 в регистр ebx. Строка “div ebx” выполняет деление регистра eax на значение регистра ebx с сохранением частного в регистре eax и остатка в регистре edx.

5 Остаток от деления записывается в регистр edx.

6 Инструкция “inc edx” используется для увеличения значения в регистре edx на 1 В данном случае, она увеличивает остаток от деления на 1 

7 Строка “mov eax,edx” передает значение остатка от деления в регистр eax. Строка “call iprintLF” вызывает процедуру iprintLF для вывода значения на экран вместе с переводом строки.

# Задание для самостоятельной работы

![Создаем новый файл в каталоге](image/21.png)

Открываем его и заполняем,чтобы решалось выражение f(x)=x^3 * 1/3 + 21

![Заполняем файл](image/22.png)

![Запускаем программу и проверяем ее работу для x=1 и x=3](image/23.png)


# Выводы

Мы приобрели навыки создания исполнительных файлов для решения выражений и освоили арифметические инструкции в NASM.

# Список литературы{.unnumbered}

::: {#refs}
:::
