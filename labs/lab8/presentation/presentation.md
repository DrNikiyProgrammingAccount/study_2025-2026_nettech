---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 8
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

Изучение принципов маршрутизации в IPv4- и IPv6-сетях и принципов настройки сетевого оборудования

## 

![Создание проекта в GNS3](image/1.png){#fig:001}

## 

![Топология сети в GNS3](image/2.png){#fig:002}

## 

![Настройка IPv4 на PC1](image/3.png){#fig:003}

## 

![Настройка IPv4 на PC2](image/4.png){#fig:004}

## 

![Базовая настройка gw-01](image/5.png){#fig:005}

## 

![Базовая настройка gw-02](image/6.png){#fig:006}

## 

![Базовая настройка gw-03](image/7.png){#fig:007}

## 

![Базовая настройка gw-04](image/8.png){#fig:008}

## 

![Настройка IPv6 на PC1](image/9.png){#fig:009}

## 

![Настройка IPv6 на PC2](image/10.png){#fig:010}

## 

![Настройка IPv6 на gw-01](image/11.png){#fig:011}

## 

![Настройка IPv6 на gw-02](image/12.png){#fig:012}

## 

![Настройка IPv6 на gw-03](image/13.png){#fig:013}

## 

![Настройка IPv6 на gw-04](image/14.png){#fig:014}

## 

![Настройка RIPv2 на gw-01](image/15.png){#fig:015}

## 

![Настройка RIPv2 на gw-02](image/16.png){#fig:016}

## 

![Настройка RIPv2 на gw-03](image/17.png){#fig:017}

## 

![Настройка RIPv2 на gw-04](image/18.png){#fig:018}

## 

![Проверка RIP на gw-01](image/19.png){#fig:019}

## 

![Проверка RIP на gw-02](image/20.png){#fig:020}

## 

![Проверка RIP на gw-03](image/21.png){#fig:021}

## 

![Проверка RIP на gw-04](image/22.png){#fig:022}

## 

![Проверка связности IPv4](image/23.png){#fig:023}

## 

![Таблица RIP на gw-01](image/24.png){#fig:024}

## 

![Отключение интерфейса на gw-04](image/25.png){#fig:025}

## 

![Изменение метрик RIP после сбоя](image/26.png){#fig:026}

## 

![Включение интерфейса на gw-04](image/27.png){#fig:027}

## 

![Проверка доступности во время сходимости](image/28.png){#fig:028}

## 

![Анализ пакетов RIPv2 в Wireshark](image/29.png){#fig:029}

## 

![Настройка RIPng на gw-01](image/30.png){#fig:030}

## 

![Настройка RIPng на gw-02](image/31.png){#fig:031}

## 

![Настройка RIPng на gw-03](image/32.png){#fig:032}

## 

![Настройка RIPng на gw-04](image/33.png){#fig:033}

## 

![Проверка связности IPv6](image/34.png){#fig:034}

## 

![Таблица RIPng на gw-01](image/35.png){#fig:035}

## 

![Отключение интерфейса IPv6 на gw-04](image/36.png){#fig:036}

## 

![Изменения в таблице RIPng](image/37.png){#fig:037}

## 

![Проверка трассировки IPv6 после сбоя](image/38.png){#fig:038}

## 

![ICMPv6 Time Exceeded в Wireshark](image/39.png){#fig:039}

## 

![Анализ IPv6 трафика в Wireshark](image/40.png){#fig:040}

## 

![Настройка OSPF на gw-01](image/41.png){#fig:041}

## 

![Настройка OSPF на gw-02](image/42.png){#fig:042}

## 

![Настройка OSPF на gw-03](image/43.png){#fig:043}

## 

![Настройка OSPF на gw-04](image/44.png){#fig:044}

## 

![Проверка связности через OSPF](image/45.png){#fig:045}

## 

![Таблица соседей и маршрутов OSPF на gw-01](image/46.png){#fig:046}

## 

![Мониторинг OSPF на gw-01](image/47.png){#fig:047}

## 

![Повторная трассировка IPv4](image/48.png){#fig:048}

## 

![Включение интерфейса на gw-04](image/49.png){#fig:049}

## 

![Трассировка через восстановленный маршрут](image/50.png){#fig:050}

## 

![Анализ ошибок ICMPv6 в Wireshark](image/51.png){#fig:051}

## 

![Анализ OSPF и RIP трафика](image/52.png){#fig:052}

## 

![Анализ ICMP и ARP](image/53.png){#fig:053}

## 

![Анализ ошибок TCP и ICMP](image/54.png){#fig:054}

## 

![Настройка OSPFv3 на gw-01](image/55.png){#fig:055}

## 

![Настройка OSPFv3 на gw-02](image/56.png){#fig:056}

## 

![Настройка OSPFv3 на gw-03](image/57.png){#fig:057}

## 

![Настройка OSPFv3 на gw-04](image/58.png){#fig:058}

## 

![Проверка связности OSPFv3](image/59.png){#fig:059}

## 

![Проверка OSPFv3 на gw-01](image/60.png){#fig:060}

## 

![Анализ ошибок Time Exceeded в Wireshark](image/61.png){#fig:061}

## 

![Анализ ошибок Destination Unreachable](image/62.png){#fig:062}

## 

![Продолжение анализа ошибок в Wireshark](image/63.png){#fig:063}

## 

![Создание проекта lab8-1](image/64.png){#fig:064}

## 

![Топология с VyOS](image/65.png){#fig:065}

## Выводы

В результате выполнения лабораторной работы были получены навыки настройки маршрутизации
