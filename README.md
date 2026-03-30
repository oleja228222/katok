# katok
Установите зависимости
composer install
npm install

Настройте окружение
cp .env.example .env
php artisan key:generate

Настройте базу данных
В файле .env:
DB_CONNECTION=sqlite
# Создайте файл database/database.sqlite

Выполните миграции и сидеры
php artisan migrate:fresh --seed

Настройте ЮKassa
В файле .env укажите тестовые данные:
YOOKASSA_SHOP_ID=ваш_shop_id
YOOKASSA_SECRET_KEY=ваш_secret_key

Соберите ассеты
npm run build

Запустите сервер
php artisan serve

Доступы
Админ-панель
URL: /admin/login
Email: admin@ice-rink.ru
Пароль: admin123
