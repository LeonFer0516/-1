---
# Front matter
lang: ru-RU
title: "Шаблон отчёта по лабораторной работе 2"
subtitle: "дисциплина: Операционные системы"
author: "Студент: Леон Атупанья Хосе Фернандо"

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

# Цель работы

Изучить идеологию и применение средств контроля версий.

# Задание

Сделайте отчёт по предыдущей лабораторной работе в формате Markdown.–В качестве отчёта просьба предоставить отчёты в 3 форматах:pdf,docxиmd(вархиве,поскольку он должен содержать скриншоты,Makefile ит.д.)


# Выполнение лабораторной работы

Создайте учётную запись на https://github.com. (рис. -@fig:001)

![imagen 1](imagenes/1.png){ #fig:001 width=70% }

Настроим систему контроля версий git. Поэтому во первых мы должны установить git на системе. Создаем наш репозиторий на Github.com (рис. -@fig:002)

![imagen 2](imagenes/2.png){ #fig:002 width=70% }

Прежде создать наш локальный репозиторий, мы делаем предварительную конфигурацию, указав имя и email владельца репоитория, а на консоль пишем команд git congif –global user.name “leonjose” и git config –global user.email “fernandoleon833@gmail.com”   (рис. -@fig:003)

![imagen 3](imagenes/3.png){ #fig:003 width=70% }

После этого мы пишем код чтобы получить Key для последующей идентификации пользователя на сервере репозиториев, потом пишем код cat /home/Fernando/.ssh/id_rsa.pub чтобы показать key. (рис. -@fig:004)

![imagen 4](imagenes/4.png){ #fig:004 width=70% }

Опять зайдем на Github.com и мы ввели код, который мы получили в разделе SSH and GPG Keys. Мы назначаем имя и код. (рис. -@fig:005)

![imagen 5](imagenes/5.png){ #fig:005 width=70% }

Создаем каталоги по имени program/2020-2021/OS/laboratory и используем коды echo “# lab-2” >> README.md, git init, git add, git add README.md. (рис. -@fig:006)

![imagen 6](imagenes/6.png){ #fig:006 width=70% }

После этого выкладываем на Gibhub. (рис. -@fig:007)

![imagen 7](imagenes/7.png){ #fig:007 width=70% }

Добавим файл лицензии, шаблон игнорируемых файлов, новые файлы и выполним коммит и отправим на github. (рис. -@fig:008) (рис. -@fig:009)

![imagen 8](imagenes/8.png){ #fig:008 width=70% }
![imagen 9](imagenes/9.png){ #fig:009 width=70% }

А теперь начинаем с конфигурацией git flow и инициализируем, проверяем если мы на ветке develop, запишем версию, добавим индекс, зальём реализую ветку в основную ветку и отправим данные на git.hub. (рис. -@fig:0010) (рис. -@fig:0011)

![imagen 10](imagenes/10.png){ #fig:0010 width=70% }
![imagen 11](imagenes/11.png){ #fig:0011 width=70% }


# Выводы

В ходе данной работы я научился о системе контроль версий и как можем работать с сервером Github.com, из того же образом я узнал, как создать локальный репозиторий и как связать его с сервером.
