## Описание

Проект YaMDb собирает отзывы пользователей на произведения. Сами произведения в YaMDb не хранятся, здесь нельзя посмотреть фильм или послушать музыку.

http://127.0.0.1:8000/redoc/ Документация для YaMDb


## Технологии

Python 3.7

Django 3.2

DRF

JWT + Djoser


## Установка

Скопируйте репозиторий в свою папку: 

```
https://github.com/Ekaterishe4ka/api_yamdb
```

Установите виртуальное окружение: 

```
python -m venv venv
```

Активируйте виртуальное окружение: 

```
source venv/Scripts/activate
```

Установите зависимости из requirements.txt: 

```
pip install -r requirements.txt
```

Выполните миграции: 

```
python manage.py migrate
```

Запустите сервер: 

```
python manage.py runserver
```

## Примеры запросов к API

Регистрация нового пользователя: 

```
POST /api/v1/auth/signup/
```

Получение данных своей учетной записи:

```
GET /api/v1/users/me/
```


Получение списка всех отзывов:

```
GET /api/v1/titles/{title_id}/reviews/
```

Добавление комментария к отзыву:

```
POST /api/v1/titles/{title_id}/reviews/{review_id}/comments/
```

Добавление новой категории:

```
POST /api/v1/categories/
```

Удаление жанра:

```
DELETE /api/v1/genres/{slug}
```

Частичное обновление информации о произведении:

```
PATCH /api/v1/titles/{titles_id}
```

Полный список запросов API находятся в документации.

## Авторы проекта

Екатерина Богомолова https://github.com/Ekaterishe4ka
Данил Аникин https://github.com/BestTpaktop
Артем Беспалов https://github.com/Artem-Bespalov
