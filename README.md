# Nuxt 3 Minimal Starter

Для начала работы с проектом вам понадобятся несколько вещей:

1. **Node.js**: Убедитесь, что у вас установлена актуальная версия Node.js. Можно скачать [отсюда](https://nodejs.org/en/download/current).
   
2. **Редактор кода**: Если у вас еще нет редактора кода, рекомендуем использовать бесплатный редактор [VSCode](https://code.visualstudio.com/download).

3. Откройте в редакторе кода терминал, предварительно открыв папку с проектом и выполните следующую команду для установки зависимостей:

```bash
# npm
npm install
```

## Запуск локального сервера

После установки зависимостей можно запустить локальный сервер. Проект будет доступен по адресу `http://localhost:3000`:

```bash
# npm
npm run dev
```

## Компиляция проекта

При подготовке проекта к развертыванию на сервере вам понадобится скомпилировать его. Вот как это сделать:

- **Сборка для VDS**:

```bash
# npm
npm run build
```

- **Сборка для VPS** (если не уверены, какой сервер используете):

```bash
# npm
npm run generate
```

## Структура проекта

- **assets/**
  - **styles/**
    - `_variables.scss`: Файл со стилями и переменными, используемыми в проекте (сейчас тут только цвета).
    - `index.scss`: Основной файл стилей проекта.
  - **svg/**: Директория для SVG файлов, используемых в проекте.
  
- **components/**
  - **Layout/**
    - `footer.vue`: Компонент для футера сайта **(тут нужно добавить ссылки для соцсетей)**.
    >`NuxtLink href="/#" target="_blank"...` - внутрь кавычек, вместо "/#" добавляем ссылки.
    - `header.vue`: Компонент для шапки сайта **(тут нужно добавить ссылки для соцсетей)**.
    >`{ url: '/#', icon: '/ico/Instagram.png', alt: 'Instagram ico' },"...` - внутрь кавычек, вместо "/#" добавляем ссылки.
  - **main/**
    - **index/**
      - `index.vue`: Главная страница сайта.
      - `advantages.vue`: Компонент с преимуществами компании.
    - **about/**
      - `index.vue`: Страница "О нас".
      - `Info.vue`: Компонент с информацией о компании.
      - `Pogruzka.vue`: Компонент для блока о погрузке.
      - `Cart.vue`: Компонент для Pogruzka.vue, в котором текст.
      - `Work.vue`: Компонент с информацией о работе компании.
    - **form/**
      - `index.vue`: Страница с формой обратной связи.
      - `Modal.vue`: Модальное окно для формы.
      - `RequestForm.vue`: Компонент самой формы.
  - **UI/**
    - `Button.vue`: Компонент для кнопок.
    - `logo.vue`: Компонент с логотипом.
    
- **config/**
  - `config.js`: Файл с данными для формы **(тут нужно добавить id чата и id бота телеграма)**.
  >Инструкция по созданию бота и получения чат id телеграма - [ссылка](https://docs.moontrader.com/ru/telegram-personal).
  
- **layouts/**
  - `default.vue`: Основной шаблон страниц сайта.
  
- **pages/**
  - `index.vue`: Главная страница сайта.
  
- **public/**
  - **ico/**
    - *Директория для иконок.*
  - **img/**
    - *Директория для изображений.*
  - `favicon.ico`: Иконка, отображаемая во вкладке браузера.
  
- `nuxt.config.ts`: Файл конфигурации Nuxt.js.

- `package.json`: Файл с описанием зависимостей и скриптов проекта.

Теперь вы готовы к работе с вашим проектом на Nuxt 3!