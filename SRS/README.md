# Требования к проекту 

Содержание
=================
* 1 [Введение](#1-введение)
* 2 [Требования пользователя](#2-требования-пользователя)
  * 2.1 [Программные интерфейсы](#21-программные-интерфейсы)
  * 2.2 [Интерфейс пользователя](#22-интерфейс-пользователя)
  * 2.3 [Характеристики пользователей](#23-характеристики-пользователей)
* 3 [Системные требования](#3-системные-требования)
  * 3.1 [Функциональные требования](#31-функциональные-требования)
  * 3.2 [Программные требования](#32-программные-требования)


## 1. Введение
В этом документе описаны требования к приложению "Avia tickets".
Продукт является полноценным кроссплатформенным адаптивным приложением и представляет собой платформу для мониторинга авиабилетов.
Пользователь использующий данное приложение может искать авиабилеты по указанным критериям (место отправления, место прибытия, дата отправления), просматривать авиабилеты, также пользователь может сохранять билеты добавляя их в корзину. Выполнив поиск билетов, пользователь может получить информацию о стоимости билетов и компании, которая осуществляет его продажу.

## 2. Требования пользователя

### 2.1 Программные интерфейсы
Проект включает в себя только клиентскую часть. Клиент должен быть реализован с использованием современных фронтенд технологий, в частности такой фреймворк как React.js. Пользователь должен иметь возможность поменять цветовую тему приложения. 
Информация о билетах получается из API Travelpayouts.

### 2.2 Интерфейс пользователя

При входе в приложение пользователь оказывается на главной странице. Здесь он может изменить тему приложения (при выходе с сайта и повторном открытии выбранная тема должна сохраняться):

1) Темная тема

![image](https://user-images.githubusercontent.com/68506750/198299191-d4e7d9bf-dbce-4bab-8e5b-3d7a1c043761.png)

2) Светлая тема

![image](https://user-images.githubusercontent.com/68506750/198299321-61a1f594-27de-4681-87d3-20b13cddf720.png)

3) Стандартная тема

![image](https://user-images.githubusercontent.com/68506750/198299440-1ff7addf-0673-45b0-97df-e2f5be441977.png)

На главной странице находится форма, в которой пользователь задаёт критерии для поиска авиабилетов. Для поиска билетов пользователь обязательно должен ввести места прибытия и отправления, а дату отправления можно не вводить.

![image](https://user-images.githubusercontent.com/68506750/198300365-4a691ba9-00b4-45a2-ad62-e58a581d7619.png)

После нажатия кнопки "Search" должен происходить переход на страницу с найденными билетами. На данной странице должна быть предусмотрена сортировка билетов по различным характеристикам (цена, продающая компания, дата отправления), возврат на страницу поиска, а также бесконечная подгрузка новых билетов. 

![image](https://user-images.githubusercontent.com/68506750/198307098-03e3859b-8401-4806-a40b-6fe5a8445f0c.png)

На данной странице должна быть предусмотрена функция добавления билета в корзину. 

![image](https://user-images.githubusercontent.com/68506750/198307206-2cc2324c-b24d-4926-a3cc-0ac855c13954.png)

Должна быть корзина, в которой пользователь может просмотреть выбранные билеты, увеличить их количество, посмотреть их общую стоимость, удалить ненужные билеты. Также должна быть предусмотренна функция сохранения содержимого корзины при выходе с сайта.

![image](https://user-images.githubusercontent.com/68506750/198302945-f2f7170a-9716-4d55-be29-4c30ca77f030.png)


### 2.3 Характеристики пользователей

#### 2.3.1 Классификация пользователей

В данном приложении существует один вид пользователей, который может использовать весь функционал приложения.

#### 2.3.2 Целевая аудитория

Данным приложением могут пользоваться люди различных возрастных групп, которые заинтересованы в поиске авиабилетов.

## 3. Системные требования

### 3.1 Функциональные требования
Должны быть реализованы следующие возможности:
1. Смена темы приложения
2. Поиск билетов по месту прибытия, месту отправления и даты отправления.
3. Сортировка найденных билетов по различным параметрам (цена, дата отправления, продающая компания).
4. Добавление билетов в корзину.
5. Сохранение содержимого корзины при выходе с сайта.

### 3.2 Программные требования
1. Версия React.js 16.0 и выше.
2. Поддерживаемые браузеры: Google Chrome версии 96.0 и выше, Mozilla Firefox версии 98.0 и выше, Opera версии 70.0 и выше, Microsoft Edge версии 100 и выше
3. Язык приложения английский.
