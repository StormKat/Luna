# Luna Character Sheet

Отдельный статический сайт листа персонажа. Старый проект не используется и не изменяется.

## Структура

- `outputs/character-sheet.html` - сам лист персонажа.
- `netlify/functions/` - загрузка и чтение портрета через Netlify Blobs.
- `netlify.toml` - Netlify публикует папку `outputs` и открывает лист с корня сайта.

## Деплой на новый GitHub/Netlify

1. Репозиторий: `https://github.com/StormKat/Luna`.
2. Залей туда содержимое папки `luna-character-sheet`.
3. В Netlify: **Add new project -> Import an existing project**.
4. Выбери новый репозиторий.
5. Netlify сам прочитает `netlify.toml`.
6. Publish directory должен быть `outputs`.
7. В **Site configuration -> Environment variables** добавь:
   - Key: `PORTRAIT_UPLOAD_TOKEN`
   - Value: пароль для загрузки портрета
8. Сделай новый deploy.

Портрет сохраняется в Netlify Blobs. Локальная копия в браузере используется только как запасной вариант.
