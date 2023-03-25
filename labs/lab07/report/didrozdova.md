---
## Front matter
title: "Лабораторная работа №7"
subtitle: "Операционные системы"
author: "Дарья Игоревна Дроздова"

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
lot: false # List of tables
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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

- Освоение основных возможностей командной оболочки Midnight Commander;
- Приобретение навыков практической работы по просмотру каталогов и файлов и по манипуляциям с ними.

# Выполнение лабораторной работы

1. **Задание по mc**
  - Изучите информацию о mc, вызвав в командной строке man mc. Запустите из командной строки mc, изучите его структуру и меню:
  
![mc](image/111.jpg){#fig:001 width=70%}
   
![F1](image/23.jpg){#fig:001 width=70%}
  
  - Выполните несколько операций в mc, используя управляющие клавиши  
*операции с панелями:*  

![F9](image/22.jpg){#fig:001 width=70%}

*копирование/перемещение файлов*

![mv](image/21.jpg){#fig:001 width=70%}

![cp](image/20.jpg){#fig:001 width=70%}

![результат cp, mv](image/18.jpg){#fig:001 width=70%}

*получение информации о размере и правах доступа на файлы и/или каталоги*

![info](image/17.jpg){#fig:001 width=70%}
  
  - Выполните основные команды меню левой (или правой) панели. Оцените степень подробности вывода информации о файлах.
  
![info](image/16.jpg){#fig:001 width=70%}  
  
  - Используя возможности подменю Файл , выполните:
*просмотр содержимого текстового файла:*

![просмотр файла](image/15.jpg){#fig:001 width=70%}

*редактирование содержимого текстового файла (без сохранения результатов
редактирования)*
*создание каталога*
*копирование в файлов в созданный каталог*

![cp](image/14.jpg){#fig:001 width=70%}

  -  С помощью соответствующих средств подменю Команда осуществите:
  
  *поиск в файловой системе файла с заданными условиями: с расширением .pdf содержащего строку pandoc*

![*.pdf](image/13.jpg){#fig:001 width=70%}

![*.pdf](image/12.jpg){#fig:001 width=70%}

![pandoc](image/11.jpg){#fig:001 width=70%}

  - Вызовите подменю Настройки . Освойте операции, определяющие структуру экрана mc (Full screen, Double Width, Show Hidden Files и т.д.)
  
![экран mc](image/10.jpg){#fig:001 width=70%}  
  
2. **Задание по встроенному редактору mc**

  - Создайте текстовой файл text.txt.
  
![text.txt](image/09.jpg){#fig:001 width=70%}

  - Откройте этот файл с помощью встроенного в mc редактора. Вставьте в открытый файл небольшой фрагмент текста, скопированный из любого другого файла или Интернета.

![text.txt](image/07.jpg){#fig:001 width=70%}

  - Проделайте с текстом следующие манипуляции, используя горячие клавиши:
*Удалите строку текста* 

![Ctrl-y](image/08.jpg){#fig:001 width=70%}

*Выделите фрагмент текста и скопируйте его на новую строку*

![F3](image/06.jpg){#fig:001 width=70%}

![F5](image/05.jpg){#fig:001 width=70%}

*Выделите фрагмент текста и перенесите его на новую строку. Отмените последнее действие*

![F6](image/04.jpg){#fig:001 width=70%}

*Сохраните и закройте файл*

![F2, F10](image/03.jpg){#fig:001 width=70%}

  - Откройте файл с исходным текстом на некотором языке программирования( в моем случае на языке С++)
  
![.cpp](image/02.jpg){#fig:001 width=70%}
  
  - Используя меню редактора, включите подсветку синтаксиса, если она не включена, или выключите, если она включена
  
![подсветка синтаксиса](image/01.jpg){#fig:001 width=70%}
  
  
# Выводы
В ходе выполнения данной лабораторной работы мы ознакомились с основными возможностями командной оболочки Midnight Commander и  приобрели практические навыки по просмотру каталогов и файлов и по манипуляциям с ними.
