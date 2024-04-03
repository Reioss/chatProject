
### Зависимостей
```bash
pip install -r requirements.txt
```

### Файл .env.sample необходимо переименовать в .env и скопировать в него следующее:

```bash
DEBUG=True
SECRET_KEY='generated secret key'

EMAIL_HOST='host'
EMAIL_HOST_USER='user'
EMAIL_HOST_PASSWORD='password'
EMAIL_PORT=25

REDIS_HOST='localhost'
REDIS_PORT=6379
```

### Запуск 

```bash
./manage.py runserver
```

### Для проверки работоспособности есть тестовых аккаунта:
```bash
chat_user1@gmail.com / 123qweasdzxc123
chat_user2@gmail.com / 123qweasdzxc123
```

### Функционал:
```bash
http://127.0.0.1:8000/ - Поиск или создание новой группы для общения 
http://127.0.0.1:8000/swagger-ui/ - Доступный API 
http://127.0.0.1:8000/users/ - Доступные пользователи
http://127.0.0.1:8000/rooms/ - Доступные группы
http://127.0.0.1:8000/user/profile/ - Профиль пользователя
```
### !!!
```bash
Функционал websocket'ов 
реализован с помощью django-channels.  
```