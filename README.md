# yamdb_final

![example workflow](https://github.com/forester2k/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)

### О проекте

Данный проект является учебным.
Проект YaMDb собирает отзывы (Review) пользователей на произведения (Titles). Произведения делятся на категории (Category): «Книги», «Фильмы», «Музыка».
Сами произведения в YaMDb не хранятся.
Произведению может быть присвоен жанр (Genre).
Пользователи YaMDb оставляют к произведениям текстовые отзывы (Review) и ставят произведению оценку в диапазоне от одного до десяти (целое число); из пользовательских оценок формируется усреднённая оценка произведения — рейтинг (целое число).

### Как запустить проект.

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/forester2k/api_yamdb.git
```

```
cd api_yamdb
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


### Как делать запросы:

К проекту по адресу .../redoc/ подключена документация redoc, содержащая сведения по доступным эндпоинтам и примеры запросов.


### Импорт внешних данных в проект:

При необходимости импортировать внешние данные, в проекте реализована команда csv_sql для  заполнения таблиц БД из .csv файлов. Синтаксис команды:

```
python manage.py csv_sql <файл .csv> <название модели>
```



### Под руководством команды Яндекс-Практикума над проектом работали:

- Васильев Кирилл - Разработчик
- Ежов Михаил - Разработчик
- Сосновский Александр - Разработчик
- Тихонов Станислав - Разработчик / Тимлид

 
 
