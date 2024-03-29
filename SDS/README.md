﻿# Software Development Specification
---

# Содержание
1 [Описание проекта](#описание-проекта)

2 [Системные требования](#системные-требования)

3 [Диаграмма вариантов использования](#диаграмма-вариантов-использования)  

4 [Разработка фронтенда](#разработка-фронтенда)

4 [Диаграммы активностей](#диаграммы-активностей)  

5 [Диаграммы последовательностей](#диаграммы-последовательностей)

6 [Диаграммы состояний](#диаграммы-состояний)  

7 [Диаграмма классов](#диаграмма-классов)  

8 [Диаграмма компонентов и развертывания](#диаграмма-компонентов-и-развертывания)

# Описание проекта

Продукт является полноценным кроссплатформенным адаптивным приложением и представляет собой платформу для мониторинга авиабилетов.
Пользователь использующий данное приложение может искать авиабилеты по указанным критериям (место отправления, место прибытия, дата отправления), просматривать авиабилеты, также пользователь может сохранять билеты добавляя их в корзину. Выполнив поиск билетов, пользователь может получить информацию о стоимости билетов и компании, которая осуществляет его продажу.

# Системные требования

## 1 Функциональные требования
Должны быть реализованы следующие возможности:
1. Смена темы приложения
2. Поиск билетов по месту прибытия, месту отправления и даты отправления.
3. Сортировка найденных билетов по различным параметрам (цена, дата отправления, продающая компания).
4. Добавление билетов в корзину.
5. Сохранение содержимого корзины при выходе с сайта.

## 2 Нефункциональные требования
1. Версия React.js 16.0.
2. Поддерживаемые браузеры: Google Chrome версии 96.0 и выше, Mozilla Firefox версии 98.0 и выше, Opera версии 70.0 и выше, Microsoft Edge версии 100 и выше
3. Язык приложения английский.

# Разработка фронтенда

Для получения информации о билетах на авиарейсы используется Travelpayouts API. Для их получения делается запрос "/travelpayouts/v2/prices". Для более подробной информации нужно использовать [документацию](https://support.travelpayouts.com/hc/en-us/categories/200358578-API-and-data) данного API.
# Диаграмма вариантов использования

## 1 Актёры

| Актёр        | Описание                                                                                         |
| :----------- | :----------------------------------------------------------------------------------------------- |
| Пользователь | Человек, использующий приложение                                                                 |
| Клиент       | Приложение                                                                                       |
| Сервер       | Интернет ресурс для получения расписания авиарейсов (https://support.travelpayouts.com/hc/en-us) |
| Хранилище    | Локальное хранилище, которое хранит забронированные билеты                                       |

## 2 Варианты использования

Use Case диаграммы приложения "Avia tickets":

![useCase vpd (1)](https://user-images.githubusercontent.com/68506750/203756617-b03207af-a13b-415a-bdd6-ea0c16c8ea27.jpg)

### 2.1 Поиск билетов

**Описание.** Вариант использования "Поиск билетов" позволяет пользователю найти авиабилеты.

1. Пользователь выбирает места прибытия и отправления (обязательные параметры).
2. Пользователь может выбрать время отправления с помощью встроенного виджета "Календарь" (необязательный параметр).
4. Клиент валидирует введённые данные.
5. Клиент уведомляет пользователя, если данные введены неверно.
6. Пользователь нажимает кнопку поиска билетов.
7. Клиент выполняет запрос на интернет-ресурс и получает авиабилеты в соответствии с введенными данными.
8. Клиент получает ответ от сервера.
9. Клиент уведомляет пользователя, если произошла ошибка.
10. Клиент уведомляет пользователя, если билеты не были найдены.
11. Клиент перенаправляет пользователя на страницу с найденными билетами.
12. Конец варианта использования.

# Диаграммы активностей

![activityvpd vpd](https://user-images.githubusercontent.com/68506750/203758042-6a535b62-57a5-4810-a9a5-0845e737eb73.jpg)

# Диаграммы последовательностей

![Sequence vpd](https://user-images.githubusercontent.com/68506750/203759821-1f36aae1-90fb-4d01-b588-74d6f66b28f1.jpg)

# Диаграммы состояний

![state vpd](https://user-images.githubusercontent.com/68506750/203758654-86e1995f-23cf-468e-96fe-70dbedfa0467.jpg)

# Диаграмма классов

![image](https://user-images.githubusercontent.com/68506750/203620951-e569945c-bac2-4664-8c40-03aef58b6d51.png)

# Диаграмма компонентов и развертывания

![Components vpd](https://user-images.githubusercontent.com/68506750/203618941-fe10814e-f342-4b14-a4cb-2b9b29123988.jpg)
