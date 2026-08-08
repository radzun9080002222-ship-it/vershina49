# Вершина — премиальный клининг в Липецке

Лендинг. React + Vite + TypeScript + Tailwind CSS.

## Реклама

Полная конфигурация подготовленной, но не запущенной ЕПК Липецка хранится в [`advertising/YANDEX-DIRECT-LIPETSK-PRELAUNCH.md`](advertising/YANDEX-DIRECT-LIPETSK-PRELAUNCH.md).

## Концепция
Сайт продаёт не «услуги уборки», а уверенность: точная цена до приезда, прозрачный чек-лист 47 пунктов, гарантия 48 часов и отдельное направление для арендного и корпоративного жилья. Телефон, MAX, Telegram и WhatsApp общие с брендом «Вершина».

## Запуск
```bash
pnpm install
pnpm run dev      # разработка
pnpm run build    # сборка в dist/
```

## Где что лежит
- `src/data.ts` — ВЕСЬ контент: телефоны, WhatsApp, тарифы, ставки ₽/м², чек-листы, кейсы, FAQ
- `src/components/` — секции в порядке страницы (см. App.tsx)
- `public/images/` — изображения и отдельная social-card Липецка
- `source-assets/images/GPT/` — исходные GPT-генерации, не попадают в production build
## Публикация

- GitHub Pages собирается workflow из ветки `main`.
- Основной домен сайта — `https://vershina48.ru`; относительный `base` сохраняет корректную работу GitHub Pages и локальной сборки.
- Для Липецка используется отдельный счётчик Яндекс.Метрики `111309225` и отдельная верификация Яндекс Вебмастера; счётчики других городов намеренно не переносятся.
- Домен закреплён файлом `public/CNAME`; канонические URL, Open Graph, structured data, robots и sitemap используют `vershina48.ru`.
