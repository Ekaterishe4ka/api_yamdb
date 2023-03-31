# Описание

Проект YaMDb собирает отзывы пользователей на произведения. Сами произведения в YaMDb не хранятся, здесь нельзя посмотреть фильм или послушать музыку.

http://127.0.0.1:8000/redoc/ Документация для YaMDb

# Системные требования
- Python 3.7+
- Works on Linux, Windows, macOS

# Стек технологий

- Python 3.7

- Django 3.2

- DRF

- JWT + Djoser

# Установка

Клонировать репозиторий и перейти в него в командной строке:

```
https://github.com/Ekaterishe4ka/api_yamdb.git
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект: 

```
python3 manage.py runserver
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
