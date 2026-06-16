# 🔧 Настройка переменных (config.ini)

Скопируй `config_example.ini` → `config.ini` и заполни вручную:

```ini
[telegram]
token = "СЮДА_ТОКЕН_БОТА"
user_id = "СЮДА_ТВОЙ_TELEGRAM_ID"

[timezone]
name = "Europe/Moscow"

[settings]
language = "ru"
```

## Где взять значения

| Переменная | Что это | Как получить |
|---|---|---|
| `token` | Токен Telegram-бота | [@BotFather](https://t.me/botfather) → `/newbot` → скопировать токен |
| `user_id` | Твой Telegram ID (число) | Напиши [@userinfobot](https://t.me/userinfobot) — он пришлёт ID |
| `name` | Часовой пояс | Формат `Region/City`, например `Europe/Moscow`, `Asia/Almaty` — [список](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) |
| `language` | Язык уведомлений | `ru` или `en` |

> ⚠️ `config.ini` добавлен в `.gitignore` — он **никогда не попадёт на GitHub**. Храни токен только локально.

## Запуск

```bash
pip install -r requirements.txt
python main.py
```
