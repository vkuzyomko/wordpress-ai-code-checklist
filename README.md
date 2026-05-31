# wordpress-ai-code-checklist
Checklist for checking WordPress plugins and AI-generated PHP code.

# WordPress AI Code Checklist

Чек-лист для проверки WordPress-плагинов и PHP-кода, написанного через ChatGPT, Cursor или другие AI-инструменты.

Полезные материалы:

- [Доработка проекта после вайб-кодинга](https://sites-creator.com.ua/dorabotka-proekta-posle-vibe-coding/)
- [Разработка WordPress-плагинов под заказ](https://sites-creator.com.ua/razrabotka-wordpress-plaginov-pod-zakaz/)
- [Техническая поддержка WordPress](https://sites-creator.com.ua/tehnicheskaya-podderzhka-wordpress/)


## Что проверять в AI-сгенерированном WordPress-коде

### 1. Безопасность
- Есть ли nonce в AJAX-запросах
- Проверяются ли права пользователя
- Защищены ли SQL-запросы через prepare
- Экранируется ли вывод через esc_html, esc_attr, esc_url
- Нет ли прямого доступа к PHP-файлам

### 2. WordPress-логика
- Используются ли хуки WordPress
- Не ломается ли админка
- Не конфликтует ли код с темой или плагинами
- Работает ли код после обновления WordPress

### 3. AJAX и формы
- Правильно ли указан admin-ajax.php
- Есть ли обработчик для авторизованных и неавторизованных пользователей
- Возвращается ли wp_send_json_success или wp_send_json_error
- Проверяется ли ошибка на стороне frontend

### 4. База данных
- Нет ли прямой вставки данных в SQL
- Проверяются ли входные данные
- Есть ли индексы в таблицах
- Не создаются ли дубли записей

### 5. Поддержка проекта
- Можно ли понять структуру кода
- Есть ли понятные названия функций
- Нет ли повторов одного и того же кода
- Можно ли безопасно доработать проект дальше
