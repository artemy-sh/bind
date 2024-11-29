# Bitrix in Docker

Минимальный набор для быстрого запуска окружения Bitrix в контейнерах Docker.

- **Docker** и **Docker Compose** — для работы с контейнерами.
- **PHP 8.4-fpm** — для работы серверной части Bitrix.
- **Nginx** — для обработки веб-запросов.
- **MySQL** — для хранения данных.
- **PHPMyAdmin** — для управления базой данных через веб-интерфейс.

## Быстрый старт
1. **Клонируйте репозиторий:**
   ```bash
   git clone https://github.com/artemy-sh/bind
   cd bitrix-docker
   ```

2. **Скопируйте пример конфигурации:**
   ```bash
   cp .env.example .env
   ```

3. **Соберите и запустите контейнеры:**
   ```bash
   docker-compose up --build
   ```

4. **Откройте проект в браузере:**
   Перейдите по адресу `http://localhost`
   
5. **Установите или восстановите Bitrix:**
   - Для новой установки откройте `http://localhost/bitrixsetup.php`.
   - Для восстановления проекта откройте `http://localhost/restore.php`.

## Настройки
Все основные настройки:
- `.env` — основные параметры.
- `nginx.conf` — конфигурация Nginx.
- `mysql.cnf` — параметры MySQL.
- `php.ini` — настройки PHP.
- `mime.types` — MIME-типы для обработки запросов.

## Лицензия
Проект распространяется под лицензией [MIT](LICENSE).

## Контакты
Если у вас есть вопросы или предложения, пишите на:  
**artemy.sh@gmail.com**