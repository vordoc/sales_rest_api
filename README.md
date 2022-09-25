# «API Сервис заказа товаров для розничных сетей»

## Описание

Приложение предназначено для автоматизации закупок в розничной сети. Пользователи сервиса — покупатель (менеджер торговой сети, который закупает товары для продажи в магазине) и поставщик товаров.

**Клиент (покупатель):**

- Менеджер закупок через API делает ежедневные закупки по каталогу, в котором
  представлены товары от нескольких поставщиков.
- В одном заказе можно указать товары от разных поставщиков — это
  повлияет на стоимость доставки.
- Пользователь может авторизироваться, регистрироваться и восстанавливать пароль через API.
    
**Поставщик:**

- Через API информирует сервис об обновлении прайса.
- Может включать и отключать прием заказов.
- Может получать список оформленных заказов (с товарами из его прайса).



В проекте задействованы такие технологии как:
* Python 3
* Django
* Django Rest Framework

## Установка

Клонируйте этот репозиторий

    git clone https://github.com/Varyag-Ingvar/sales_rest_api.git

Создайте и активировуйте виртуальное окружение

Установите зависимости из файла **requirements.txt**:
```bash
pip install -r requirements.txt
```
### В файле settings.py установите настройки базы данных PostgreSQL, либо используйте настройки по умолчанию (sqlite3).
# Выполните следующие команды:

* Команда для создания миграций приложения для базы данных
```bash
python manage.py makemigrations
python manage.py migrate
```

* Запустите приложение
```bash
python manage.py runserver
```
### Используйте любой REST Client для отправки запросов (напр.расширение REST Client для VisualStudioCode)
    
