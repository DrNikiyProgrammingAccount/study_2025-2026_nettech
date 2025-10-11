---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 3
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

Изучение посредством Wireshark кадров Ethernet, анализ PDU протоколов транспортного и прикладного уровней стека TCP/IP.

## ipconfig

![ipconfig](image/1.png){width=40%}

## ipconfig /all

![ipconfig /all](image/2.png){width=60%}

## Выбор соединения

![Выбор соединения](image/3.png){width=60%}

## Wireshark

![Wireshark](image/4.png){width=60%}

## ping

![ping](image/5.png){width=60%}

## icmp

![icmp](image/6.png){width=60%}

## Анализ исходящего пакета

![Анализ исходящего пакета](image/7.png){width=60%}

## Анализ входящего пакета

![Анализ входящего пакета](image/8.png){width=60%}

## arp

![arp](image/9.png){width=60%}

## Второй arp пакет

![Второй arp пакет](image/10.png){width=60%}

## ping ya.ru

![ping ya.ru](image/11.png){width=60%}

## arp пакеты

![arp пакеты](image/12.png){width=60%}

## Второй arp пакет

![Второй arp пакет](image/13.png){width=60%}

## Исходящий пакет icmp

![Исходящий пакет icmp](image/14.png){width=50%}

## Входящий пакет icmp

![Входящий пакет icmp](image/15.png){width=60%}

## Подключение по http

![Подключение по http](image/16.png){width=60%}

## Исходящий http пакет

![Исходящий http пакет](image/17.png){width=50%}

## Входящий http пакет

![Входящий http пакет](image/18.png){width=50%}

## Исходящий dns пакет

![Исходящий dns пакет](image/19.png){width=60%}

## Входящий dns пакет

![Входящий dns пакет](image/20.png){width=50%}

## Исходящий quic пакет

![Исходящий quic пакет](image/21.png){width=60%}

## Входящий quic пакет

![Входящий quic пакет](image/22.png){width=60%}

## syn

![syn](image/23.png){width=6=50%}

## syn + ack

![syn + ack](image/24.png){width=50%}

## ack

![ack](image/25.png){width=50%}

## Хендшейк на графике потока

![Хендшейк на графике потока](image/26.png){width=50%}

## Выводы

В результате выполнения работы были получены навыки анализа пакетов в wireshark
