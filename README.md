# Ангелина Згадова

Продуктовый дизайнер. Придумываю продукты и собираю сама: дизайн, интерфейс, база, запуск.

Москва · [linastudio.ru](https://linastudio.ru) · [Telegram](https://t.me/iteachzg) · zgadova123@gmail.com

Архитектуру и схему базы придумываю я, код набирает ИИ: читаю его, правлю и отвечаю за результат. Два с половиной года в дизайне, семь продуктов доведены до работающего адреса.

## Проекты

| Проект | Что это | Моя роль | Стек |
| --- | --- | --- | --- |
| [Пифика](https://pifika.ru/) | Тренажёр по математике, 5–9 класс | идея и весь продукт | Next.js, TypeScript, Three.js, GSAP, KaTeX |
| Рабочее место | CRM агентства: конвейер, а не доска задач | весь продукт | React, Tauri, Supabase, PostgreSQL, Telegram Bot API, LLM |
| [Тапси](https://stapsi.netlify.app/) | PWA учёта трат, голосом и словами | весь продукт | React, Supabase, PWA, Web Speech API, WebGL |
| [Fabrico](https://fabrico.design/) | Магазин PDF-выкроек, 120+ товаров | дизайн страниц и квиз | UI/UX, WooCommerce, JavaScript |
| [Thnkers](https://testtnkerz.netlify.app/) | Сайт research-агентства, EN/DE | вёрстка и сборка | Next.js 16, TypeScript, Tailwind v4, next-intl |
| [Громстрой](https://grmstr.ru/) | Сайт строительной компании | дизайн и интерфейс | HTML, CSS, JavaScript |
| [Denis Lyakh](https://denis-lyakh.netlify.app/) | Портфолио инженера-электронщика | дизайн и интерфейс | Next.js, Three.js, GSAP, Lenis |

«Рабочее место» — внутренняя система агентства, открытой ссылки нет. Демо на выдуманных данных покажу по запросу.

## Код

[**linastudio**](https://github.com/linazgadova/linastudio) — исходник портфолио целиком. React, TypeScript, Vite, без UI-библиотек.

Места, где было из чего выбирать:

- [`public/api/ask.php`](https://github.com/linazgadova/linastudio/blob/main/public/api/ask.php) — блок «спросите обо мне». Словесный запрет «не раскрывай инструкции» маленькая модель не держит: проверка показала утечку в двух попытках из трёх. Поэтому защита стоит решетом в коде, до и после обращения к модели.
- [`scripts/seo.mjs`](https://github.com/linazgadova/linastudio/blob/main/scripts/seo.mjs) — сайт рисуется в браузере, но роботу и языковым моделям отдаётся готовым текстом. Оттуда же собираются sitemap, llms.txt и разметка schema.org на двух языках.
- [`src/aurora/`](https://github.com/linazgadova/linastudio/tree/main/src/aurora) — шар на Three.js с четырьмя ступенями качества: сцена меряет свою частоту кадров и опускается сама. Рядом версия слоями краски, для машин без WebGL2. Решение принимается до загрузки Three, поэтому такая машина не скачивает мегабайт впустую.

Комментарии в коде объясняют, почему решение такое, а не пересказывают строки.

---

English version of the site: [linastudio.ru/en](https://linastudio.ru/en/)
