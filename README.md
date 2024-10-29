# Проект Neva Tickets

## Установка
Для успешного развертывания проекта выполните следующие шаги:

1. **Клонирование репозитория:**

   ```bash
   git clone https://github.com/MrAbayDev/A_Tickets.git
   cd <папка_проекта>
2. **Создание .env файла Скопируйте содержимое файла .env.example в .env и отредактируйте его для настройки подключения к базе данных:**

    ```bash
    cp .env.example .env
3. **Установка зависимостей Docker Убедитесь, что у вас установлен Docker. Выполните команду:**
    
   ```bash
    docker compose up --build
   
4. **После запуска Docker вы запускаете эту команду в контейнере Docker. Если вы не выполните миграцию, программа не будет работать и вернет ошибку.**
    ```bash
   php artisan migrate
   
5. **Наконец, обновите контейнер этой командой, и все будет работать нормально.**
    ```bash
   php artisan optimize
