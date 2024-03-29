# Определение перспективного тарифа для телеком-компании
## Описание проекта

Клиентам компании «Мегалайн», федерального оператора сотовой связи, предлагают два тарифных плана: «Смарт» и «Ультра». Чтобы скорректировать рекламный бюджет, коммерческий департамент хочет понять, какой тариф приносит больше денег.
Нужно сделать предварительный анализ тарифов на небольшой выборке клиентов. В нашем распоряжении данные 500 пользователей «Мегалайна»: кто они, откуда, каким тарифом пользуются, сколько звонков и сообщений каждый отправил за 2018 год. Нужно проанализировать поведение клиентов и сделать вывод — какой тариф лучше.

**Заказчик проекта** - коммерческий деппартамент.\
**Цель проекта** - определить, какой из двух тарифов приносит больший доход компании, проверить следующие гипотезы:
- средняя выручка пользователей тарифов «Ультра» и «Смарт» различаются;
- средняя выручка пользователей из Москвы отличается от выручки пользователей из других регионов.

###### Описание тарифов

**Тариф «Смарт»**
    
Ежемесячная плата: 550 рублей\
Включено 500 минут разговора, 50 сообщений и 15 Гб интернет-трафика\
Стоимость услуг сверх тарифного пакета:\
минута разговора: 3 рубля\
сообщение: 3 рубля\
1 Гб интернет-трафика: 200 рублей
    
**Тариф «Ультра»**  
    
Ежемесячная плата: 1950 рублей\
Включено 3000 минут разговора, 1000 сообщений и 30 Гб интернет-трафика\
Стоимость услуг сверх тарифного пакета:\
минута разговора: 1 рубль\
сообщение: 1 рубль\
1 Гб интернет-трафика: 150 рублей

###### Примечание:
    
«Мегалайн» всегда округляет секунды до минут, а мегабайты — до гигабайт. Каждый звонок округляется отдельно: даже если он длился всего 1 секунду, будет засчитан как 1 минута.\
Для веб-трафика отдельные сессии не считаются. Вместо этого общая сумма за месяц округляется в бо́льшую сторону. Если абонент использует 1025 мегабайт в этом месяце, с него возьмут плату за 2 гигабайта.

**Ход проекта**\
В ходе проекта проверим исходные данные, при необходимости проведем их обработку, затем рассчитаем помесячную выручку от каждого клиента, проанализируем поведение абонентов и проверим сформулированные выше гипотезы.\
Основные этапы проекта:

- Обзор данных,
- Предобработка данных,
- Расчеты и добавление результатов в таблицу,
- Анализ данных,
- Проверка гипотез,
- Выводы.