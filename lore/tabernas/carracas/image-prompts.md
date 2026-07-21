# Carracas — image prompts

Каталог удачных сохранённых концептов каррак и промптов для повторной генерации.

Важно: это не общий архив всех попыток. Здесь зафиксированы только те варианты, которые были выбраны и сохранены как полезные для дальнейшей работы.

## Общие параметры стиля

- **Модель:** `gpt_image_2`
- **Соотношение сторон:** `3:2`
- **Тип изображения:** minimalist semi-abstract watercolor design study
- **Техника:** wet-on-wet watercolor, dark dry-brush accents, large white paper space
- **Материалы мира:** pale bone, dark old wood, rope, torn cloth, leather, dust
- **Палитра:** burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink
- **Ограничение по деталям:** 1 транспорт, 0–2 маленьких безликих пассажира, без лиц крупным планом, без современного автомобиля
- **Стиль-референсы:**
  - `images/style-reference-ancient-ram-test.png`
  - `images/style-reference-wide-single-cart.png`

### Базовый стиль-блок

```text
Use image 1 as the material and vehicle style reference, and image 2 as the loose watercolor atmosphere reference.
Create a minimalist semi-abstract watercolor design study.
The vehicle is made of pale bone ribs, dark old wood, rope lashings and rough cloth.
Forms are simplified wet watercolor shapes: key details suggested by dark blotches and a few sharp angular strokes, secondary elements dissolve into white paper.
Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink.
Lots of white paper space. No fine details, no patterns, no modern metal, no modern car body, no readable text.
```

---

## Light carraca — Cometa

Лёгкая двухместная каррака. Визуально это не машина и не мотоцикл в современном смысле, а лёгкий ветровой скелет: кости, дерево, верёвки, ручное крыло или острый парус, низкая масса, ощущение прыжка.

### `light-cometa-01-three-wheel-arrow`

- **Файл:** `images/light-cometa-01-three-wheel-arrow.png`
- **Смысл:** каноничный кандидат для Cometa; один передний рулевой узел, два задних колеса, узкая “стрела”.
- **Когда использовать:** когда нужен самый читаемый базовый силуэт лёгкой двухместной карраки.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "light-cometa-01-three-wheel-arrow",
  "images": [
    "images/style-reference-ancient-ram-test.png",
    "images/style-reference-wide-single-cart.png"
  ],
  "prompt": "Use image 1 as the material and vehicle style reference, and image 2 as the loose watercolor atmosphere reference. Create a minimalist semi-abstract watercolor design study of a light two-person Cometa carraca: a narrow three-wheel arrow-shaped desert sail frame, one large front steering bone wheel and two smaller rear wheels, a low ribbed bone-and-wood chassis, rope lashings, and a small sharp triangular handheld wing-sail angled forward. It must look ancient and improvised, not like a modern motorcycle or car. Two tiny rider silhouettes may be suggested only as dark simple shapes for scale, no faces. Pale bone ribs, dark old wood, rough cloth, dust. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no text, no modern metal, no realistic car body."
}
```

### `light-cometa-02-two-wheel-dragonfly`

- **Файл:** `images/light-cometa-02-two-wheel-dragonfly.png`
- **Смысл:** самый “мотоциклетный” вариант, но без современного байка; длинная двухколёсная стрекоза.
- **Когда использовать:** когда хочется более рискованный, быстрый и нервный силуэт.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "light-cometa-02-two-wheel-dragonfly",
  "images": [
    "images/style-reference-ancient-ram-test.png",
    "images/style-reference-wide-single-cart.png"
  ],
  "prompt": "Use image 1 as the material and vehicle style reference, and image 2 as the loose watercolor atmosphere reference. Create a minimalist semi-abstract watercolor design study of a light two-person Cometa carraca: a two-wheel dragonfly-like desert sail frame, two large bone wheels in line, a long thin ribbed chassis between them, small side stabilizer bones like folded insect wings, and one sharp dark cloth wing-sail held on short ropes. It must not look like a modern motorcycle: no engine block, no chrome, no modern bike fork. Ancient bone, dark wood, rope, cloth, dust. One or two tiny rider silhouettes only if needed for scale, no faces. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no text."
}
```

### `light-cometa-03-low-bone-cradle`

