# Frontend starter template

## Технологии

```bash
- BEM
- Webpack
- Pug
- Scss
- JavaScript
- Lints
```

## Команды

```bash
npm i                  # Установка всех необходимых зависимостей
npm start              # Запуск проекта для разработки с сервером
npm run build          # Сборка проекта для prod
npm run dev            # Сборка проекта для разработки
```

## BEM

1. БЭМ-именование: `__` — разделитель элемента, `--` — разделитель модификатора.
2. Для каждого блока создается отдельный файл стилей.
3. Очередность селекторов:
   - Стилевые правила сущности.
   - Медиа условия.
   - Псевдоселекторы и псевдоэлементы.
   - Сторонние вложенные селекторы.
   - Элементы блока.
   - Модификаторы блока.

## Разметка

Все файлы располагаются в `dev/layout/`. Для каждого компонента или блока создается отдельный файл.

- `dev/layout/content/` - контент страниц.
- `dev/layout/page/` - начальная разметка страниц.
- `dev/layout/sections/` - блоки контента секций.
- `dev/layout/modules/` - header, footer.
- `dev/layout/*.pug` - главные файлы, куда включается основная часть с папки `page/` (переменные, контент, скрипты).

## Стили

Все стили располагаются в `src/styles/`. Для каждого компонента или блока создается отдельный файл.
Для использования другого препроцессора переименуйте все файлы в `dev/styles/` в нужное расширение.

- `src/styles/helpers/` - переменные и миксины.
- `src/styles/base/` - базовые стили и шрифты.
- `src/styles/sections/` - стили секций.
- `src/styles/components/` - отдельные встраиваемые компоненты, виджеты и т.п.
- `src/styles/modules/` - блоки, такие как header, footer.
- `src/styles/libs/` - стили установленных библеотек.
- `src/styles/media/` - стили для адаптивных сайтов (desktop first).
- `src/styles/styles.scss` - главный стилевой файл, в который импортируются все компоненты.

## Скрипты

`src/js/` - файлы со скриптами.

## Git

`.gitignore` - указаны папки и файлы, которые будут игнорироваться.

## EditorConfig

Для корректной работы нужно установить плагин для вашего редактора или IDE.
Список редакторов и IDE для которых нужно установить плагин [EditorConfig](https://editorconfig.org/#download)
Список редакторов и IDE для которых плагин не нужен [EditorConfig](https://editorconfig.org/#pre-installed)

## Линтинг

Для проверки кода на ошибки и соответствие код-гайдам.

`.stylelintrc` - конфиг для проверки (`less, scss, sass`) [stylelint](https://stylelint.io/).

## Webpack

- Файл `webpack.config.js`:
   - Конфигурационный файл `webpack`
