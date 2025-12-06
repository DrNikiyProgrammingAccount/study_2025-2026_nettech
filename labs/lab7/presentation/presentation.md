---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 7
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

Получение навыков настройки службы DHCP на сетевом оборудовании для распределения адресов IPv4 и IPv6.

## Создание нового проекта в GNS3

![Создание нового проекта в GNS3](image/1.png){height=60%}

## Топология сети для настройки DHCPv4

![Топология сети для настройки DHCPv4](image/2.png){height=60%}

## Запуск захвата трафика в Wireshark

![Запуск захвата трафика в Wireshark](image/3.png){height=60%}

## Базовая настройка маршрутизатора VyOS

![Базовая настройка маршрутизатора VyOS](image/4.png){height=60%}

## Удаление стандартного пользователя

![Удаление стандартного пользователя](image/5.png){height=60%}

## Настройка IPv4 адресации и DHCP-сервера

![Настройка IPv4 адресации и DHCP-сервера](image/6.png){height=60%}

## Проверка статистики DHCP-сервера

![Проверка статистики DHCP-сервера](image/7.png){height=60%}

## Получение IP-адреса на клиенте PC1 (процесс DORA)

![Получение IP-адреса на клиенте PC1 (процесс DORA)](image/8.png){height=60%}

## Проверка списка выданных адресов (Leases)

![Проверка списка выданных адресов (Leases)](image/9.png){height=60%}

## Просмотр логов DHCP-сервера

![Просмотр логов DHCP-сервера](image/10.png){height=60%}

## Детальный анализ логов работы DHCP

![Детальный анализ логов работы DHCP](image/11.png){height=60%}

## Анализ DHCP пакетов в Wireshark

![Анализ DHCP пакетов в Wireshark](image/12.png){height=60%}

## Расширенная топология для настройки DHCPv6

![Расширенная топология для настройки DHCPv6](image/13.png){height=60%}

## Настройка IPv6 адресов на интерфейсах

![Настройка IPv6 адресов на интерфейсах](image/14.png){height=60%}

## Настройка Stateless DHCPv6 на интерфейсе eth1

![Настройка Stateless DHCPv6 на интерфейсе eth1](image/15.png){height=60%}

## Просмотр конфигурации маршрутизатора

![Просмотр конфигурации маршрутизатора](image/16.png){height=60%}

## Проверка автоконфигурации IPv6 (SLAAC) на PC2

![Проверка автоконфигурации IPv6 (SLAAC) на PC2](image/17.png){height=60%}

## Получение DNS-настроек через Stateless DHCPv6 на PC2

![Получение DNS-настроек через Stateless DHCPv6 на PC2](image/18.png){height=60%}

## Проверка таблицы аренды DHCPv6 (Stateless)

![Проверка таблицы аренды DHCPv6 (Stateless)](image/19.png){height=60%}

## Анализ пакетов Stateless DHCPv6 в Wireshark

![Анализ пакетов Stateless DHCPv6 в Wireshark](image/20.png){height=60%}

## Настройка Stateful DHCPv6 на интерфейсе eth2

![Настройка Stateful DHCPv6 на интерфейсе eth2](image/21.png){height=60%}

## Проверка таблицы аренды перед подключением клиента

![Проверка таблицы аренды перед подключением клиента](image/22.png){height=60%}

## Начальное состояние сети на PC3

![Начальное состояние сети на PC3](image/23.png){height=60%}

## Получение адреса через Stateful DHCPv6 на PC3

![Получение адреса через Stateful DHCPv6 на PC3](image/24.png){height=60%}

## Проверка сетевых настроек на PC3 после работы DHCPv6

![Проверка сетевых настроек на PC3 после работы DHCPv6](image/25.png){height=60%}

## Проверка таблицы аренды DHCPv6 (Stateful) с активной записью

![Проверка таблицы аренды DHCPv6 (Stateful) с активной записью](image/26.png){height=60%}

## Анализ пакетов Stateful DHCPv6 в Wireshark

![Анализ пакетов Stateful DHCPv6 в Wireshark](image/27.png){height=60%}

## Выводы

В результате выполнения лабораторной работы были получены навыки использования и настройки dhcpv6
