# D&D Art Style — Минималистичная акварель

> Единый стиль для генерации арта к приключениям кампании **Dragones Valenciana**.
> Выбран 14 апреля 2026 после калибровки из 6 стилей.

---

## Шаблон промпта (Style Template)

Вставлять в начало каждого промпта перед описанием конкретной сцены:

```
Minimalist semi-abstract watercolor. [SCENE DESCRIPTION]. Forms are simplified wet watercolor shapes — key details suggested by dark blotches and sharp angular strokes, secondary elements dissolve at edges. Very few colors: [PALETTE — 3-5 colors max]. Lots of white paper space. Scene is clearly readable but forms dissolve where they meet the background. No fine details, no textures, no patterns. Atmospheric, moody, evocative. Wet-on-wet watercolor technique with occasional sharp dry-brush accents for focal points.
```

### Обязательные правила стиля

| Правило | Описание |
|---|---|
| **Минимализм** | Только необходимые элементы. Никакой избыточности |
| **Белое пространство** | Большая часть «холста» — пустая белая бумага |
| **Палитра** | 3-5 цветов максимум. Приглушённые + 1 акцент |
| **Читаемость** | Сцена понятна с первого взгляда, несмотря на абстрактность |
| **Растворение** | Формы чёткие в центре внимания, размываются к краям |
| **Фон** | Минимальные намёки — пара пятен, силуэты, дымка |
| **НЕ делать** | Не копировать конкретных художников, без зализанности, без красивых эльфийских лиц, без мелких деталей, без рамок/текста |

### Палитры по темам

| Тема | Цвета |
|---|---|
| **Пустошь / Mad Max** | burnt orange, ashen grey-brown, dried blood red, bone white |
| **Лес / природа** | deep olive green, warm brown, misty grey, golden amber |
| **Ночь / тревога** | deep indigo, cold grey, pale amber (огни), charcoal |
| **Бой / осада** | burnt sienna, smoke grey, blood red accent, dusty ochre |
| **Магия / портал** | muted teal, warm amber glow, deep purple, pale gold |

---

## Пример: Гоблин-дикарь пустоши

### Промпт

```
Minimalist semi-abstract watercolor. Close-up of a wasteland mutant goblin pointing forward — mad hungry predator gaze, crazed grin, commanding an attack. Face is simplified wet watercolor shapes — tumors and bone growths suggested by dark blotches, skull helmet a rough dark wash. Pointing finger is a sharp angular stroke. Background: vast empty white paper with faint warm washes suggesting scorched wasteland, a few tiny dark silhouettes of raiders barely visible in the haze. Very few colors: burnt orange, ashen grey-brown, dried blood spot. Lots of white space. Scene is clearly readable but forms dissolve at edges.
```

### Параметры генерации

```json
{
  "prompt": "[см. выше]",
  "filename": "goblin_wasteland_raider",
  "aspect_ratio": "4:3"
}
```

### Результат

Безумный гоблин-мутант в шлеме из черепа, указывающий вперёд с хищным оскалом. На заднем плане — размытые силуэты бегущих дикарей в оранжевой дымке пустоши. Формы растворяются в мокрых акварельных пятнах, много белого пространства.

**Файл:** `goblin_03_watercolor.png`

---

## Как использовать (арт сцен)

1. Взять **шаблон** из секции выше
2. Заменить `[SCENE DESCRIPTION]` на описание сцены
3. Заменить `[PALETTE]` на подходящую палитру из таблицы (или свою из 3-5 цветов)
4. Соотношение сторон: `4:3` для сцен, `3:4` для портретов, `16:9` для панорам
5. Генерировать через `asi-generate-image`

---

## Шаблон промпта для заголовков (Title Template)

Отдельный шаблон для генерации названий приключений как изображений.
Модель: обязательно `gpt_image_1_5` (умеет рисовать текст).

> **Важно:** без явного описания формы букв модель каждый раз выбирает разный шрифт (может выдать курсив, скоропись, засечки и т.д.). Описание шрифта ниже фиксирует стиль, чтобы все заголовки серии выглядели одинаково.

```
The text "[YOUR TITLE]" written in ONE SINGLE HORIZONTAL LINE on white paper, all words on the same line, no line breaks. ALL LETTERS ARE UPPERCASE CAPITAL LETTERS. The letterforms are hand-painted with a medium round brush — straight, slightly irregular strokes, moderate weight (not super heavy/blocky, not thin either), narrow proportions so all characters fit on one row, no italic slant, no cursive connections between letters, no script handwriting. Each letter stands separately with clear gaps. Some letters slightly taller or shorter than neighbors for handmade feel. The letters show rich black watercolor texture with visible variation in ink density — some strokes deep saturated black, others fading to translucent grey. Edges bleed softly outward into the wet paper with feathered borders typical of wet-on-wet watercolor. Only a few tiny satellite droplets near letters, no heavy drips, no large splatter. Pure black ink on white background, no other colors, no other elements.
```

### Обязательные правила для заголовков

| Правило | Описание |
|---|---|
| **Одна строка** | Весь текст в одну горизонтальную строку, никаких переносов |
| **ВСЁ ЗАГЛАВНЫМИ** | ALL UPPERCASE CAPITAL LETTERS — обязательно прописать большими в промпте |
| **Форма букв** | Рубленые (sans-serif), прямые штрихи, средний вес, узкие пропорции |
| **БЕЗ курсива** | no italic slant, no cursive connections, no script handwriting — обязательно явно запретить |
| **Отдельные буквы** | Each letter stands separately with clear gaps — буквы не соединяются |
| **Лёгкая неровность** | Some letters slightly taller or shorter — рукотворное ощущение |
| **Только чёрный** | Никаких цветов, только чёрная акварель |
| **Акварельная текстура** | Расплывшиеся мягкие края, перепады плотности пигмента |
| **Минимум шума** | Пара мелких капель рядом — не больше. Без крупных потёков вниз |
| **Модель** | `gpt_image_1_5` — единственная модель, корректно рисующая текст |
| **Формат** | `16:9` — горизонтальный, чтобы текст поместился в строку |

### Параметры генерации

```json
{
  "prompt": "[см. шаблон выше, заменить YOUR TITLE]",
  "filename": "title_adventure_name",
  "aspect_ratio": "16:9",
  "model": "gpt_image_1_5"
}
```

### Как совмещать с артом

1. Сгенерировать заголовок отдельно по шаблону выше
2. Скриптом обрезать белые поля (crop по тёмным пикселям)
3. Масштабировать до ~75% ширины основной картинки
4. Расширить холст арта вниз и вклеить заголовок по центру
5. Гоблин / основная картинка при этом остаётся пиксель-в-пиксель

---

## Примеры заголовков

### «GUARDIANES DEL OMBLIGO» (приключение 4)

**Файл надписи:** `title_v1c_watercolor_bloom.png`
**Файл с артом:** `goblin_wc_bloom_title.png`

### «HUESOS DE PRUEBA» (приключение 5)

**Файл надписи:** `adventures/005-huesos-de-prueba/images/title.png`

Промпт собирается из шаблона выше подстановкой `HUESOS DE PRUEBA` вместо `[YOUR TITLE]`.
