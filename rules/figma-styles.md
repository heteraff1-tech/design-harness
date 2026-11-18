# Variables и стили Figma проекта «Здоровье»

Снимок локальных определений файла и привязок секции [«Здоровье · Исходные макеты»](https://www.figma.com/design/u0EdPHQOmvdQuc7158uN5C/Untitled?node-id=77-4755).

## Variables

| Коллекция | Режимы | Локальных переменных | Пути в DTCG |
| --- | --- | --- | --- |
| Health · Colors | Light по умолчанию, Dark | 54 | `color.light.*` и `color.dark.*` |
| Health · Dimensions | Value | 30 | `radius.*`, `size.*`, `font.*` |

Для выбора роли используй [список семантических имён](tokens-summary.md). В DTCG исходное имя и ID сохранены в метаданных, размеры записаны в `px`. Например, Figma `bg/page` соответствует `color.light.bg.page` или `color.dark.bg.page`. При импорте выбирай ветку по активной теме. Числовые свойства типографики описаны отдельными размерными токенами.

`font.family` хранит значение `SF Pro` из коллекции Dimensions. Текстовые стили проекта ниже используют `SB Sans Display` и `SB Sans Text`.

Актуальная коллекция Dimensions содержит радиусы, размеры контролов и параметры шрифтов. В слоях этих экранов остались привязки `space/4` (4 px) и `space/8` (8 px), которые читаются по ID, но отсутствуют в списке переменных коллекции. Перед повторным использованием уточни, нужно ли восстановить их или заменить на утверждённые токены отступов.

## Text Styles

Все численные значения в таблице указаны в px. «В секции» означает, что в дереве целевых фреймов обнаружена привязка к этому стилю.

| Имя Figma | Семейство и начертание | Кегль | Интерлиньяж | Трекинг | В секции | Назначение |
| --- | --- | ---: | --- | ---: | --- | --- |
| `Health/Heading/H1` | SB Sans Display Semibold | 24 | 30 | 0 | Да | Приветствие на экране помощника. |
| `Health/Heading/H2` | SB Sans Display Semibold | 20 | 26 | 0 | — | Заголовки экранов и компактное приветствие. |
| `Health/Heading/H3` | SB Sans Display Regular | 18 | 22 | 0 | Да | Заголовки карточек и быстрых действий. |
| `Health/Heading/H4` | SB Sans Display Semibold | 16 | 20 | 0 | Да | Компактные заголовки блоков и диапазонов. |
| `Health/Display/Metric` | SB Sans Display Semibold | 44 | 54 | -1.6 | Да | Крупное числовое показание метрики. |
| `Health/Display/Metric-2` | SB Sans Display Semibold | 32 | 30 · `font.line.heading.h1` | -1.6 | Да | Крупное числовое показание метрики. |
| `Health/Text/Body` | SB Sans Text Regular | 16 | 21 | 0 | Да | Основной текст и ввод сообщения. |
| `Health/Text/Label` | SB Sans Text Medium | 14 | 18 | 0 | Да | Кнопки, подписи действий и заголовки метрик. |
| `Health/Text/Small` | SB Sans Text Regular | 13 | 18 | 0 | Да | Короткая подпись или статус. |
| `Health/Text/Footnote` | SB Sans Text Medium | 12 | 16 | 0 | Да | Табы и подписи выбранного измерения. |
| `Health/Text/Caption` | SB Sans Text Regular | 11 | 13 | 0 | Да | Подписи осей, легенды и единицы. |

У этих стилей исходный регистр, без декора, с нулевыми межабзацным интервалом и отступом. Трекинг двух стилей Metric показан с округлением до −1,6 px. У `Health/Display/Metric-2` интерлиньяж привязан к `font/line/heading/h1` в Figma. У остальных текстовых стилей в каталоге Variable-привязок на уровне определения стиля нет.

## Стили и переменные подключённых библиотек

Локальные Paint Styles, Effect Styles и Grid Styles в файле отсутствуют. В целевых фреймах встречаются привязки к библиотечным Variables. При сборке в Figma переиспользуй их через исходные экземпляры.

| Коллекция | Переменные, найденные в секции |
| --- | --- |
| Color Scheme | `Mode` (Light и Dark), `Labels - Vibrant/Primary` (алиас в каждом режиме) |
| Kit | `Liquid Glass/Opacity` 25, `Refraction` 70, `Frost - Regular` 6, `Light Angle` 0, `Splay - Regular` 20, `Depth - Regular` 30, `Dispersion` 20 |

Экспорт ограничен локальными коллекциями Health. Параметры Kit приведены в исходных единицах Figma.

Спецификация формата — [DTCG 2025.10](https://www.designtokens.org/tr/2025.10/format/).