- **Файл:** `images/light-cometa-03-low-bone-cradle.png`
- **Смысл:** низкая костяная люлька, ближе к kite buggy; устойчивый разведчик.
- **Когда использовать:** когда Cometa должна выглядеть практичной, лёгкой, но не похожей на Мучителя.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "light-cometa-03-low-bone-cradle",
  "images": [
    "images/style-reference-ancient-ram-test.png",
    "images/style-reference-wide-single-cart.png"
  ],
  "prompt": "Use image 1 as the material and vehicle style reference, and image 2 as the loose watercolor atmosphere reference. Create a minimalist semi-abstract watercolor design study of a light two-person Cometa carraca: a very low bone cradle on three wheels, pilot almost lying inside the ribbed frame, passenger space suggested behind, one dark sharp triangular wing-sail on short ropes, no tall mast. The vehicle should feel fast, dangerous and homemade, like a kite buggy made from bones and old wood. Do not make it a car; no modern suspension or body panels. Pale bone ribs, dark old wood, rope lashings, torn cloth, dust. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no text."
}
```

### `light-cometa-04-kite-landboard-riders`

- **Файл:** `images/light-cometa-04-kite-landboard-riders.png`
- **Смысл:** четырёхколёсная кайт-доска с экипажем; самый отличающийся от багги вариант.
- **Когда использовать:** для дешёвой, хлипкой, опасной или клановой модификации Cometa.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "light-cometa-04-kite-landboard-riders",
  "images": [
    "images/light-cometa-03-low-bone-cradle.png",
    "images/style-reference-ancient-ram-test.png"
  ],
  "prompt": "Use image 1 as the vehicle form reference, and image 2 as the bone-and-watercolor style reference. Create a minimalist semi-abstract watercolor design study of the same light Cometa class, redesigned as a long four-wheel kite-landboard carraca with two tiny hooded rider silhouettes. The riders are only dark simple clothing shapes, no faces. One rider pulls a short rope to control a sharp triangular cloth wing-sail; the second crouches low on the rear platform. The board is made of pale bone rails, dark old wood and rope lashings, with four rough desert wheels. Keep it ancient and fragile, not modern sports equipment. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no text."
}
```

### `light-cometa-05-two-wheel-dragonfly-riders`

- **Файл:** `images/light-cometa-05-two-wheel-dragonfly-riders.png`
- **Смысл:** двухколёсная стрекоза с одним-двумя седоками для масштаба.
- **Когда использовать:** если нужно показать, что вариант действительно рассчитан на людей, а не просто на абстрактную раму.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "light-cometa-05-two-wheel-dragonfly-riders",
  "images": [
    "images/light-cometa-02-two-wheel-dragonfly.png",
    "images/style-reference-ancient-ram-test.png"
  ],
  "prompt": "Use image 1 as the vehicle form reference, and image 2 as the bone-and-watercolor style reference. Create a minimalist semi-abstract watercolor design study of the same two-wheel dragonfly Cometa, now with one or two tiny hooded rider silhouettes for scale. The riders must be small dark shapes with no faces and no detail. Keep the long two-wheel bone frame, side stabilizer bones, rope lashings and sharp triangular wing-sail. Make it feel ancient, lightweight, fast and unsafe, not like a modern motorcycle. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no text."
}
```

### `light-cometa-06-low-bone-cradle-riders`

- **Файл:** `images/light-cometa-06-low-bone-cradle-riders.png`
- **Смысл:** низкая люлька с седоками; хороший рабочий вариант для “лёгкой багги”.
- **Когда использовать:** если нужно совместить практичность, читаемость и масштаб.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "light-cometa-06-low-bone-cradle-riders",
  "images": [
    "images/light-cometa-03-low-bone-cradle.png",
    "images/style-reference-ancient-ram-test.png"
  ],
  "prompt": "Use image 1 as the vehicle form reference, and image 2 as the bone-and-watercolor style reference. Create a minimalist semi-abstract watercolor design study of the same low bone cradle Cometa, now with one small hooded pilot and one even smaller passenger silhouette. The people are only simple dark clothing shapes, no faces, no anatomy detail. Keep the vehicle very low: ribbed bone cradle, three rough wheels, short ropes, one sharp triangular dark cloth wing-sail, no tall mast. Ancient bone-and-wood construction, dust, handmade danger. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no text."
}
```

---

## Medium carraca — Tormentor / Мучитель

Средняя четырёхместная каррака. Это уже боевой багги-класс: больше массы, больше рамы, один водитель для масштаба, но всё ещё не современная машина. Парус — острый косой треугольный, ближе к латинскому парусу.

### `medium-buggy-04-scorpion-frame`

