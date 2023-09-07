### О чём проект:

В этом проекте выполнен автоматизированный деплой действующего сайта-одностраничника "KITTIGRAM": приложения, в котором пользователи могут поделиться фотографиями и достижениями своих кошек.

(ссылка на проект[https://kittygram-sk.hopto.org/])
  

### Как развернуть проект локально:

- Склонируйте проект с GitHub с помощью команды
```
git clone git@github.com:SergeiKrm/infra_sprint1.git
```

- Откройте папку с проектом на локальном компьютере

- Разверните и активируйте виртуальное окружение командами
```
python -m venv venv
source venv/bin/activate
```

- Из папки, содержащей файл requirements.txt, при активированном виртуальном окружении выполните команду 
```
pip install -r requirements.txt
``` 
- Выполните миграции 
```
python manage.py migrate 
```
- Запустить проект:
```
python3 manage.py runserver
```


### Как развернуть проект на сервере:

- Установите Docker + Docker Compose
- Клонируйте репозиторий
- Запустите все контейнеры командой
```
docker compose -f docker-compose.production.yml up
```
- Перейдите на страницу https://kittygram-sk.hopto.org/


Используемые переменные окружения c указанием требуемого формата перечислены в файле ".env.example".

В приложении использовались технологии JavaScript, Python/Django.

Автор Kramarev Sergei
