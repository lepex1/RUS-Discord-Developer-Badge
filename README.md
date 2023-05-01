# Привет! Сегодня я расскажу как получить значок активного разработчика в дискорде
![Alt-Developer Badge](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcREt6DJ1OVMmDZCze67sft2tRlgaBSR1Ifyf97F8zxUqQ&s)

## Примечание! ГитХаб не может принимать больше 100 файлов. У меня их очень много. Я не стал их загружать в этот репозиторий повторно. Переходим по ссылке (https://github.com/toptipus/activedeveloper/archive/refs/heads/main.zip) и скачиваем все файлы отсюда.

### 1. Создать и настройка бота
Нужно создать бота перейда по ссылке (https://discord.com/developers/applications). Нажимаем "New Applications", пишем название и ставим галочку.
В столбце слева выбираем "Bot". Там ставим все слайдеры на ВКЛ кроме "REQUIRES OAUTH2 CODE GRANT" и ниже ставим галочку напротив "Administrator". В самом верху странички жмем "Reset token".  Далее нам нужно перейти в вкладку в столбце слева "OAuth2"-"URL Generator". Среди кнопок с галочками ищем "bot" и тыкаем чтобы поставить галочку. Еще ниже в окошке "SELECT REDIRECT URL" выбираем. Ниже выбираем "Administrator". Далее генерируем ссылку на бота. Переходим по ссылке и добавляем бота на ваш приватный дискорд сервер.


### 2. Config.json
Копируем токен и идем в файл "config.json"

```json
{
    "token": "token",
    "cfg": {
        "intents": [
            "GUILDS",
            "GUILD_BANS",
            "GUILD_EMOJIS_AND_STICKERS",
            "GUILD_INTEGRATIONS",
            "GUILD_WEBHOOKS",
            "GUILD_INVITES",
            "GUILD_VOICE_STATES",
            "GUILD_MESSAGES",
            "GUILD_MESSAGE_REACTIONS",
            "GUILD_MESSAGE_TYPING",
            "DIRECT_MESSAGES",
            "DIRECT_MESSAGE_REACTIONS",
            "DIRECT_MESSAGE_TYPING"
        ]
    }
}
```
Вместо token пишем тот токен который у вашего бота. Помните что этот токен никому нельзя давать т.к. с помощью токена можно будет управлять вашим ботом.

### 3. Установка NodeJS
Без установки NodeJS у вас ничего не получится. Переходим по ссылке (https://nodejs.org/en/download) и скачиваем установщик. Запускаем его. Во время установки просто нажимайте далее. **Не меняйте путь установки!**
![Alt-NodeJS](https://i.imgur.com/tdC3MGf.png)

### 4. Подготовка сервера
Переходим в настройки вашего дискорд сервера. Находим там вкладку "создать сообщество". Создаем
![Alt-Server](https://i.imgur.com/SV8Ezsj.png)

### 5. Запуск бота
Чтобы бот начал работать надо запустить файл "start_bot.bat". В консоли у вас должно быть написано "НазваниеВашегоБота READY". 
![Alt-start bot](https://i.imgur.com/JcxGRaM.png)

Переходим в чат вашего сервера и пишем команду "/ping". Бот вам ответит "pong".

![Alt-start bot](https://i.imgur.com/vI54904.png)

### 6. Получение значка
Чтобы получить значок вам надо перейти по ссылке (https://discord.com/developers/active-developer) и нажать кнопку по середине. Процесс получения занимает от 24 часов
![Alt-start bot](https://i.imgur.com/BBroFT0.png)
