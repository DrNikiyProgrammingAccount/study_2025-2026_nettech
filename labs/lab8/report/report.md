---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа 8"
author: "Андрюшин Никита Сергеевич"

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
lot: true # List of tables
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

Изучение принципов маршрутизации в IPv4- и IPv6-сетях и принципов настройки сетевого оборудования

# Выполнение работы

Создадим новый проект в GNS3 с именем «lab8» (рис. [-@fig:001]).

![Создание проекта в GNS3](image/1.png){#fig:001}

Соберём топологию сети согласно заданию, разместив коммутаторы, маршрутизаторы FRR и оконечные устройства (рис. [-@fig:002]).

![Топология сети в GNS3](image/2.png){#fig:002}

Настроим IP-адрес и шлюз по умолчанию на PC1 (рис. [-@fig:003]).

![Настройка IPv4 на PC1](image/3.png){#fig:003}

Настроим IP-адрес и шлюз по умолчанию на PC2 (рис. [-@fig:004]).

![Настройка IPv4 на PC2](image/4.png){#fig:004}

На маршрутизаторе gw-01 зададим имя хоста и настроим IPv4-адреса на интерфейсах eth0, eth1 и eth2 (рис. [-@fig:005]).

![Базовая настройка gw-01](image/5.png){#fig:005}

На маршрутизаторе gw-02 зададим имя хоста и настроим IPv4-адреса на интерфейсах eth0 и eth1 (рис. [-@fig:006]).

![Базовая настройка gw-02](image/6.png){#fig:006}

На маршрутизаторе gw-03 зададим имя хоста и настроим IPv4-адреса на интерфейсах eth0, eth1 и eth2 (рис. [-@fig:007]).

![Базовая настройка gw-03](image/7.png){#fig:007}

На маршрутизаторе gw-04 зададим имя хоста и настроим IPv4-адреса на интерфейсах eth0 и eth1 (рис. [-@fig:008]).

![Базовая настройка gw-04](image/8.png){#fig:008}

Настроим IPv6-адрес на PC1 (рис. [-@fig:009]).

![Настройка IPv6 на PC1](image/9.png){#fig:009}

Настроим IPv6-адрес на PC2 (рис. [-@fig:010]).

![Настройка IPv6 на PC2](image/10.png){#fig:010}

На маршрутизаторе gw-01 включим маршрутизацию IPv6 (forwarding) и настроим IPv6-адреса на интерфейсах (рис. [-@fig:011]).

![Настройка IPv6 на gw-01](image/11.png){#fig:011}

На маршрутизаторе gw-02 включим маршрутизацию IPv6 и настроим адреса на интерфейсах (рис. [-@fig:012]).

![Настройка IPv6 на gw-02](image/12.png){#fig:012}

На маршрутизаторе gw-03 включим маршрутизацию IPv6 и настроим адреса на интерфейсах (рис. [-@fig:013]).

![Настройка IPv6 на gw-03](image/13.png){#fig:013}

На маршрутизаторе gw-04 включим маршрутизацию IPv6 и настроим адреса на интерфейсах (рис. [-@fig:014]).

![Настройка IPv6 на gw-04](image/14.png){#fig:014}

Настроим протокол динамической маршрутизации RIP версии 2 на маршрутизаторе gw-01, объявив подключенные сети (рис. [-@fig:015]).

![Настройка RIPv2 на gw-01](image/15.png){#fig:015}

Настроим протокол RIP версии 2 на маршрутизаторе gw-02 (рис. [-@fig:016]).

![Настройка RIPv2 на gw-02](image/16.png){#fig:016}

Настроим протокол RIP версии 2 на маршрутизаторе gw-03 (рис. [-@fig:017]).

![Настройка RIPv2 на gw-03](image/17.png){#fig:017}

Настроим протокол RIP версии 2 на маршрутизаторе gw-04 (рис. [-@fig:018]).

![Настройка RIPv2 на gw-04](image/18.png){#fig:018}

Проверим таблицу маршрутизации и статус протокола RIP на gw-01 (рис. [-@fig:019]).

![Проверка RIP на gw-01](image/19.png){#fig:019}

Проверим таблицу маршрутизации и статус протокола RIP на gw-02 (рис. [-@fig:020]).

![Проверка RIP на gw-02](image/20.png){#fig:020}

Проверим таблицу маршрутизации и статус протокола RIP на gw-03 (рис. [-@fig:021]).

![Проверка RIP на gw-03](image/21.png){#fig:021}

Проверим таблицу маршрутизации и статус протокола RIP на gw-04 (рис. [-@fig:022]).

![Проверка RIP на gw-04](image/22.png){#fig:022}

Проверим связность между PC1 и PC2 с помощью утилит ping и trace. Трассировка показывает прохождение пакетов через gw-04 (рис. [-@fig:023]).

![Проверка связности IPv4](image/23.png){#fig:023}

Посмотрим метрики маршрутов в таблице RIP на gw-01 (рис. [-@fig:024]).

![Таблица RIP на gw-01](image/24.png){#fig:024}

Для проверки отказоустойчивости выключим интерфейс eth0 на маршрутизаторе gw-04 (рис. [-@fig:025]).

![Отключение интерфейса на gw-04](image/25.png){#fig:025}

Убедимся, что маршрут через отключенный интерфейс стал недоступен (метрика 16) в таблице маршрутизации gw-01 (рис. [-@fig:026]).

![Изменение метрик RIP после сбоя](image/26.png){#fig:026}

Включим интерфейс eth0 на маршрутизаторе gw-04 обратно (рис. [-@fig:027]).

![Включение интерфейса на gw-04](image/27.png){#fig:027}

Проверим доступность удаленного узла с PC1. Наблюдаем потери пакетов и незавершенную трассировку, что говорит о процессе перестроения маршрута (рис. [-@fig:028]).

![Проверка доступности во время сходимости](image/28.png){#fig:028}

Проанализируем захваченные пакеты протокола RIPv2 в Wireshark (рис. [-@fig:029]).

![Анализ пакетов RIPv2 в Wireshark](image/29.png){#fig:029}

Настроим протокол RIPng (для IPv6) на маршрутизаторе gw-01 (рис. [-@fig:030]).

![Настройка RIPng на gw-01](image/30.png){#fig:030}

Настроим протокол RIPng на маршрутизаторе gw-02 (рис. [-@fig:031]).

![Настройка RIPng на gw-02](image/31.png){#fig:031}

Настроим протокол RIPng на маршрутизаторе gw-03 (рис. [-@fig:032]).

![Настройка RIPng на gw-03](image/32.png){#fig:032}

Настроим протокол RIPng на маршрутизаторе gw-04 (рис. [-@fig:033]).

![Настройка RIPng на gw-04](image/33.png){#fig:033}

Проверим IPv6-связность между PC1 и PC2. Трассировка показывает маршрут через gw-02 (рис. [-@fig:034]).

![Проверка связности IPv6](image/34.png){#fig:034}

Просмотрим таблицу маршрутизации RIPng на gw-01 (рис. [-@fig:035]).

![Таблица RIPng на gw-01](image/35.png){#fig:035}

Сымитируем сбой, отключив интерфейс eth0 на маршрутизаторе gw-04 (рис. [-@fig:036]).

![Отключение интерфейса IPv6 на gw-04](image/36.png){#fig:036}

Посмотрим изменения в таблице маршрутизации RIPng на gw-01 (рис. [-@fig:037]).

![Изменения в таблице RIPng](image/37.png){#fig:037}

Снова проверим доступность узлов с PC1 (рис. [-@fig:038]).

![Проверка трассировки IPv6 после сбоя](image/38.png){#fig:038}

В Wireshark наблюдаем ICMPv6 сообщения о превышении лимита времени (Time Exceeded), что свидетельствует о проблемах маршрутизации (петлях) в момент сходимости (рис. [-@fig:039]).

![ICMPv6 Time Exceeded в Wireshark](image/39.png){#fig:039}

Также в трафике присутствуют запросы и ответы ping (Echo) и пакеты RIPng (рис. [-@fig:040]).

![Анализ IPv6 трафика в Wireshark](image/40.png){#fig:040}

Перейдем к настройке OSPF. На маршрутизаторе gw-01 настроим процесс OSPF и привяжем сети к зоне 0 (рис. [-@fig:041]).

![Настройка OSPF на gw-01](image/41.png){#fig:041}

Настроим OSPF на маршрутизаторе gw-02, указав сети и зону (рис. [-@fig:042]).

![Настройка OSPF на gw-02](image/42.png){#fig:042}

Настроим OSPF на маршрутизаторе gw-03 (рис. [-@fig:043]).

![Настройка OSPF на gw-03](image/43.png){#fig:043}

Настроим OSPF на маршрутизаторе gw-04 (рис. [-@fig:044]).

![Настройка OSPF на gw-04](image/44.png){#fig:044}

Проверим связность с помощью ping и trace с PC1. Трассировка показывает маршрут через gw-02 (рис. [-@fig:045]).

![Проверка связности через OSPF](image/45.png){#fig:045}

Посмотрим список соседей OSPF и таблицу маршрутизации на gw-01 (рис. [-@fig:046]).

![Таблица соседей и маршрутов OSPF на gw-01](image/46.png){#fig:046}

Повторно выведем информацию о соседях и маршрутах OSPF на gw-01 (рис. [-@fig:047]).

![Мониторинг OSPF на gw-01](image/47.png){#fig:047}

Снова выполним трассировку маршрута с PC1 до PC2 (рис. [-@fig:048]).

![Повторная трассировка IPv4](image/48.png){#fig:048}

Убедимся, что интерфейс eth0 на gw-04 включен (команда `no shutdown`) (рис. [-@fig:049]).

![Включение интерфейса на gw-04](image/49.png){#fig:049}

Проверим трассировку маршрута; теперь трафик может идти через gw-04 (рис. [-@fig:050]).

![Трассировка через восстановленный маршрут](image/50.png){#fig:050}

В Wireshark проанализируем пакеты, среди которых видны сообщения ICMPv6 о недоступности назначения и превышении времени (рис. [-@fig:051]).

![Анализ ошибок ICMPv6 в Wireshark](image/51.png){#fig:051}

Продолжаем наблюдение за служебным трафиком OSPF Hello и RIPv2 в Wireshark (рис. [-@fig:052]).

![Анализ OSPF и RIP трафика](image/52.png){#fig:052}

Зафиксируем ICMP-запросы и ARP-пакеты в Wireshark (рис. [-@fig:053]).

![Анализ ICMP и ARP](image/53.png){#fig:053}

Наблюдаем TCP-ретрансмиссии и сообщения об истечении времени жизни пакета (Time-to-live exceeded) в Wireshark (рис. [-@fig:054]).

![Анализ ошибок TCP и ICMP](image/54.png){#fig:054}

Настроим OSPFv3 для IPv6 на маршрутизаторе gw-01, задав router-id 1.1.1.1 и привязав интерфейсы к зоне 0 (рис. [-@fig:055]).

![Настройка OSPFv3 на gw-01](image/55.png){#fig:055}

Настроим OSPFv3 на маршрутизаторе gw-02 с router-id 2.2.2.2 (рис. [-@fig:056]).

![Настройка OSPFv3 на gw-02](image/56.png){#fig:056}

Настроим OSPFv3 на маршрутизаторе gw-03 с router-id 3.3.3.3 (рис. [-@fig:057]).

![Настройка OSPFv3 на gw-03](image/57.png){#fig:057}

Настроим OSPFv3 на маршрутизаторе gw-04 с router-id 4.4.4.4 (рис. [-@fig:058]).

![Настройка OSPFv3 на gw-04](image/58.png){#fig:058}

Проверим IPv6-связность с PC1. Трассировка проходит успешно (рис. [-@fig:059]).

![Проверка связности OSPFv3](image/59.png){#fig:059}

Проверим таблицу соседей и маршрутов OSPFv3 на gw-01 (рис. [-@fig:060]).

![Проверка OSPFv3 на gw-01](image/60.png){#fig:060}

В Wireshark наблюдаем сообщения ICMPv6 Time Exceeded, свидетельствующие о проблемах доставки пакетов (рис. [-@fig:061]).

![Анализ ошибок Time Exceeded в Wireshark](image/61.png){#fig:061}

Фиксируем сообщения ICMPv6 Destination Unreachable (Port unreachable) в трафике (рис. [-@fig:062]).

![Анализ ошибок Destination Unreachable](image/62.png){#fig:062}

Продолжаем наблюдать поток ошибок Destination Unreachable в Wireshark (рис. [-@fig:063]).

![Продолжение анализа ошибок в Wireshark](image/63.png){#fig:063}

Создадим новый проект «lab8-1» для выполнения следующей части задания (рис. [-@fig:064]).

![Создание проекта lab8-1](image/64.png){#fig:064}

Соберем новую топологию сети с использованием маршрутизаторов VyOS (рис. [-@fig:065]).

![Топология с VyOS](image/65.png){#fig:065}

# Выводы

В результате выполнения лабораторной работы были получены навыки настройки маршрутизации
