# Генерация изображения для модуля (Perplexity AI)

## 📋 Общая схема

**5 ПРОСТЫХ ШАГОВ:**

| Шаг | Что делаем | Загружаем | Получаем |
|-----|------------|-----------|----------|
| **1** | Одеть в костюм | Ваше фото | Повар на кухне |
| **2** | Поместить в лес | Фото куролиска | Куролиск в лесу |
| **3** | Объединить | Результаты 1+2 | Композиция с рамкой |
| **4** | Добавить текст | Результат 3 | Постер с названием |
| **5** | Стилизовать | Результат 4 + Фото стиля | Живопись |

**Что нужно подготовить:**
- ✅ Ваша фотография (где держите паэльеру)
- ✅ Фото куролиска из интернета (классное изображение монстра)
- ✅ Фото стиля (человек с пластиковыми динозаврами)

**Инструмент:** Perplexity AI (модель: Nano Banana или FLUX.1)

**Настройка модели:** Settings → Preferences → Image generation model → выбрать **Nano Banana**

**ВАЖНО:** Мы НЕ создаём изображения с нуля - мы используем ВАШИ фото и только меняем окружение/стиль!

---

## ШАГ 1: Одеть в костюм повара

### Что делаем
Берём ВАШУ фотографию и добавляем только костюм повара + заполненную паэлью. Больше НИЧЕГО не меняем.

### Входные данные
- **Загрузите:** Вашу фотографию (где держите паэльеру)

### ПРОМПТ ДЛЯ КОПИРОВАНИЯ

```
Photo editing task. Transform only the costume and props, preserve everything else.

INPUT: Uploaded photo of a person holding a paella pan

PRESERVE 100% (DO NOT CHANGE):
- The person's face (features, expression, skin)
- Body pose and position
- Hand positions
- Overall person identity

ADD ONLY these elements:
1. White chef's hat (toque blanche) on the head
2. White chef's jacket (double-breasted) on the body
3. Fill the paella pan with golden paella valenciana:
   - Saffron yellow rice
   - Pieces of cooked meat
   - Green beans
   - White beans
   - Rosemary sprigs
   - Professional presentation

BACKGROUND:
Change to professional Mediterranean kitchen:
- Hanging copper pots on wall
- Brick oven visible
- Warm orange/yellow lighting
- Wooden counters

STYLE: Photographic, realistic. Keep it natural.

CRITICAL INSTRUCTIONS:
- DO NOT add any monsters or creatures
- DO NOT add fantasy elements
- DO NOT change the person's face
- This is ONLY costume and background change
- Focus ONLY on the chef transformation
```

### Результат
Фотография повара в белом костюме с заполненной паэльей на фоне кухни.

---

## ШАГ 2: Поместить куролиска в лес

### Что делаем
Берём ВАШЕ фото куролиска из интернета и помещаем его в лесное окружение с гнездом. НЕ создаём нового монстра, ИСПОЛЬЗУЕМ существующее изображение.

### Входные данные
- **ОБЯЗАТЕЛЬНО загрузите:** Фото куролиска (ваше изображение из интернета)

### ПРОМПТ ДЛЯ КОПИРОВАНИЯ

```
Photo manipulation task. Place the uploaded creature into forest environment.

INPUT: Uploaded photo of cockatrice/monster

PRESERVE 100% (DO NOT CHANGE):
- The creature from uploaded photo (EXACT appearance)
- Monster's pose, features, colors
- Keep the creature EXACTLY as it appears in uploaded image
- Do NOT redraw or recreate the monster
- Do NOT change creature to look like a chicken or rooster

TASK: Change ONLY the background and add environment elements

NEW ENVIRONMENT: Forest clearing
- Ancient tall trees surrounding the creature
- Forest floor with moss, rocks, fallen leaves
- ADD: Nest with 5-6 large eggs on ground near the creature (slightly behind)
- Dappled sunlight through tree canopy
- Mystical forest atmosphere
- Cool green and blue lighting tones
- Slight mist for depth

LIGHTING adjustment:
- Adjust lighting on creature to match forest environment
- Dramatic forest lighting with shafts of sunlight
- Shadows and depth
- Keep creature visible and clear

COMPOSITION:
- Creature as main focus (take from uploaded photo)
- Position creature in center-left
- Nest visible in background
- Leave empty space on right side (will be used for later composition)
- Vertical or square format preferred

STYLE: Fantasy scene, atmospheric, dramatic

CRITICAL INSTRUCTIONS:
- USE the uploaded creature image as-is
- DO NOT generate a new monster
- DO NOT change the creature's appearance
- ONLY change the background to forest
- Think: "photo compositing" not "creature creation"
- The uploaded monster is PERFECT - just place it in forest setting
```

