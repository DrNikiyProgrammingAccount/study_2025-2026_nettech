---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 5
author:
  - Андрюшин Н. С. 
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 01 января 1970

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
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="60%"}

  * Андрюшин Никита Сергеевич
  * Студент
  * Российский университет дружбы народов

:::
::: {.column width="30%"}


:::
::::::::::::::


## Цель работы

Построение простейших моделей сети на базе коммутатора и маршрутизаторов FRR и VyOS в GNS3, анализ трафика посредством Wireshark

## Создание проекта

![Создание проекта](image/1.png){width=70%}

## Схема сети

![Схема сети](image/2.png){width=70%}

## Настройка первого терминала

![Настройка первого терминала](image/3.png){width=70%}

## Настройка второго терминала и пинг

![Настройка второго терминала и пинг](image/4.png){width=70%}

## Остановка всех устройств сети

![Остановка всех устройств сети](image/5.png){width=70%}

## Запуск захвата пакетов

![Запуск захвата пакетов](image/6.png){width=70%}

## Подтверждение начала захвата

![Подтверждение начала захвата](image/7.png){width=70%}

## Wireshark

![Wireshark](image/8.png){width=60%}

## Запуск всех устройств сети

![Запуск всех устройств сети](image/9.png){width=70%}

## Gratuitous ARP

![Gratuitous ARP](image/10.png){width=70%}

## Ping через ICMP

![Ping через ICMP](image/11.png){width=40%}

## Новые пакеты в Wireshark

![Новые пакеты в Wireshark](image/12.png){width=70%}

## Анализ ICMP пакета

![Анализ ICMP пакета](image/13.png){width=50%}

## Анализ второго ICMP пакета

![Анализ второго ICMP пакета](image/14.png){width=50%}

## ping по протоколу udp

![ping по протоколу udp](image/15.png){width=70%}

## UDP пакеты

![UDP пакеты](image/16.png){width=70%}

## UDP пакет

![UDP пакет](image/17.png){width=50%}

## Второй UDP пакет

![Второй UDP пакет](image/18.png){width=50%}

## ping по TCP

![ping по TCP](image/19.png){width=50%}

## TCP пакет

![TCP пакет](image/20.png){width=60%}

## TCP Echo пакет

![TCP Echo пакет](image/21.png){width=50%}

## Остановка захвата пакетов

![Остановка захвата пакетов](image/22.png){width=70%}

## Создание нового проекта

![Создание нового проекта](image/23.png){width=70%}

## Схема сети

![Схема сети](image/24.png){width=70%}

## Захват пакетов

![Захват пакетов](image/25.png){width=70%}

## Подтверждение захвата

![Подтверждение захвата](image/26.png){width=70%}

## Запуск всех устройств в сети

![Запуск всех устройств в сети](image/27.png){width=70%}

## Открытие консоли

![Открытие консоли](image/28.png){width=70%}

## Консоли

![Консоли](image/29.png){width=70%}

## Настройка терминала

![Настройка терминала](image/30.png){width=40%}

## Настройка роутера

![Настройка роутера](image/31.png){width=40%}

## Айпи eth0

![Айпи eth0](image/32.png){width=50%}

## Ping к роутеру

![Ping к роутеру](image/33.png){width=70%}

## Пакеты

![Пакеты](image/34.png){width=70%}

## Пакет

![Пакет](image/35.png){width=50%}

## Остановка захвата пакетов

![Остановка захвата пакетов](image/36.png){width=70%}

## Выключение всех устройств сети

![Выключение всех устройств сети](image/37.png){width=70%}

## Создание нового проекта

![Создание нового проекта](image/38.png){width=70%}

## Схема сети

![Схема сети](image/39.png){width=70%}

## Захват пакетов

![Захват пакетов](image/40.png){width=70%}

## Подтверждение захвата

![Подтверждение захвата](image/41.png){width=70%}

## Включение устройств сети

![Включение устройств сети](image/42.png){width=70%}

## Консоли

![Консоли](image/43.png){width=70%}

## Вид консолей

![Вид консолей](image/44.png){width=70%}

## Настройка клиента

![Настройка клиента](image/45.png){width=50%}

## Настройка vyos

![Настройка vyos](image/46.png){width=50%}

## Конфигурация

![Конфигурация](image/47.png){width=60%}

## Удаление dhcp

![Удаление dhcp](image/48.png){width=50%}

## Сохранение изменений

![Сохранение изменений](image/49.png){width=70%}

## Ping

![Ping](image/50.png){width=70%}

## Пакеты

![Пакеты](image/51.png){width=50%}

## Остановка захвата пакетов

![Остановка захвата пакетов](image/52.png){width=70%}

## Остановка устройств

![Остановка устройств](image/53.png){width=70%}

## Выводы

В результате выполнения лабораторной работы были получены навыки работы с простейшими моделями сети, их моделированием и анализом трафика в Wireshark
