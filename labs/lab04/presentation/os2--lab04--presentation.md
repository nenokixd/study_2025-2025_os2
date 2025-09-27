---
## Front matter
lang: ru-RU
title: Лабораторная работа №4
subtitle: Работа с программными пакетами
author:
  - Чекмарев Александр Дмитриевич | Группа НПИбд-03-24
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 27 сентября 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: warsaw

## Fonts
mainfont: Liberation Serif
romanfont: Liberation Serif
sansfont: Liberation Sans
monofont: Liberation Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Чекмарев Александр Дмитриевич
  * Группа НПИбд-03-24
  * Российский университет дружбы народов
  * <https://github.com/nenokixd?tab=repositories>

:::
::: {.column width="30%"}


:::
::::::::::::::


# Вводная часть


## Объект и предмет исследования

- Работа с файлами репозиториев и пакетами-rpm

## Цель работы

- Получить навыки работы с репозиториями и менеджерами пакетов.

# Ход лабораторной работы

## Переход в каталог и просмотр содержимого

- Зайдем в режим root. 
- Перейдем в каталог /etc/yum.repos.d и изучим содержание каталога

![](image/Screenshot_2.png){#fig:001 width=80%}


## Просмотр файлов репозитория

- На примере просмотрим файлы rocky-devel.repo и rocky.repo

![](image/Screenshot_3.png){#fig:001 width=50%}  ![](image/Screenshot_3.1.png){#fig:001 width=50%} 


## Список репозиториев

- Выведем на экран список репозиториев

![](image/Screenshot_4.png){#fig:001 width=70%}

## Список пакетов

- Выведем на экран список пакетов, в названии или описании которых есть слово user

![](image/Screenshot_5.png){#fig:001 width=65%}


## Просмотр пакетов nmap

- Установим nmap, предварительно изучив информацию по имеющимся пакетам
- Найдем nmap

![](image/Screenshot_6.png){#fig:001 width=70%}

## Просмотр информации nmap

- Просмотрим подробную информацию о нем

![](image/Screenshot_7.png){#fig:001 width=65%}

## Установка nmap

- Перейдем к установке nmap

![](image/Screenshot_8.png){#fig:001 width=75%}


## Установка nmap-ncat

- Установим другие пакеты с началом nmap

![](image/Screenshot_9.png){#fig:001 width=70%}


## Удаление nmap

- Удалим как nmap, так и nmap-ncat 

![](image/Screenshot_10.png){#fig:001 width=50%} ![](image/Screenshot_11.png){#fig:001 width=50%}



## Группа пакетов RPM Development Tools

- Получим список имеющихся групп пакетов, затем установим группу пакетов RPM Development Tools
- Сначала просмотрим список

![](image/Screenshot_12.png){#fig:001 width=45%} ![](image/Screenshot_13.png){#fig:001 width=45%}


## Просмотр информации о пакете RPM Development Tools

- Узнаем о информацию о группах пакета RPM Development Tools

![](image/Screenshot_14.png){#fig:001 width=70%}


## Установка RPM Development Tools

- Установим RPM Development Tools

![](image/Screenshot_15.png){#fig:001 width=70%}


## Удаление группы пакетов RPM Development Tools

- Для удаления группы пакетов RPM Development Tools можно воспользоваться командой **dnf groupremove "RPM Development Tools"**

![](image/Screenshot_16.png){#fig:001 width=60%}


## Просмотр истории команды dnf

- Посмотрим историю использования команды dnf

![](image/Screenshot_17.png){#fig:001 width=70%}


## Отмена одного из последних действий

- Отменим последнее, например 14 по счёту

![](image/Screenshot_18.png){#fig:001 width=60%}

## Скачивание rpm-пакета lynx

- Предположим, что требуется установить текстовый браузер lynx из rpm-пакета
- Посмотрим информацию о пакете и скачаем пакет lynx

![](image/Screenshot_19.png){#fig:001 width=70%} 

![](image/Screenshot_20.png){#fig:001 width=65%}

## Поиск каталога и переход

- Найдем каталог, в который был помещён пакет после загрузки
- Перейдем в этот каталог

![](image/Screenshot_21.png){#fig:001 width=70%}


## Установка rpm-пакета и просмотр инофрмации

- Установим rpm-пакет lynx
- Определим расположение исполняемого файла
- Используя rpm, определим по имени файла, к какому пакету принадлежит lynx

![](image/Screenshot_22.png){#fig:001 width=75%}


## Просмотр подробной информации о пакете

- Получим дополнительную информацию о содержимом пакета

![](image/Screenshot_23.png){#fig:001 width=70%}


## Просмотр списка всех файлов в пакете

- Получим список всех файлов в пакете

![](image/Screenshot_24.png){#fig:001 width=70%}


## Просмотр файлов с документацией пакета

- Выведем перечень файлов с документацией пакета


![](image/Screenshot_25.png){#fig:001 width=70%}


## Просмотр файлов документации

- Посмотрим файлы документации, применив команду **man lynx**

![](image/Screenshot_26.png){#fig:001 width=70%}


## Просмотр конфигурационных файлов и скриптов

- Выведем на экран перечень и месторасположение конфигурационных файлов пакета
- Выведем на экран расположение и содержание скриптов, выполняемых при установке пакета

![](image/Screenshot_37.png){#fig:001 width=75%}


## Проверка работы текстового браузера lynx

- В отдельном терминале запустим текстовый браузер lynx, чтобы проверить корректность установки пакета.

![](image/Screenshot_39.png){#fig:001 width=70%}


## Удаление lynx

- Вернемся в терминал с учётной записью root и удалим пакет
- Удалим lynx и просмотрим содержимое каталога

![](image/Screenshot_38.png){#fig:001 width=75%}


## Пакет dnsmasq

- Предположим, что требуется из rpm-пакетов установить dnsmasq (DNS-, DHCP- и TFTPсервер).
- Просмотрим информации о пакете и установим dnsmasq

![](image/Screenshot_28.png){#fig:001 width=70%}


## Просмотр расположения исполняемого файла и определение к какому пакету он принадлежит

- Определим расположение исполняемого файла
- Определите по имени файла, к какому пакету принадлежит dnsmasq

![](image/Screenshot_29.png){#fig:001 width=75%}


## Просмотр подробной информации о содержимом пакета

- Получим дополнительную информацию о содержимом пакета dnsmasq

![](image/Screenshot_30.png){#fig:001 width=70%}


## Просмотр списка всех файлов пакета

- Получим список всех файлов в пакете

![](image/Screenshot_31.png){#fig:001 width=70%}


## Просмотр файлов с документацией пакета

- Выведем перечень файлов с документацией пакета

![](image/Screenshot_32.png){#fig:001 width=75%}


## Просмотр файлов документации

- Посмотрим файлы документации, применив команду **man dnsmasq**

![](image/Screenshot_33.png){#fig:001 width=70%}

## Просмотр конфигурационных файлов пакета

- Выведем на экран перечень и месторасположение конфигурационных файлов пакета


![](image/Screenshot_34.png){#fig:001 width=75%}


## Просмотр скриптов пакета

- Выведем на экран расположение и содержание скриптов, выполняемых при установке пакета

![](image/Screenshot_35.png){#fig:001 width=75%}


## Удаление пакета

- Вернемся в терминал с учётной записью root и удалим пакет

![](image/Screenshot_36.png){#fig:001 width=75%}

## Вывод:

В ходе работы приобретены навыки работы с репозиториями и менеджерами пакетов