### Результат
Ваш куролиск (из загруженного фото) помещён в лесное окружение с гнездом.

---

## ШАГ 3: Объединить композицию

### Что делаем
Берём результаты Шагов 1 и 2 и объединяем в единую композицию с плавным переходом. Добавляем декоративную рамку внизу для текста. Пока БЕЗ стиля живописи - просто соединяем две фотографии красиво.

### Входные данные
- **Загрузите 2 изображения:**
  1. Результат Шага 1 (повар на кухне)
  2. Результат Шага 2 (куролиск в лесу)

### ПРОМПТ ДЛЯ КОПИРОВАНИЯ

```
Advanced photo compositing and blending task. Seamlessly merge two uploaded images into one unified horizontal composition with natural, magical transition.

INPUT IMAGES:
- Image 1: Chef in kitchen (from Step 1)
- Image 2: Cockatrice in forest (from Step 2)

MAIN TASK: Create seamless blend with NO visible border or harsh edge between images.

COMPOSITION LAYOUT:

LEFT SIDE (50% of width):
- Use Image 2 (cockatrice in forest)
- Monster and mystical forest environment
- Cool dramatic lighting (greens, blues, teals)
- Ancient trees, nest with eggs
- Keep all creature details from uploaded image

RIGHT SIDE (50% of width):
- Use Image 1 (chef in kitchen)
- Chef with paella on Mediterranean kitchen background
- Warm lighting (oranges, yellows, browns)
- Copper pots, brick oven
- Keep all chef details from uploaded image

CENTER TRANSITION ZONE (20% overlap in middle):
CRITICAL - This is the most important part:
- Create SEAMLESS, GRADUAL blend between forest and kitchen
- Use ethereal magical mist/fog that flows from forest into kitchen
- Mystical smoke effect connecting both worlds
- Soft gradient transition - NO hard edge, NO black line, NO sharp border
- Colors blend smoothly: cool tones gradually warming up
- Dragon eggs should emit subtle golden glow that echoes kitchen warmth
- Atmospheric depth with translucent fog
- Think: "two worlds merging through magical portal" not "two separate photos side by side"

ALIGNMENT & PROPORTIONS:
- Align both images at the TOP edge
- If images have different heights (forest image taller than chef):
  * Keep both images at full quality
  * Create decorative bottom section to fill any gaps
- Create elegant TEXT FRAME at the bottom:
  * Decorative dark banner/border (deep forest green or warm brown)
  * Ornamental design with subtle fantasy patterns
  * Medieval/fantasy style decorative frame
  * This area is specifically for text overlay later
  * Should look intentional and beautiful, not like a mistake
  * Width: full image width
  * Height: whatever needed to make composition rectangular
- Overall composition should be rectangular with unified professional look

LIGHTING HARMONY:
- Blend lighting in transition zone
- Forest light gradually warming toward kitchen
- Kitchen warmth subtly reaching into forest edge
- Unified atmospheric lighting across entire composition
- Shadows and highlights should connect naturally

FORMAT & LAYOUT:
- Horizontal panoramic poster format
- Epic cinematic composition with decorative bottom text frame
- Professional fantasy photography aesthetic
- Decorative banner/border at bottom for text (ornamental medieval/fantasy style)
- Main images aligned at top, decorative frame fills bottom if needed
- Overall feeling: seamless magical realism with professional poster design

STYLE: Keep photographic/realistic
- DO NOT apply painting style yet
- Keep images as high-quality photos
- Focus on PERFECT blending and transition
- Natural photo compositing with magical atmosphere
- No filters, no artistic effects yet

CRITICAL REQUIREMENTS:
✓ NO visible seam or border line between images
✓ NO harsh edge where images meet
✓ NO black bars or gaps anywhere
✓ NO mismatched heights or proportions
✓ Smooth, gradual, magical transition in center
✓ Both images perfectly aligned and blended
✓ Looks like ONE unified scene, not two separate photos
✓ Mystical fog/mist creates natural connection

NEGATIVE (what to AVOID):
✗ Split-screen effect with clear division line
✗ Sharp border or straight edge between scenes
✗ Black line separating the images
✗ Mismatched heights creating gaps
✗ Jarring transition
✗ Two disconnected scenes side by side

RESULT: One seamless panoramic poster showing mystical forest with dragon on left flowing magically into warm kitchen with chef on right, with elegant decorative frame at bottom for text overlay. The transition should be so smooth that it feels like one magical scene, not two separate images combined. Bottom decorative banner should look intentional and beautiful, perfect for adding adventure title or text later.
```

