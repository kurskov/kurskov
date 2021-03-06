# Создание нового проекта Django
Рассматривается вариант создания проекта в PyCharm под Ubuntu.

## Создаем новый проект в PyCharm
В меню `File` выбираем пункт `New Project...`.
1. В поле `Location` вписываем название папки с новым проектом (это будет название репозитория на GitHub).
2. Вибираем окружение venv.
3. Выбираем интерпитатор Python.
4. Убираем галку создания main.py.
5. Жмем `Create`.

## Подключаем проект к GitHub
В меню `VCS` выбираем пункт `Share Project On GitHub`.
1. В поле `Repository name` подставиться название папки с нашим проектом.
2. В поле `Description` можно вписать что-то краткое описательное.
3. Жмем `Share`.
4. В появившемся окне жмем `Add`.

Теперь у нас есть пустой проект и пустой репозиторий.

## Устанавливаем Django

В терминале PyCharm прописываем:
```
python -m pip install Django
```
Проверяем установку:
```
python
```
```
import django
```
```
print(django.get_version())
```
Выходим обратно `Ctrl+D`.

## Создаем новый проект Django 
Название `projectname`; проект будет создан в текущем каталоге:
```
django-admin startproject projectname
```
Переходим в каталог с названием проекта (projectname) и проверяем работу сервера.
```
python manage.py runserver
```
Поумолчанию сервер использует порт 8000, 
но если он занят можно вручную ввести другой номер порта в команде, например:
```
python manage.py runserver 8001
```
При запуске сервера в терменале появиться ссылка, жмем ее и видим ракету.
Выходим обратно `Ctrl+C`.

## Создаем новое приложение Django
Создаем приложение name:
```
python manage.py startapp name
```
И творим, что хотим )))