- **Файл:** `images/medium-buggy/medium-buggy-04-scorpion-frame.png`
- **Смысл:** самый злой и характерный вариант, скорпионья рама.
- **Когда использовать:** когда нужен агрессивный боевой Мучитель.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "medium-buggy-04-scorpion-frame",
  "images": [
    "images/style-reference-ancient-ram-test.png"
  ],
  "prompt": "Use image 1 as the watercolor and carraca style reference. Create a minimalist semi-abstract watercolor design study of a medium Tormentor carraca: a scorpion-like desert sail buggy for four people, with a low aggressive bone-and-wood frame, arched tail-like rear support, horned bone ram spikes on the front bumper, large rough wheels, rope lashings, and one small faceless driver silhouette seated low for scale. Add a sharp triangular lateen-style sail, not a square rag. The vehicle should look ancient, brutal and improvised, not like a real modern car. Pale bone ribs, dark old wood, rough cloth, dust. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no readable text."
}
```

### `medium-buggy-05-low-wedge-sail-buggy`

- **Файл:** `images/medium-buggy/medium-buggy-05-low-wedge-sail-buggy.png`
- **Смысл:** низкий клин, быстрый и агрессивный.
- **Когда использовать:** когда Мучитель должен казаться скоростным тараном.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "medium-buggy-05-low-wedge-sail-buggy",
  "images": [
    "images/style-reference-ancient-ram-test.png"
  ],
  "prompt": "Use image 1 as the watercolor and carraca style reference. Create a minimalist semi-abstract watercolor design study of a medium Tormentor carraca: a low wedge-shaped desert sail buggy for four people, with a sloped bone ram prow, tusk-like spikes on the bumper, wide rear wheels, a narrow ribbed cockpit, rope lashings, and one small faceless driver silhouette for scale. The sail is a sharp triangular lateen-style cloth sail leaning backward, not a square torn flag. It must feel like an ancient bone-and-wood war buggy, not a modern dune buggy or car. Pale bone, dark old wood, rough cloth, dust. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no text."
}
```

### `medium-buggy-06-bone-sand-rail`

- **Файл:** `images/medium-buggy/medium-buggy-06-bone-sand-rail.png`
- **Смысл:** базовый sand rail / багги-вариант, самый понятный как транспорт.
- **Когда использовать:** когда нужна нейтральная каноничная форма Мучителя.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "medium-buggy-06-bone-sand-rail",
  "images": [
    "images/style-reference-ancient-ram-test.png"
  ],
  "prompt": "Use image 1 as the watercolor and carraca style reference. Create a minimalist semi-abstract watercolor design study of a medium Tormentor carraca: a four-person desert sand-rail buggy built from pale bone tubes, dark wood braces and rope lashings. Show a simple open cage frame, four rough wheels, a front bone ram with horn-like spikes, one small faceless driver silhouette, and a sharp triangular lateen-style sail. Keep the silhouette readable and ancient, not a modern off-road car. Forms dissolve into white paper at the edges. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no text."
}
```

### `medium-buggy-07-tall-cage-buggy`

- **Файл:** `images/medium-buggy/medium-buggy-07-tall-cage-buggy.png`
- **Смысл:** более бронированный вариант с высокой клеткой-рамой.
- **Когда использовать:** для защищённой, караванной или командирской модификации.

```json
{
  "model": "gpt_image_2",
  "aspect_ratio": "3:2",
  "filename": "medium-buggy-07-tall-cage-buggy",
  "images": [
    "images/style-reference-ancient-ram-test.png"
  ],
  "prompt": "Use image 1 as the watercolor and carraca style reference. Create a minimalist semi-abstract watercolor design study of a medium Tormentor carraca: a tall cage-frame sail buggy for four people, built from vertical pale bone ribs, dark old wood braces and rope lashings. It has four rough wheels, a protected raised cockpit, one small faceless driver silhouette, horn-like bone spikes on the front ram, and a sharp triangular lateen-style sail rising above the cage. It should look ancient and handmade, not like a modern car or armored vehicle. Very few colors: burnt orange, dusty ochre, ashen grey-brown, bone white, sparse dark ink. Lots of white paper space. No fine details, no text."
}
```

---

## Быстрый выбор по задаче

- **Базовая Cometa:** `light-cometa-01-three-wheel-arrow`
- **Cometa ближе к “мотоциклу”:** `light-cometa-02-two-wheel-dragonfly` или `light-cometa-05-two-wheel-dragonfly-riders`
- **Практичная Cometa с людьми:** `light-cometa-06-low-bone-cradle-riders`
- **Самый отличающийся дешёвый/клановый вариант:** `light-cometa-04-kite-landboard-riders`
- **Базовый Мучитель:** `medium-buggy-06-bone-sand-rail`
- **Злой боевой Мучитель:** `medium-buggy-04-scorpion-frame`
- **Быстрый таран:** `medium-buggy-05-low-wedge-sail-buggy`
- **Защищённый/командирский Мучитель:** `medium-buggy-07-tall-cage-buggy`

## Негативные правила для будущих генераций

Добавлять в конец промпта, если модель начинает “ломаться”:

```text
Do not draw a modern car, motorcycle, engine, chrome, rubber tire detail, realistic dashboard, headlights, license plate, sci-fi vehicle, many people, detailed faces, readable text, decorative border, busy background.
Only one vehicle. At most one or two tiny faceless rider silhouettes.
```
