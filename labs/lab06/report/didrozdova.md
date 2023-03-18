---
## Front matter
title: "Лабораторная работа №6"
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

1. Ознакомление с инструментами поиска файлов и фильтрации текстовых данных.
2. Приобретение практических навыков: 
  - по управлению процессами (и заданиями), 
  - проверке использования диска,
  - по обслуживанию файловых систем.

# Выполнение лабораторной работы

1. Осуществите вход в систему, используя соответствующее имя пользователя.

2. Запишите в файл file.txt названия файлов, содержащихся в каталоге /etc. Допишите в этот же файл названия файлов, содержащихся в вашем домашнем каталоге.

  ![/etc](image/02.1.jpg){#fig:001 width=70%}
  
   ![~/](image/02.jpg){#fig:001 width=70%}

3. Выведите имена всех файлов из file.txt, имеющих расширение .conf, после чего запишите их в новый текстовой файл conf.txt.

 ![conf.txt](image/03.jpg){#fig:001 width=70%}

4. Определите, какие файлы в вашем домашнем каталоге имеют имена, начинавшиеся с символа c? 

 ![c*](image/04.jpg){#fig:001 width=70%}

5. Выведите на экран (по странично) имена файлов из каталога /etc, начинающиеся с символа h.

 ![h*](image/05.jpg){#fig:001 width=70%}

6. Запустите в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log.

 ![logfile](image/06.jpg){#fig:001 width=70%}

7. Удалите файл ~/logfile.

8. Запустите из консоли в фоновом режиме редактор gedit.

 ![gedit&](image/08.jpg){#fig:001 width=70%}

9. Определите идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep. Как ещё можно определить идентификатор процесса?

 ![ps aux](image/09.jpg){#fig:001 width=70%}
 
  ![pgrep](image/09.1.jpg){#fig:001 width=70%}

10. Прочтите справку (man) команды kill, после чего используйте её для завершения процесса gedit.

 ![kill <>](image/10.jpg){#fig:001 width=70%}

11. Выполните команды df и du, предварительно получив более подробную информацию об этих командах, с помощью команды man.

  - *df ~/*

 ![df](image/11.jpg){#fig:001 width=70%}
 
 - *du ~/work*
 
  ![du](image/11.1.jpg){#fig:001 width=70%}
  
  ![du](image/11.2.jpg){#fig:001 width=70%}

12. Воспользовавшись справкой команды find, выведите имена всех директорий, имеющихся в вашем домашнем каталоге.

  ![man find](image/12.1.jpg){#fig:001 width=70%}
  
  ![каталоги ~/](image/12.jpg){#fig:001 width=70%}
  
# Выводы
В ходе выполнения данной лабораторной работы мы ознакомились с инструментами поиска файлов и фильтрации текстовых данных и приобрели практические навыки по управлению процессами (и заданиями), по
проверке использования диска и обслуживанию файловых систем.

