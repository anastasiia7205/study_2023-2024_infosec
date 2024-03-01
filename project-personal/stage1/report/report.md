---
## Front matter
title: "Индивидуальный проект. Этап №1"
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание

Установка операционной системы Linux, дистрибутив Kali.

# Выполнение лабораторной работы

Начимаем создание новой виртуальной машины, указываем тип и имя ОС. В моем случае имя ОС такое же как логин для работы в ДК. (рис. [-@fig:001]).

![Тип и имя ОС](image/1.jpg){#fig:001 width=70%}

Указываем объем памяти. Указываем 2048 МБ. (рис. [-@fig:002]).

![Объем памяти](image/2.jpg){#fig:002 width=70%}

Создаем новый виртуальный жесткий диск (рис. [-@fig:003]).

![Жесткий диск](image/3.jpg){#fig:003 width=70%}

Указываем тип виртуального жесткого диска (рис. [-@fig:004]).

![Тип жесткого диска](image/4.jpg){#fig:004 width=70%}

Указываем формат хранения (рис. [-@fig:005]).

![Формат хранения](image/5.jpg){#fig:005 width=70%}

Указываем имя и размер нового виртуального жесткого диска. Выбираем 40 ГБ (рис. [-@fig:006]).

![Имя и размер жесткого диска](image/6.jpg){#fig:006 width=70%}

Далее необходимо было в настройках в разделе "Ностители" выбрать контроллер IDE. Для этого нужно было предварительно установить Kali с разрещением .iso. (рис. [-@fig:007]).

![Установка контроллера IDE](image/7.jpg){#fig:007 width=70%}

Заупскаем виртуальную машину. Выбираем "Graphical install" (рис. [-@fig:008]).

![Зпауск виртуальной машины](image/9.jpg){#fig:008 width=70%}

Выбираем русский язык для процесса установки (рис. [-@fig:009]).

![Выбор языка процесса установк](image/10.jpg){#fig:009 width=70%}

Выбираем страну (рис. [-@fig:010]).

![Выбор страны](image/11.jpg){#fig:010 width=70%}

Выбираем раскладку клавиатуры (рис. [-@fig:011]).

![Расклавдка клваиатуры](image/11.jpg){#fig:011 width=70%}

Вводим имя компьютера и имя домена (рис. [-@fig:012] - [-@fig:013]).

![Имя компьютера](image/12.jpg){#fig:012 width=70%}

![Имя домена](image/13.jpg){#fig:013 width=70%}


Настройка пользователей системы (рис. [-@fig:014] -  [-@fig:016]).

![Имя суперпользователя](image/14.jpg){#fig:014 width=70%}

![Имя пользователя](image/15.jpg){#fig:015 width=70%}

![Пароль для обычного пользователя](image/16.jpg){#fig:016 width=70%}

Выбираем часовой пояс (рис.[-@fig:017]).

![Выбор часового поса](image/17.jpg){#fig:017 width=70%}

Далее необходимо настроить разметку дисков. Оставляем все значения без изменений. (рис. [-@fig:018] - [-@fig:022]).

![Выбор метода разметки](image/18.jpg){#fig:018 width=70%}

![Выбор диска для разметки](image/19.jpg){#fig:019 width=70%}

![Выбор схемы разметки](image/20.jpg){#fig:020 width=70%}

![Список настроенны разделов и их точки монтирования](image/21.jpg){#fig:021 width=70%}

![Окончание разметки диска](image/22.jpg){#fig:022 width=70%}


Далее идет выбор дополнительных пакетов, необходимых для установки. Выбранные пункты позволят установить страндартную версию Кали (рис.[-@fig:023]).

![Устоанвка стандартных инструментов Кали](image/23.jpg){#fig:023 width=70%}

Установка системного загрузчика. Устнавлваем его на первичный диск(рис. [-@fig:024]).

![Установка системного загрузчика](image/24.jpg){#fig:024 width=70%}

Выбор устройства для установки системного загрузчика. (рис.[-@fig:025]).

![Устройство для установки системного загрузчика](image/25.jpg){#fig:025 width=70%}


Перезагрузка машины и заверщение устновки (рис. [-@fig:026]).

![Перезагрузка машины и заверщение устновки ](image/26.jpg){#fig:026 width=70%}

Загрузка заверена. Можем запускать Кали (рис. [-@fig:027]).

![Главный экра Кали](image/27.jpg){#fig:027 width=70%}



# Выводы

В ходе выполнения лабораторной раьоты я приобрела практические навыки установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

