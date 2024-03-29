# Проект «kittygram_final»

## О проекте:
Проект kittygram_final позволяет пользователям выкладывать фото своих котиков с указанием его имени, даты рождения(год), цвета окраса и его достежения.

## Инструкция для развёртывания проекта:

### Первый вариант:

- Создать на боевом сервере пустой файл  docker-compose.production.yml
- С помощью редактора nano добавьте в него содержимое из локального docker-compose.production.yml 

### Второй вариант:
#### С помощью утилиты SCP скопировать файл между компьютерами:
- scp -i path_to_SSH/SSH_name docker-compose.production.yml \
    username@server_ip:/home/username/taski/docker-compose.production.yml

## Отличие docker-compose.yml от docker-compose.production.yml:
docker-compose.yml написан так, что образы билдятся при каждом запуске. Это удобно в процессе отладки, но в продакшене удобнее запускать контейнеры из готовых образов. Поэтому docker-compose.production.yml используеться на боевых серверах, а docker-compose.yml для отладки

## В проекте используются переменные окружения, чтобы использовать их ознакомтесь с файлом:
example.env

## Доступные endpiont:
### - Регистрация нового пользователя:
https://kittygramtdvwork.serveirc.com/signup

### - Вход в систему:
https://kittygramtdvwork.serveirc.com/signin

### - Главная страница:
https://kittygramtdvwork.serveirc.com/

### - Добавление нового котика:
https://kittygramtdvwork.serveirc.com/cats/add

## Использованные технологии:
- Язык програмирования - Python 3.9.10
- Фреймворк DRF
- СУБД - postgresql
- Docker

## Об авторах:
https://github.com/TDVwork696