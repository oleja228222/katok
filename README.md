# Сайт ледового катка с бронированием коньков

## Установка

1. **Установите зависимости**
```bash
composer install
npm install
```

2. **Настройте окружение**
```bash
cp .env.example .env
php artisan key:generate
```

3. **Настройте базу данных**

В файле `.env`:
```
DB_CONNECTION=sqlite
# Создайте файл database/database.sqlite
```

4. **Выполните миграции и сидеры**
```bash
php artisan migrate:fresh --seed
```

5. **Настройте ЮKassa**

В файле `.env` укажите тестовые данные:
```
YOOKASSA_SHOP_ID=ваш_shop_id
YOOKASSA_SECRET_KEY=ваш_secret_key
```

6. **Соберите ассеты**
```bash
npm run build
```

7. **Запустите сервер**
```bash
php artisan serve
```

## Доступы

### Админ-панель
- **URL:** `/admin/login`
- **Email:** admin@ice-rink.ru
- **Пароль:** admin123