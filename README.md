# Yatube API

Yatube API предоставляет интерфейс для взаимодействия с моделями постов, комментариев и групп Yatube. Этот проект реализован с использованием Django и Django REST Framework. 


### Фреймворки и библиотеки

* **Django** : Высокоуровневый веб-фреймворк для быстрой разработки и чистого, прагматичного дизайна. Он предоставляет мощные инструменты и библиотеки для разработки веб-приложений.
* **Django REST Framework (DRF)** : Набор инструментов для построения веб-API на основе Django. DRF предоставляет мощные и гибкие инструменты для создания API, такие как сериализация данных, аутентификация и разрешения.

### Аутентификация

* **Django Rest Framework Token Authentication** : DRF Token Authentication предоставляет простой способ аутентификации пользователей с использованием токенов. Он позволяет клиентам аутентифицироваться, отправляя токен с каждым запросом, что облегчает работу с API.

### Эндпоинты

* `POST /api/v1/api-token-auth/`: Получить токен аутентификации. Отправьте свои `username` и `password`.
* `GET /api/v1/posts/`: Получить список всех постов.
* `POST /api/v1/posts/`: Создать новый пост.
* `GET /api/v1/posts/{post_id}/`: Получить подробную информацию о посте.
* `PUT /api/v1/posts/{post_id}/`: Полностью обновить пост.
* `PATCH /api/v1/posts/{post_id}/`: Частично обновить пост.
* `DELETE /api/v1/posts/{post_id}/`: Удалить пост.
* `GET /api/v1/groups/`: Получить список всех групп.
* `GET /api/v1/groups/{group_id}/`: Получить информацию о группе.
* `GET /api/v1/posts/{post_id}/comments/`: Получить список всех комментариев к посту.
* `POST /api/v1/posts/{post_id}/comments/`: Создать новый комментарий к посту.
* `GET /api/v1/posts/{post_id}/comments/{comment_id}/`: Получить информацию о комментарии.
* `PUT /api/v1/posts/{post_id}/comments/{comment_id}/`: Полностью обновить комментарий.
* `PATCH /api/v1/posts/{post_id}/comments/{comment_id}/`: Частично обновить комментарий.
* `DELETE /api/v1/posts/{post_id}/comments/{comment_id}/`: Удалить комментарий.

### Запуск

* **git clone https://github.com/your-username/yatube-api.git**
* **pip install -r requirements.txt**
* **python manage.py migrate**
* **python manage.py runserver**