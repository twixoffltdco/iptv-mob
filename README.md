# IPTV Player — быстрый мобильный плеер

Простой и шустрый IPTV-плеер для просмотра каналов из M3U-плейлистов.  
Оптимизирован для **мобильных устройств** (Android/iOS), не тормозит, кнопки отзываются мгновенно.  
Использует мощный плеер [PlayerJS](https://playerjs.com/) и HLS.js для потоков.



## Возможности

- 📺 Поддержка нескольких M3U-плейлистов (переключение кнопками в шапке)
- 🔍 Поиск по названиям каналов и группам
- 📱 Адаптивный интерфейс: на мобилках выезжающий сайдбар с каналами
- 🧩 **Embed-код** для вставки плеера на другой сайт (с текущим каналом)
- 🔗 Копирование прямой ссылки на поток
- 🖥️ Полноэкранный режим
- ⚡ Максимальная производительность: минимум CSS-эффектов, быстрый рендер списка, без лишних перерисовок

## Используемые технологии

- HTML5/CSS3/JS (vanilla)
- [HLS.js](https://github.com/video-dev/hls.js) — для HLS-потоков
- [PlayerJS](https://playerjs.com/) — универсальный HTML5-плеер

## Плейлисты (предустановлены)

| Кнопка в интерфейсе | Ссылка на M3U |
|---------------------|---------------|
| LIVEM3U | `https://secure-272717.tatnet.app/livem3u.tatnet.app/data/playlist.m3u` |
| WINK Zabava | `https://secure-272717.tatnet.app/livem3u.tatnet.app/zabava-full.m3u` |
| WINK Off. | `https://raw.githubusercontent.com/CrocoUser/zabava-project/refs/heads/main/zabava-full.m3u` |
| Мультики ССР | `https://secure-272717.tatnet.app/iptvplay.tatnet.app/iptvlist.ru-mult (1).m3u` |
| Мульт Off. | `https://secure-272717.tatnet.app/iptvplay.tatnet.app/iptvlist.ru-kids (1).m3u` |
| Russia TV | `https://secure-272717.tatnet.app/livem3u.tatnet.app/russ.m3u` |
| Russia Off. | `https://secure-272717.tatnet.app/livetv.tatnet.app/russ.m3u` |

> Легко добавить свои: отредактируй объект `PLAYLISTS` в коде.

## Установка и запуск

1. Скачай все файлы: `index.html`, `playerjs.js` (скачай с [официального сайта](https://playerjs.com/) или используй CDN).
2. Помести их в одну папку на сервере (или локально).
3. Открой `index.html` в браузере (для полной работы нужно локальный сервер, например, `npx serve .`).

Или просто залей на GitHub Pages / любой хостинг.

## Структура файлов
├── index.html # главный плеер
├── playerjs.js # библиотека плеера (обязательна)
└── README.md

text

## Важно

- Если используешь **embed-функцию** — нужен файл `embed.html` на сервере. Его можно создать отдельно или просто скопировать этот же `index.html` под другим именем, предварительно убрав лишние элементы. Но в текущей версии embed генерирует код с ссылкой на `embed.html` — доработай под свои нужды.
- Для работы HLS-потоков необходима поддержка HLS.js или нативного HLS в Safari.

## Благодарности

- [PlayerJS](https://playerjs.com/) за отличный плеер
- [HLS.js](https://github.com/video-dev/hls.js) за воспроизведение HLS

## Лицензия

MIT — делай что хочешь.

---

**Приятного просмотра!** 📡
