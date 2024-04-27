---
## Front matter
title: "Индивидуальный проект. Этап №4"
subtitle: "Основы инфомационной безопасности"
author: "Астраханцева А. А."

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

Знакомство со сканером безопастности Nikto и применение.

# Теоретическое введение

Nikto – бесплатный (open source) сканер для поиска уязвимостей в веб-серверах. Утилита относиться к классу blackbox сканеров, т. е. сканеров, использующих стратегию сканирования методом черного ящика. Это значит, что заранее неизвестно о внутреннем устройстве программы/сайта (доступ к исходному коду отсутствует) и упор сделан на функциональность. Программа может обнаруживать более 6700 потенциально опасных файлов и уязвимостей. Новые уязвимости добавляются в базу данных программы по мере их возникновения. Помимо поиска уязвимостей, сканер производит поиск на наличие устаревших версий, используемых библиотек и фреймворков. Nikto не позиционируется как стелс сканер (стелс сканеры никогда не устанавливают TCP-соединения до конца, тем самым сканирование происходит скрытно) – при сканировании сайта в логах сайта или в любой другой системе обнаружения вторжений, если она используется, будет отображена информация о том, что сайт подвергается сканированию.

Среди функций Nikto можно выделить следующие:

    поддержка SSL,

    поддержка HTTP прокси;

    создание отчетов в текстовом формате, XML, HTML, NBE или CSV;

    возможность сканирования портов;

    поиск поддоменов;

    поддержка плагинов для расширения функционала сканирования [1].

# Выполнение

Прверяем, утсновлен ли Nikto, запрашивая его версию: `nikto -Version`. После этого для ознакомления читаем справку по команде nikto: `nikto -Help`(рис. [-@fig:001]).

![Провесрка версии и просмотр справки](image/1.jpg){#fig:001 width=70%}

Попробуем запустить сканер на сайте rudn.ru (рис. [-@fig:002]).

![Проверка работы сканера на сайте rudn.ru](image/2.jpg){#fig:002 width=70%}


# Выводы

Познакомилась со сканером безопастности Nikto и примениа его для сканирования сайта.

# Список литературы. Библиография

[1] Обзор сканера Nikto для поиска уязвимостей в веб-серверах: https://habr.com/ru/companies/first/articles/731696/

[2] Проверяем на уязвимости любой сайт с помощью Nikto: https://habr.com/ru/companies/otus/articles/492546/
