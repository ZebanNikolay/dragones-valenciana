# D&D Art Style — Минималистичная акварель

> Единый стиль для генерации арта к приключениям кампании **Dragones Valenciana**.
> Выбран 14 апреля 2026 после калибровки из 6 стилей.

---

## Шаблон промпта (Style Template)

Вставлять в начало каждого промпта перед описанием конкретной сцены:

```
Minimalist semi-abstract watercolor. [SCENE DESCRIPTION]. Forms are simplified wet watercolor shapes — key details suggested by dark blotches and sharp angular strokes, secondary elements dissolve at edges. Very few colors: [PALETTE — 3-5 colors max]. Lots of white paper space. Scene is clearly readable but forms dissolve where they meet the background. No fine details, no textures, no patterns. Atmospheric, moody, evocative. Wet-on-wet watercolor technique with occasional sharp dry-brush accents for focal points.
```

### Обязательные правила стиля

| Правило | Описание |
|---|---|
| **Минимализм** | Только необходимые элементы. Никакой избыточности |
| **Белое пространство** | Большая часть «холста» — пустая белая бумага |
| **Палитра** | 3-5 цветов максимум. Приглушённые + 1 акцент |
| **Читаемость** | Сцена понятна с первого взгляда, несмотря на абстрактность |
| **Растворение** | Формы чёткие в центре внимания, размываются к краям |
| **Фон** | Минимальные намёки — пара пятен, силуэты, дымка |
| **НЕ делать** | Не копировать конкретных художников, без зализанности, без красивых эльфийских лиц, без мелких деталей, без рамок/текста |

### Палитры по темам

| Тема | Цвета |
|---|---|
| **Пустошь / Mad Max** | burnt orange, ashen grey-brown, dried blood red, bone white |
| **Лес / природа** | deep olive green, warm brown, misty grey, golden amber |
| **Ночь / тревога** | deep indigo, cold grey, pale amber (огни), charcoal |
| **Бой / осада** | burnt sienna, smoke grey, blood red accent, dusty ochre |
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

Безумный гоблин-мутант в шлеме из черепа, указывающий вперёд с хищным оскалом. На заднем плане — размытые силуэты бегущих дикарей в оранжевой дымке пустоши. Формы растворяются в мокрых акварельных пятнах, много белого пространства.

**Файл:** `goblin_03_watercolor.png`

---

## Как использовать (арт сцен)

1. Взять **шаблон** из секции выше
2. Заменить `[SCENE DESCRIPTION]` на описание сцены
3. Заменить `[PALETTE]` на подходящую палитру из таблицы (или свою из 3-5 цветов)
4. Соотношение сторон: `4:3` для сцен, `3:4` для портретов, `16:9` для панорам
5. Генерировать через `asi-generate-image`

---

## Шаблон промпта для заголовков (Title Template)

Отдельный шаблон для генерации названий приключений как изображений.
Модель: обязательно `gpt_image_1_5` (умеет рисовать текст).

```
The text [YOUR TITLE] written in a single horizontal line in black watercolor on white paper. The letters show rich watercolor texture: where the brush carried more pigment the black is deep and saturated, where less pigment it fades to translucent grey. The edges of each letter bleed softly outward into the wet paper — feathered, diffused borders typical of wet-on-wet watercolor technique. Visible variation in ink density within each stroke. Only a few tiny satellite droplets near letters, no heavy drips streaming downward, no large splatter clouds. The overall feel is handmade, organic, with that distinctive watercolor bloom effect at letter edges. Pure black ink only on white background, no other colors, no other elements.
```

### Обязательные правила для заголовков

| Правило | Описание |
|---|---|
| **Одна строка** | Весь текст в одну горизонтальную строку |
| **Только чёрный** | Никаких цветов, только чёрная акварель |
| **Акварельная текстура** | Расплывшиеся мягкие края букв, перепады плотности пигмента |
| **Минимум шума** | Пара мелких капель рядом — не больше. Без крупных потёков вниз |
| **Модель** | `gpt_image_1_5` — единственная модель, корректно рисующая текст |
| **Формат** | `16:9` — горизонтальный, чтобы текст поместился в строку |

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
2. Скриптом обрезать белые поля (crop по тёмным пикселям)
3. Масштабировать до ~75% ширины основной картинки
4. Расширить холст арта вниз и вклеить заголовок по центру
5. Гоблин / основная картинка при этом остаётся пиксель-в-пиксель

---

## Пример: заголовок «GUARDIANES DEL OMBLIGO»

### Промпт

```
The text GUARDIANES DEL OMBLIGO written in a single horizontal line in black watercolor on white paper. The letters show rich watercolor texture: where the brush carried more pigment the black is deep and saturated, where less pigment it fades to translucent grey. The edges of each letter bleed softly outward into the wet paper — feathered, diffused borders typical of wet-on-wet watercolor technique. Visible variation in ink density within each stroke. Only a few tiny satellite droplets near letters, no heavy drips streaming downward, no large splatter clouds. The overall feel is handmade, organic, with that distinctive watercolor bloom effect at letter edges. Pure black ink only on white background, no other colors, no other elements.
```

### Результат

Чёрная акварельная надпись в одну строку — мягкие расплывшиеся края, перепады плотности пигмента, пара мелких капель. Совмещена с гоблином-дикарём (75% ширины, под картинкой).

**Файл надписи:** `title_v1c_watercolor_bloom.png`
**Файл с артом:** `goblin_wc_bloom_title.png`
