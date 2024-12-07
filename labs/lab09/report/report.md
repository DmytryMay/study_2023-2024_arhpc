---
## Front matter
title: "Отчёт по лабораторной работе №9"
subtitle: "Понятие подпрограммы.Отладчик GBD"
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

Приобретение навыков написания программ с использованием подпрограмм. Знакомство с методами отладки при помощи GDB и его основными возможностями.



# Выполнение лабораторной работы

![Создаем каталог для програм лабораторной работы и файл в нем](image/01.png)

![Открываем файл и заполняем его в соотвествии с листингом](image/02.png)

![Создаем исполняемый файл и запускаем его](image/03.png)

![Изменяем файл. Добавляем подпрограмму](image/04.png)

![Создаем исполняемый файл и запускаем его](image/05.png)

![Создаем новый файл](image/06.png)

![Открываем файл и заполняем его в соотвествии с листингом](image/07.png)

![Загружаем исходный файл в отладчик](image/08.png)

![Запускаем программу командой run](image/09.png)

![Запускаем программу с брейкпоином](image/10.png)

![Смотрим дисассимилированный код программы](image/11.png)

![Переключаемся на синтаксис intel](image/12.png)

Различия отображения синтаксиса машинных команд в режимах ATT и Intel:
1.Порядок операндов: В ATT синтаксисе порядок операндов обратный, сначала указывается исходный операнд, а затем - результирующий операнд. В Intel син- таксисе порядок обычно прямой, результирующий операнд указывается первым, а исходный - вторым.
2.Разделители: В ATT синтаксисе разделители операндов - запятые. В Intel синтаксисе разделители могут быть запятые или косые черты (/).
3.Префиксы размера операндов: В ATT синтаксисе размер операнда указывается перед операндом с использованием префиксов, таких как “b” (byte), “w” (word), “l” (long) и “q” (quadword). В Intel синтаксисе размер операнда указывается после операнда с использованием суффиксов, таких как “b”, “w”, “d” и “q”.
4.Знак операндов: В ATT синтаксисе операнды с позитивными значениями предваряются символом “". "”.
5.Обозначение адресов: В ATT синтаксисе адреса указываются в круглых скобках. В Intel синтаксисе адреса указываются без скобок.
6.Обозначение регистров: В ATT синтаксисе обозначение регистра начинается с символа “%”. В Intel синтаксисе обозначение регистра может начинаться с символа “R” или “E” (например, “%eax” или “RAX”).

![Включаем отображение регистров, их значений и результат дисассимилирования программы](image/13.png)

![Создаем новую точку останова](image/14.png)

![Смотрим информацию](image/15.png)

![Отслеживаем регистры командой si](image/16.png)

Во время выполнения команд менялись регистры: ebx, ecx, edx,eax, eip.

![Смотрим значение переменной msg1 по имени](image/17.png)

![Смотрим значение переменной msg2 по адресу](image/18.png)

![Изменим перввй символ переменной msg1](image/19.png)

![Изменим перввй символ переменной msg2](image/20.png)

![Смотрим значение регистра edx в разных форматах](image/21.png)

![Изменяем регистр ebx](image/22.png)

Выводится разные значения, так как команда без кеавычек присваивает регистру вводимое значение.

![Прописываем команды для завершения программы и выхода из GDB](image/23.png)

![Копируем файл lab8-2.asm в файл с именем lab09-3.asm](image/24.png)

![Создаем исполняемый файл и запускаем его в отладчике GDB](image/25.png)

![Устанавливаем точку останова](image/26.png)

![Изучаем полученные данные](image/27.png)

Шаг изменения адреса равен 4 потому что адресные регистры имеют размерность 32 бита(4 байта).

# Задание для самостоятельной работы

Задание 1

![Копируем файл lab8-4.asm в файл с именем lab09-4.asm](image/28.png)

![Изменяем файл. СОздаем подпрограмму](image/29.png)

![Создаем исполняемый файл и запускаем его](image/30.png)

Задание 2

![Создаем файл](image/31.png)

![ОТкрываем файл и заполняем его в соответсвии с листингом](image/32.png)

![Создаем исполняемый файл и запускаем его. Программа работает неправильно](image/33.png)

![Ищем ошибку регистров в отладчике](image/34.png)

![Изменяем файл](image/35.png)

![Создаем исполняемый файл и запускаем его. Программа работает правильно](image/36.png)

# Выводы

Мы познакомились с методами отладки при помощиGDBи его возможностями.

# Список литературы{.unnumbered}

::: {#refs}
:::
