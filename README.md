# Калькулятор зарплаты нетто — Израиль 2026

Онлайн-калькулятор для расчёта чистой зарплаты в Израиле. Подоходный налог, битуах леуми, битуах бриют, пенсия.

## Деплой на Render

### Вариант 1: Через GitHub (рекомендуется)

1. Создай репозиторий на GitHub и залей туда содержимое этой папки
2. Зайди на [render.com](https://render.com) → **New** → **Static Site**
3. Подключи GitHub-репозиторий
4. Настройки:
   - **Build Command:** `echo "Static site ready"`
   - **Publish Directory:** `./public`
5. Нажми **Create Static Site**

### Вариант 2: Через render.yaml (Blueprint)

1. Залей папку в GitHub
2. На Render → **New** → **Blueprint** → выбери репозиторий
3. Render автоматически прочитает `render.yaml` и задеплоит

### После деплоя

1. Скопируй URL, который выдал Render (например `https://israel-salary-calculator.onrender.com`)
2. Открой `public/index.html` и замени все вхождения:
   ```
   https://israel-salary-calculator.onrender.com
   ```
   на твой реальный URL
3. Закоммить и запушь — Render обновится автоматически

## Структура

```
render-site/
├── render.yaml              # Конфиг Render
├── README.md                # Этот файл
└── public/
    ├── index.html           # Калькулятор (всё в одном файле)
    └── og-image.png         # Картинка для соцсетей (1200×630)
```

## Что внутри

- **OG-теги** для Facebook, Telegram, WhatsApp, Twitter
- **Кнопки шаринга** (Telegram, Facebook, WhatsApp, копировать ссылку)
- **Favicon** — эмодзи калькулятора 🧮
- **Ссылка на канал** «ИИ что дальше?» в футере
- Полностью автономный — никаких внешних зависимостей

## Проверка OG-тегов

После деплоя проверь превью:
- Facebook: https://developers.facebook.com/tools/debug/
- Telegram: отправь ссылку боту @WebPageBot
- Twitter: https://cards-dev.twitter.com/validator