### Результат
Композиция из двух фотографий: повар справа, куролиск слева, плавный переход в центре, декоративная рамка внизу для текста. Пока в фотографическом стиле.

---

## ШАГ 4: Добавить название модуля

### Что делаем
Берём композицию из Шага 3 и добавляем текст "Куролиск для Paella Valenciana" в декоративную рамку внизу.

### Входные данные
- **Загрузите:** Результат Шага 3 (композиция с рамкой)

### ПРОМПТ ДЛЯ КОПИРОВАНИЯ

```
Text overlay task. Add adventure module title to the decorative frame at bottom of uploaded image.

INPUT IMAGE:
- Uploaded composition from Step 3 (chef + cockatrice with decorative bottom frame)

TASK: Add text to the bottom decorative frame/banner

TEXT TO ADD:
Line 1 (main title): "КУРОЛИСК"
Line 2 (subtitle): "для Paella Valenciana"

TEXT STYLING:

Main title "КУРОЛИСК":
- Large, bold fantasy font
- Medieval/gothic style lettering
- Color: Gold/cream or light color that contrasts with dark frame
- Dominant and eye-catching
- Centered horizontally
- All capital letters
- Slightly ornamental but readable

Subtitle "для Paella Valenciana":
- Smaller, elegant font below main title
- More refined, script or serif style
- Same color scheme as main title (gold/cream)
- Centered horizontally
- Mix of Cyrillic and Latin letters (keep as written)

FRAME INTEGRATION:
- Text should sit beautifully within the decorative bottom frame
- Good spacing from frame edges
- Text color should complement frame decoration
- If frame has ornamental elements, text should work harmoniously with them
- Overall look: professional fantasy adventure poster/book cover

LAYOUT:
- Both text lines centered in bottom decorative frame
- Main title takes 60% of vertical space in frame
- Subtitle takes 30% of vertical space
- Leave some breathing room (10% padding)

STYLE: Fantasy adventure module poster
- Think: D&D adventure module cover, fantasy book title
- Professional, epic, inviting
- Readable but stylized
- Title should look integral to the design, not just slapped on

CRITICAL REQUIREMENTS:
✓ Text must be CLEARLY READABLE
✓ Cyrillic letters "КУРОЛИСК" must render correctly
✓ Good contrast between text and frame background
✓ Professional typography
✓ Text integrated naturally into decorative frame
✓ Maintains poster/cover aesthetic

DO NOT:
✗ Cover or overlap the main images (forest or kitchen scenes)
✗ Use plain boring fonts
✗ Make text too small or hard to read
✗ Place text outside the bottom decorative frame
✗ Use colors that don't contrast well with frame

RESULT: Fantasy adventure poster with clear, beautiful title "КУРОЛИСК для Paella Valenciana" integrated into bottom decorative frame.
```

