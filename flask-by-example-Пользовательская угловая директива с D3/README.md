# Flask на примере

## Сообщения в блоге

Это репо для серии блогов Real Python, Flask by Example -

1. [Часть первая] (https://realpython.com/blog/python/flask-by-example-part-1-project-setup/): настройте локальную среду разработки, а затем разверните как промежуточную, так и производственную среда на Heroku.
1. [Часть вторая] (https://realpython.com/blog/python/flask-by-example-part-2-postgres-sqlalchemy-and-alembic): настройте базу данных PostgreSQL вместе с SQLAlchemy и Alembic для обработки миграции.
1. [Часть третья] (https://realpython.com/blog/python/flask-by-example-part-3-text-processing-with-requests-beautifulsoup-nltk/): добавьте внутреннюю логику для очистки и последующей обработки количества слов с веб-страницы с помощью библиотек запросов, BeautifulSoup и Natural Language Toolkit (NLTK).
1. [Часть четвертая] (https://realpython.com/blog/python/flask-by-example-implementing-a-redis-task-queue/): Реализуйте очередь задач Redis для обработки текста.
1. [Часть пятая] (https://realpython.com/blog/python/flask-by-example-integrating-flask-and-angularjs/): настройте Angular во внешнем интерфейсе для непрерывного опроса серверной части. чтобы узнать, завершена ли обработка запроса.
1. [Часть шестая] (https://realpython.com/blog/python/updating-the-staging-environment/): отправка на промежуточный сервер на Heroku - настройка Redis и подробное описание того, как запускать два процесса (веб-интерфейс и рабочий) на одном динамометрическом стенде.
1. [Часть седьмая] (https://realpython.com/blog/python/flask-by-example-updating-the-ui/): обновите интерфейс, чтобы сделать его более удобным для пользователя.
1. Часть восьмая: добавьте в микс библиотеку D3, чтобы построить график частотного распределения и гистограммы.

Посетите http://realpython.com

## Быстрый старт

### Первые шаги

```sh
$ pyvenv-3.5 env
$ source env/bin/activate
$ pip install -r requirements.txt
```

### Настроить миграцию

```sh
$ python manage.py db init
$ python manage.py db migrate
$ python manage.py db upgrade
```

### Запустить

Запускайте каждый в другом окне терминала ...

```sh
# redis
$ redis server

# рабочий процесс
$ python worker.py

# приложение
$ python app.py
```