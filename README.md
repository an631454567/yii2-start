yii2-blog
=========

- Простой демо блог на Yii 2.
- Рабочий пример можно посмотреть тут: http://yii2-blog.find-freelancer.pro/www/
- Для входа: Login: Amin; Password: Admin11; | Login: test1; Password: Test11;

Модули
-----------
- Блоги: возможность создавать пост, удалять и редактировать свои существующие посты. Админу доступны все функции для всех постов.
- Комментарии: любой зарегистрированный пользователь может добавить комментарий. Или отредактировать/удалить уже существующий свой коммент. Админ может управлять любыми комментариями.
- Пользователи: простой модуль пользователей, с регистрацией, авторизацией, активацией аккаунта через почту, и обычными страницами профиля.
- RBAC - простой модуль для создания ролей на сайте. Основано на описание ролей в файле.
- Сайт: основной модуль приложение. В нем хранится основной контроллер от которого унаследуются все остальные (FController). Плюс страница "Контактов", и "О нас"

Установка
---------
- Копируем репозиторий 
- Создаём новую БД 
- В файле @app/config/params.php настраиваем параметры соединения с БД 
- Если нужны демо материалы, импортируем в созданную БД дамп @app/data/yii2.sql
- Если демо материалы не нужны, применяем миграции:
~~~
cd yii2-blog
yii migrate
~~~
- Открываем в браузере http://localhost/yii2-blog/www/ и тестим!
