---
# Front matter
lang: ru-RU
title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №4"
subtitle: "Системы линейных уравнений"
author: "Аминов Зулфикор Мирзокаримович"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---



# 4.4.1 Метод Гаусса

Построим расширенную матрицу

![рисунка 1](img/1.png){ #fig:001 width=70% }

Можно просматривать поэлементно:

![рисунка 2](img/2.png){ #fig:001 width=70% }

Вывод 1ого строка:

![рисунка 3](img/3.png){ #fig:001 width=70% }

Явной реализации метод Гаусса

![рисунка 4](img/4.png){ #fig:001 width=70% }

Добавим к третьей строке вторую строку, умноженную на -1.5:

![рисунка 5](img/5.png){ #fig:001 width=70% }

Octave располагает встроенной командой для непосредсвенного поиска реугольной формы матрицы:

![рисунка 6](img/6.png){ #fig:001 width=70% }

Включим формат long

![рисунка 7](img/7.png){ #fig:001 width=70% }

Вернем предыдущий формат представления:

![рисунка 8](img/8.png){ #fig:001 width=70% }

# 4.4.2 Левое деление

Выделим из расширенной матрицы B матрицу A:

![рисунка 9](img/9.png){ #fig:001 width=70% }

и вектор b

![рисунка 10](img/10.png){ #fig:001 width=70% }

После найдем вектор x:

![рисунка 11](img/11.png){ #fig:001 width=70% }

# 4.4.4 LU-разложение

LUP-разложение вычисляется в Octave с помощью команды:

![рисунка 12](img/12.png){ #fig:001 width=70% }

# Вывод:

    Научился вычислить СЛУ методом Гауссом в octave