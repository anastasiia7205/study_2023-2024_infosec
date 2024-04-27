---
## Front matter
lang: ru-RU
title: Лабораторная работа №6
subtitle: Основы информационной безопастности
author:
  - Астраханцева А. А.
institute:
  - Российский университет дружбы народов, Москва, Россия

date: 27 апреля 2024

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Астраханцева Анастасия Александровна
  * студентка НКАбд-01-22
  * Студ. билет: 1132226437
  * Российский университет дружбы народов
  * <https://anastasiia7205.github.io/>

:::
::: {.column width="50%"}

![](./image/nastya.jpg)

:::
::::::::::::::

## Цель работы

Развить навыки администрирования ОС Linux. Получить первое практическое знакомство с технологией SELinux1.
Проверить работу SELinx на практике совместно с веб-сервером Apache.

# Выполнение лабораторной работы

## Проверка работы SELinux

![Проверка работы SELinux](image/1.jpg){#fig:001 width=70%}

## Проверка работы веб-сервера
	
![Проверка работы веб-сервера](image/3.jpg){#fig:002 width=70%}

## Контекст безопасности веб-сервера Apache

![Контекст безопасности веб-сервера Apache](image/4.jpg){#fig:003 width=70%}

## Текущее состояние переключателей SELinux для Apache

![Текущее состояние переключателей SELinux для Apache](image/5.jpg){#fig:004 width=70%}

## Статистика по политике

![Статистика по политике](image/6.jpg){#fig:005 width=70%}

## Типы файлов в дирректриях /var/www и /var/www/html

![Типы файлов в дирректриях /var/www и /var/www/html](image/7.jpg){#fig:006 width=70%}

## Создание html-файла

![Создание html-файла](image/8.jpg){#fig:007 width=70%}

## Контекст файла /var/www/html

![Контекст файла /var/www/html](image/9.jpg){#fig:008 width=70%}

## Файл /var/www/html

![Файл /var/www/html](image/10.jpg){#fig:009 width=70%}

## Изменение контекста файла /var/www/html/test.html

![Изменение контекста файла /var/www/html/test.html](image/11.jpg){#fig:010 width=70%}

## Сообщение об ошибке

![Сообщение об ошибке](image/12.jpg){#fig:011 width=70%}

## Просмотр log-файлов

![Просмотр log-файлов](image/13.jpg){#fig:012 width=70%}

## Просмотр log-файлов

![Просмотр log-файлов](image/14.jpg){#fig:013 width=70%}

## Просмотр файлов /var/log/messages, /var/log/http/error_log

![Просмотр файлов /var/log/messages, /var/log/http/error_log](image/15.jpg){#fig:014 width=70%}

## Добавление порта 81

![Добавление порта 81](image/16.jpg){#fig:015 width=70%}

## Зпапуск веб-сервера Apache

![Зпапуск веб-сервера Apache](image/17.jpg){#fig:016 width=70%}

## Исправление конфигурационного файла apache

![Исправление конфигурационного файла apache](image/18.jpg){#fig:017 width=70%}

## Удаление привзяки к порту 81 и файла /var/www/html/test.html:

![Удаление привзяки к порту 81 и файла /var/www/html/test.html:](image/19.jpg){#fig:018 width=70%}


## Выводы

В ходе выполения ЛР№6 я развила навыки администрирования ОС Linux. Получила первое практическое знакомство с технологией SELinux1. Прверила работу SELinx на практике совместно с веб-сервером Apache.

# Спасибо за внимание

