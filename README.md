# Luna Character Sheet

Отдельный статический сайт листа персонажа. Старый проект не используется и не изменяется.

## Структура

- `outputs/character-sheet.html` - сам лист персонажа.
- `netlify.toml` - Netlify публикует папку `outputs` и открывает лист с корня сайта.

## Деплой на новый GitHub/Netlify

1. Репозиторий: `https://github.com/StormKat/Luna`.
2. Залей туда содержимое папки `luna-character-sheet`.
3. В Netlify: **Add new project -> Import an existing project**.
4. Выбери новый репозиторий.
5. Netlify сам прочитает `netlify.toml`.
6. Publish directory должен быть `outputs`.

Портрет сейчас сохраняется локально в браузере через `localStorage`, без облачной синхронизации.