### Результат
Постер с названием модуля "Куролиск для Paella Valenciana" красиво размещенным в декоративной рамке внизу. Пока в фотографическом стиле.

---

## ШАГ 5: Стилизация под живопись

### Что делаем
Берём готовый постер из Шага 4 (с текстом) и применяем стиль живописи с видимыми мазками кисти.

### Входные данные
- **Загрузите 2 изображения:**
  1. Результат Шага 4 (постер с названием "Куролиск для Paella Valenciana")
  2. Фото стиля (человек с пластиковыми динозаврами - ваш референс)

### ПРОМПТ ДЛЯ КОПИРОВАНИЯ

```
Apply painting style to uploaded poster. Transform photo poster into painted artwork.

INPUT IMAGES:
- Image 1: Photo poster with text (chef + cockatrice + title "Куролиск для Paella Valenciana" from Step 4)
- Image 2: Style reference (man with dinosaurs - contemporary figurative painting style)

TASK: Apply contemporary figurative painting style to Image 1, using Image 2 as style guide.

PAINTING STYLE APPLICATION:
Apply oil/acrylic painting aesthetic to entire composition:

Style characteristics (match Image 2):
- Oil/acrylic painting aesthetic
- VISIBLE brush strokes throughout entire image
- Paint texture clearly visible - looks like real paint
- Vibrant, saturated colors enhanced
- Slightly toy-like color palette
- Post-pop-art aesthetic
- Modern realism meets pop surrealism
- Ironic, whimsical tone

Painting technique:
- Expressive brushwork visible across entire image
- Paint looks like PAINT, not digital filter
- Impasto texture in places (thick paint effect)
- Loose, expressive strokes especially in backgrounds
- Refined but still painterly in main subjects (faces, key elements)
- Traditional painting feel
- Visible canvas texture underneath

COLOR TREATMENT:
- Enhance color saturation significantly
- Make colors more vibrant and juicy
- Bold contrasts between warm kitchen (right) and cool forest (left)
- Rich, thick color application
- Post-pop-art vibrant palette

TECHNIQUE APPLICATION:
- Apply painting effect uniformly across entire composition
- Brushstrokes should be visible but natural
- Paint texture should feel authentic, not digital
- Think: "photo painted over by artist" not "digital filter applied"

CRITICAL BALANCE:
- Chef's face must remain RECOGNIZABLE after painting style
- Don't over-paint to lose person's identity
- Apply style at 70-80% intensity, not 100%
- Main subjects (chef, monster) should keep detail but look painted
- Backgrounds can be looser and more expressive

MOOD: Epic yet ironic, playful yet masterfully executed, contemporary art meets fantasy adventure

FINAL RESULT: The photo composition transformed into contemporary figurative painting with visible brushstrokes, vibrant colors, and painterly texture throughout. Face remains recognizable.
```

### Результат
Финальное изображение: постер с повар + куролиск + название "Куролиск для Paella Valenciana", стилизованный под живопись с видимыми мазками кисти в стиле contemporary figurative painting.

---

## ✅ Чеклист выполнения

**Подготовка:**
- [ ] Открыть Perplexity AI
- [ ] Установить модель Nano Banana в настройках
- [ ] Подготовить свою фотографию (держите паэльеру)
- [ ] Найти и скачать хорошее фото куролиска/кокатриса из интернета
- [ ] Подготовить фото стиля (человек с динозаврами)

**Выполнение:**
- [ ] **ШАГ 1:** Загрузить своё фото → Скопировать промпт → Генерировать → Сохранить результат
- [ ] **ШАГ 2:** Загрузить фото куролиска → Скопировать промпт → Генерировать → Сохранить результат
- [ ] **ШАГ 3:** Загрузить 2 изображения (результаты Шагов 1 и 2) → Скопировать промпт → Генерировать → Сохранить композицию
- [ ] **ШАГ 4:** Загрузить композицию из Шага 3 → Скопировать промпт → Добавить текст → Сохранить постер
- [ ] **ШАГ 5:** Загрузить 2 изображения (результат Шага 4 + фото стиля) → Скопировать промпт → Генерировать финал

