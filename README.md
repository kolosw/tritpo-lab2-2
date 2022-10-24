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
  * 3.2 [Нефункциональные требования](#32-нефункциональные-требования)


## 1. Введение
В этом документе описаны требования к приложению "Courseadora".
Продукт является полноценным клиент-серверным кроссплатформенным приложением и представляет собой платформу для онлайн-обучения.
Данное приложение ориентерованно как на студентов, так и на преподавателей. Преподаватели создают курсы, онлайн-уроки, тесты и различные задания для студентов. Студенты же в свою очередь проходят и обучаются по элементам созданными преподавателями. Приложение рассчитано на все возрастные группы, так как курсы могут быть на любую тему.

## 2. Требования пользователя

### 2.1 Программные интерфейсы
Проект включает в себя как клиентскую, так и серверную части.
Клиент должен быть реализован с использованием современных фронтенд технологий, в частности такой библиотеки как React.js.
Серверная часть проекта должна быть реализована с использованием современного JavaScript бэкенд фреймворка Express.js, базы данных MongoDB. 
Пользователь должен иметь возможность поменять язык приложения. Должны быть представлены два языка - Русский и Английский.
Для корректной работы приложения картинки хранятся в бинарном виде в базе данных.

### 2.2 Интерфейс пользователя

Заглавная страница

![image](https://user-images.githubusercontent.com/68506750/197595852-c024613c-6933-4503-aaf0-ced60738156c.png)

Страница входа

![image](https://user-images.githubusercontent.com/68506750/197596485-266492fb-3d1a-4618-b7b5-b02805b0bc7d.png)

Страница регистрации

![image](https://user-images.githubusercontent.com/68506750/197597274-a92da8d2-3e79-4b65-bce8-88e1ed8e2153.png)

Просмотр профиля пользователя

![image](https://user-images.githubusercontent.com/68506750/197599143-ddeeb951-7972-42da-8537-36abdf6b406f.png)

Поиск курсов

![image](https://user-images.githubusercontent.com/68506750/197600238-2c6bfc67-69e7-4213-b656-7e9d272b50ca.png)

### 2.3 Характеристики пользователей

#### 2.3.1 Классификация пользователей

Пользователи разбиваются на 3 группы:
1. Преподователи - это пользователи, которые зарегестрировались и подтвердили своё образование. Данный тип пользователей имеет доступ к созданию различных курсов, а также к проведению онлайн-уроков.
2. Студенты - это пользователи имеющие свой аккаунт на платформе. Они имеют доступ к покупке различных курсов, оцениванию преподователей, участии в онлайн-уроках.
3. Гости - это неавторизованные пользователи. Они имеют доступ только к первой странице приложения, на которой размещена различная информация о стоимости курсов, уроков. 

#### 2.3.2 Целевая аудитория

Данным приложением могут пользоваться люди различных возрастных групп, так как курсы посвящены различным темам и предметам. Особенно восстребованным это приложение будет для преподавателей, так как может являтся как дополнительным заработкам, так и основным. 

## 3. Системные требования

### 3.1 Функциональные требования
Должны быть реализованы следующие возможности:
1. Регистрация пользователей
2. Авторизация пользователей
3. Потдвержедение диплома (сертификата) об образовании преподователей
4. Создание курсов и онлайн-уроков
5. Оценивание и комментирование работы преподователей
6. Оплата занятий

### 3.2 Нефункциональные требования
1. Версия React.js 16.0.
2. Версия Node.js 16.0.
3. Версия Express.js 10.0.
4. Само приложение на React.js + Express.js.
5. Для хранения данных пользователей MongoDB версии 9.0.
6. Во время разработки рекомендуется использовать Docker.
7. Язык приложения русский и английский. В будущем, по мере роста приложения, могут быть добавлены и другие языки 
