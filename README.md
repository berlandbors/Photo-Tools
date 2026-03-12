# 📸 Photo Tools

Коллекция отдельных инструментов для манипуляций с фотографиями. Каждый инструмент — самодостаточный HTML-файл со встроенными CSS и JavaScript. Никаких зависимостей, всё работает прямо в браузере.

## 🚀 Демо

Откройте `index.html` в любом современном браузере — установка не требуется.

## 🛠 Инструменты

### Простые

| # | Инструмент | Описание | Технология |
|---|-----------|----------|------------|
| 01 | [Яркость](tools/01-brightness/index.html) | Регулировка яркости от −100 до +100 | `filter: brightness()` |
| 02 | [Контраст](tools/02-contrast/index.html) | Регулировка контраста от 0 до 200 | `filter: contrast()` |
| 03 | [Черно-белое](tools/03-grayscale/index.html) | Преобразование в оттенки серого | `filter: grayscale()` |
| 04 | [Сепия](tools/04-sepia/index.html) | Ретро-эффект сепии | `filter: sepia()` |
| 05 | [Инверсия цветов](tools/05-invert/index.html) | Эффект «негатива» | `filter: invert()` |
| 06 | [Поворот](tools/06-rotate/index.html) | Поворот на 90°/180°/270° или произвольный угол | `ctx.rotate()` |
| 07 | [Отражение](tools/07-flip/index.html) | Горизонтальное и вертикальное отражение | `ctx.scale()` |

### Средние

| # | Инструмент | Описание | Технология |
|---|-----------|----------|------------|
| 08 | [Размытие](tools/08-blur/index.html) | Размытие по Гауссу (0-20px) | `filter: blur()` |
| 09 | [Резкость](tools/09-sharpen/index.html) | Повышение чёткости изображения | Convolution matrix |
| 10 | [Кадрирование](tools/10-crop/index.html) | Интерактивная обрезка изображения | Mouse events + Canvas |
| 11 | [Изменение размера](tools/11-resize/index.html) | Масштабирование с сохранением пропорций | `drawImage()` |
| 12 | [Насыщенность](tools/12-saturation/index.html) | Регулировка насыщенности цветов (0-200%) | `filter: saturate()` |
| 13 | [Оттенок](tools/13-hue/index.html) | Сдвиг цветового тона (0-360°) | `filter: hue-rotate()` |

### Сложные

| # | Инструмент | Описание | Технология |
|---|-----------|----------|------------|
| 14 | [Instagram-фильтры](tools/14-instagram-filters/index.html) | 10 готовых фильтров в стиле Instagram | Комбинации CSS filters |
| 15 | [Виньетка](tools/15-vignette/index.html) | Затемнение/осветление по краям | Radial gradient |
| 16 | [Рисование](tools/16-draw-annotate/index.html) | Кисть, текст, фигуры, аннотации | Mouse events + Canvas |
| 17 | [Удаление фона](tools/17-background-removal/index.html) | Удаление фона по цвету | Pixel manipulation |
| 18 | [HDR эффект](tools/18-hdr-effect/index.html) | Расширенный динамический диапазон | Tone mapping |
| 19 | [Пиксель-арт](tools/19-pixel-art/index.html) | Конвертация в пиксельную графику | Color quantization + dithering |
| 20 | [Коллаж](tools/20-collage/index.html) | Объединение нескольких фото | Multiple image loading |
| 21 | [Удаление фона по виньетке](tools/21-vignette-background-removal/index.html) | Прозрачный фон за пределами круга/эллипса | Radial mask + alpha channel |

## 📖 Как использовать

1. Откройте `index.html` в браузере
2. Выберите нужный инструмент
3. Нажмите кнопку загрузки или перетащите изображение на страницу
4. Отрегулируйте параметры с помощью слайдеров или кнопок
5. Нажмите «Скачать», чтобы сохранить результат

## 🧰 Технологии

- **HTML5** — семантическая разметка
- **CSS3** — Flexbox, Grid, CSS-переменные, анимации
- **JavaScript** — чистый JS без фреймворков
- **Canvas API** — обработка изображений
- **CSS Filters** — `brightness()`, `contrast()`, `grayscale()`, `sepia()`, `invert()`

## 📂 Структура проекта

```
Photo-Tools/
├── index.html              ← главная страница
├── README.md
└── tools/
    ├── 01-brightness/
    │   └── index.html
    ├── 02-contrast/
    │   └── index.html
    ├── 03-grayscale/
    │   └── index.html
    ├── 04-sepia/
    │   └── index.html
    ├── 05-invert/
    │   └── index.html
    ├── 06-rotate/
    │   └── index.html
    ├── 07-flip/
    │   └── index.html
    ├── 08-blur/
    │   └── index.html
    ├── 09-sharpen/
    │   └── index.html
    ├── 10-crop/
    │   └── index.html
    ├── 11-resize/
    │   └── index.html
    ├── 12-saturation/
    │   └── index.html
    ├── 13-hue/
    │   └── index.html
    ├── 14-instagram-filters/
    │   └── index.html
    ├── 15-vignette/
    │   └── index.html
    ├── 16-draw-annotate/
    │   └── index.html
    ├── 17-background-removal/
    │   └── index.html
    ├── 18-hdr-effect/
    │   └── index.html
    ├── 19-pixel-art/
    │   └── index.html
    ├── 20-collage/
    │   └── index.html
    └── 21-vignette-background-removal/
        └── index.html
```

## 🌐 Поддерживаемые форматы

- JPEG / JPG
- PNG
- WebP