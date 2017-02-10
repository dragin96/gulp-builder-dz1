# IGOSHEVA| Сборка проекта с помощью Gulp версии 4.0.

> Автор: Игошева Анастасия
> Основано на сборке онлайн-школы LoftSchool

## Старт проект

1. Склонируйте репозиторий и перейдите в папку проекта
```
git clone git@github.com:igosheva/gulp-builder-dz1.git
```

2. Установите модуль gulp-cli глобально
```
npm i gulp-cli -g
```

3. Установите модули локально
```
npm i
```

4. Запустите сборку проекта
```
gulp
```

## Структура папок и файлов
```
├── build/                     # Сборка (автогенерация)
│   ├── assets/                # Подключаемые ресурсы
│       └── css/               # Стили
│           └── app.css        # Главные стили
│           └── foundation.css # Стили normalize.css
│       ├── img/               # Изображения
│           └── block.png      # Картинка в png
│           └── block.jpg      # Картинка в jpg
│       ├── js/                # Скрипты
│           └── app.js         # Главные скрипты
│           └── foundation.js  # Скрипты normalize.js
│    └── index.html            # Страница
├── gulp/                      # Модули для функционирования gulpfile.js
│   ├── paths/                 # Пути для сборки проекта
│       ├── app.js             # Путь для js-файлов
│       ├── css.foundation.js  # Путь до стилей в npm
│       ├── js.foundation.js   # Путь до скриптов в npm
│       ├── tasks.js           # Пути до задач для gulpfile.js
│   ├── tasks/                 # Задачи для gulpfile.js
│       ├── clean.js           # Очистка
│       ├── copy.image.js      # Копирование картинок
│       ├── css.foundation.js  # Подключение стилей для foundation.js
│       ├── js.foundation.js   # Подключние скриптов для foundation.js
│       ├── js.lint.js         # Подключние линтов
│       ├── js.process.js      # Оптимизация скриптов
│       ├── pug.js             # Сборка страниц из Pug шаблонов
│       ├── sass.js            # Сборка и оптимизация стилей
│       ├── serve.js           # Запуск локального сервера
│       ├── sprite.svg.js      # Сборка спрайтов SVG
│       ├── watch.js           # Отслеживание изменений и запуск задач
│   ├── config/                # Файл с доп.настройками
├── source/                    # Исходники
│   ├── images/                # Папка картинок
│       └── block.png          # Картинка в png
│       └── block.jpg          # Картинка в jpg
│   ├── js/                    # Скрипты
│       └── app.js             # Главный скрипт
│   └── styles/                # Стили
│       ├── common/            # Помощники
│           ├── style.scss     # Стили для одной страницы
│       └── app.scss           # Главный стилевой файл
│   ├── template/              # Блоки
│       └── common/            # Компоненты страниц
│           ├── block.pug      # Разметка компонента
│       └── pages/             # Страницы
│           ├── block.pug      # Разметка страниц
│       └── block.pug          # Основной файл страниц
├── .eslintrc                  # Конфигурация проверки JavaScript в ESLint
├── .gitignore                 # Список исключённых файлов из Git
├── gulpfile.js                # Файл для запуска Gulp.js
├── package.json               # Список модулей и прочей информации
├── README.md                  # Документация шаблона
```
