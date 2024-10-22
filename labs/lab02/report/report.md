---
## Front matter
title: "Отчет по лабораторной работе №2"
subtitle: "Система контроля версий git"
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

Изучить идеологию и применение средств контроля версий. Приобрести
практические навыки по работе с системой git.



# Выполнение лабораторной работы

Настройка GitHub

![Создаем аккаунт на сайте GitHub и вводим основные данные.](image/01.jpg)

Базовая настройка git

![Открываем терминал и вводим команды, указывая имя и email.](image/02.jpg)

![Настраиваем utf-8 в выводе сообщений git. Зададим имя начальной ветки. Параметр autocrlf, параметр safecrlf.](image/03.jpg)

Создание SHH ключа

![Для последующей идентификации пользователя на сервере репозиториев необходимо сгенерировать пару ключей. Ключи сохраняться в каталоге ~/.ssh/.](image/04.jpg)

![Копируем ключ из локальной консоли в буфер обмена](image/05.jpg)

![Далее необходимо загрузить сгенерённый открытый ключ. Для этого зайти на сайт http: //github.org/ под своей учётной записью и перейти в меню Setting. После этого выбрать в боковом меню SSH and GPG keys и нажать кнопку New SSH key. Вставляем ключ в появившееся на сайте поле и указываем для ключа имя (Title).](image/06.jpg)

Сздание рабочего пространства и репозитория курса на основе шаблона

![Открываем терминал и создаем каталог для предмета «Архитектура компьютера».](image/07.jpg)

Создание репозитория курста на основе шаблона

![Переходим на станицу репозитория с шаблоном курса https://github.com/yamadharma/cour se-directory-student-template. Далее выбераем Use this template](image/08.jpg)

![В открывшемся окне задаем имя репозитория (Repository name) study_2023–2024_arhpc и создаем репозиторий (кнопка Create repository from template)](image/09.jpg)

![Открываем терминал и переходим в каталог курса. Клонируем созданный репозиторий. (Ссылку для клонирования копируем на странице созданного репозитория Code -> SSH)](image/10.jpg)

Настройка каталога курса

![Переходим в каталог курса, удаляем лишние файлы.](image/11.jpg)

![Создаем каталоги](image/12.jpg)

![Отправляем файлы на сервер](image/13.jpg)

![Проверяем правильность создания иерархии рабочего пространства в локальном репозитории и на странице github.](image/14.jpg)

Выполнение самостоятельной работы

![Скопируем отчет по первой лабараторной работе в локальный репозиторий. Проверим его наличие.](image/15.jpg)

![Отправим изменения на github](image/16.jpg)

![Проверяем, появился ли отчет.](image/17.jpg)

Все действия проводим со второй лабаротной работой.




# Выводы

Я изучил идеологию и применение средств контроля версий. Приобрел практические навыки по работе с системой git

# Список литературы{.unnumbered}

::: {#refs}
:::