**После генерации:**
- [ ] Проверить, что лицо повара узнаваемо
- [ ] Проверить, что композиция выглядит гармонично
- [ ] Проверить, что стиль живописи применён с видимыми мазками
- [ ] При необходимости регенерировать с корректировками

### 💡 Почему 5 шагов?

Разделение на отдельные этапы даёт максимальный контроль:
- **Шаг 3 (композиция):** Сначала создаём чистую фото-композицию с плавным переходом и декоративной рамкой. Если что-то не так с расположением или переходом - можем исправить до добавления текста.
- **Шаг 4 (текст):** Добавляем название модуля в готовую рамку. Если текст плохо читается или расположен неудачно - переделываем только этот шаг.
- **Шаг 5 (стиль):** Применяем живопись к уже готовому постеру с текстом. Если стиль слишком сильный или слабый - можем переделать только этот шаг, не трогая композицию и текст.

Это экономит время и даёт лучший контроль над результатом!

---

## 💡 Важные заметки

### Если на Шаге 1 появляется монстр:
Добавьте в промпт:
```
CRITICAL: Generate ONLY the chef. Do NOT add any monsters, creatures, or fantasy elements. Focus ONLY on chef costume transformation.
```

### Если лицо не сохраняется на Шаге 1:
Добавьте в промпт:
```
PRIORITY #1: Preserve the exact face from uploaded photo. This is photo editing, not person creation.
```

### Если на Шаге 2 монстр перерисовывается (выглядит как уродливый петух):
Убедитесь, что:
1. Вы ЗАГРУЗИЛИ фото куролиска перед генерацией
2. Добавьте в промпт:
```
CRITICAL: Use the UPLOADED creature image. DO NOT generate a new monster. DO NOT draw a chicken or rooster. Take the creature EXACTLY from uploaded photo and only change the background. This is photo compositing task, not creature generation.
```

### Альтернатива для Шага 2 (если всё равно не работает):
Используйте другой подход - попросите только добавить элементы окружения:
```
Add forest environment around the uploaded creature image: trees, forest floor, nest with eggs, forest lighting. Keep the creature exactly as uploaded. Only add background elements.
```

### Если на Шаге 3 композиция получается плохой:
Попробуйте уточнить:
```
Make the transition between two images SMOOTH and SEAMLESS. Blend naturally. The boundary should be visible but not harsh. Magical misty effect in center.
```


### Если текст плохо читается на Шаге 4:
Добавьте в промпт:
```
CRITICAL: Text must be clearly readable with strong contrast. Use bright gold/yellow text on dark frame. Make text LARGER if needed. Readability is priority #1.
```

### Если текст на Шаге 4 расположен неправильно:
Добавьте в промпт:
```
Place text ONLY in the decorative bottom frame. Do NOT overlap the main images. Center text horizontally. Keep good spacing from frame edges.
```

### Если кириллица не отображается правильно на Шаге 4:
Попробуйте альтернативный вариант:
```
Use Cyrillic font that supports Russian letters. The word "КУРОЛИСК" must render correctly in Cyrillic alphabet. If needed, use clear sans-serif or decorative Cyrillic font.
```

### Если стиль слишком сильный на Шаге 5 (лицо или текст теряются):
Добавьте в промпт:
```
Apply painting style GENTLY at 70% intensity. Face recognition and text readability are priority #1. Don't over-paint. Chef's face and title text must stay recognizable and readable.
```

### Если стиль недостаточно выражен на Шаге 5:
Добавьте в промпт:
```
Make brushstrokes MORE VISIBLE. Increase paint texture. The result should clearly look like a PAINTING, not a photo with slight filter. Bold, expressive brushwork.
```

---

*Создано: 2026-01-23*
*Инструмент: Perplexity AI с Nano Banana / FLUX.1*
