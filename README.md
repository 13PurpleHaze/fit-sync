# Fit-sync

## About The Project

Frontend - https://github.com/13PurpleHaze/fit-sync-frontend
Backend - https://github.com/13PurpleHaze/fit-sync-backend
Видео с функционалом приложения - https://youtu.be/2lfmJYTn4vQ


Проект представляет собой приложение для совместных тренировок в режиме реального времени. Основной функционал заключается в том, что пользователи создают тренировки на основе упражнений и тренируются по ним, приглашая других пользователей в свою тренировку. В рамках каждой тренировочной сессии доступен чат, а результаты выполнения упражнений отображаются пользователям в режиме реального времени. После тренировки пользователь может посмотреть свою историю.

Функционал обычного пользователя
* Создание, удаление, обновление тернировок
* Просмотр истории тренировок
* Возможность тренироваться в группе до 5 человек
* Чат во время тренировки


Функционал администратора
* Добавление пользователей
* Блокировка или разблокировка пользователей
* Добавление, обновление, удаление упражнений


### Built With

Проект создан с использованием следующих технологий

На клиентской стороне
* ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
* ![Mobx](https://camo.githubusercontent.com/1705f2440ee444c8b69a7c7b72ab06f83afc6ccf09e61ed0e47a91bef0bb20a6/68747470733a2f2f696d672e736869656c64732e696f2f7374617469632f76313f7374796c653d666f722d7468652d6261646765266d6573736167653d4d6f625826636f6c6f723d323232323232266c6f676f3d4d6f6258266c6f676f436f6c6f723d464639393535266c6162656c3d)

На серверной стороне
* ![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
* ![Express.js](https://img.shields.io/badge/Express.*js-404D59?style=for-the-badge)
* ![Socket.io](https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&badgeColor=010101)
* ![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
* ![Redis](https://img.shields.io/badge/redis-222222.svg?style=for-the-badge&logo=redis&logoColor=red)

Все изображения храняться в yandex-object-storage, для валидации используется react-hook-form и express-validator


## Getting Started

### Installation

1. Клонируйте репозиторий
   ```sh
   git clone https://github.com/13PurpleHaze/fit-sync.git
   ```
2. Установите docker и docker-compose
3. В файле docker-compose.yaml измените параметры конфигурации на свои если это вам нужно.
4. В директории проета запустите следующие команды
    ```sh
    docker-compose build
    docker-compose up
    ```
PS. т.к. приложение хранит картинки в yandex object storage вы должны изменить переменные на свои значения. Либо использовать те, что находяться в файле docker-compose.yaml.
  YANDEX_USER_KEY: ***
  YANDEX_USER_SECRET_KEY: ***
  YANDEX_REGION: ru-central1
  BUCKET_NAME: ***


## Usage

Перейдите по адресу http://localhost:3000 (в том случае если вы не меняли порт в docker-compose.yaml)
Данные для входа:
 * login - nikita1 - password - 123
 * login - anna1 - password - 123


## Contact

Nikita - [@purplehazedp](https://t.me/purplehazedp)