# AeHubTools — панель и скрипты для Adobe After Effects

**AeHubTools** (also known as *animation_script*) is a CEP extension panel for **Adobe After Effects**: motion tools, null rigs, project organization, text utilities, and reusable composition templates.  
**Русский:** расширение CEP / панель AeHubTools для **After Effects** — набор скриптов и инструментов для анимации, нулевых объектов, сортировки проекта, текста и библиотеки композиций.

**Latest release:** [v1.4.5](https://github.com/mujlax/AeHubTools/releases/latest) · **Последняя версия:** 1.4.5

---

## Что это

AeHubTools — это **CEP-панель** (Common Extensibility Platform) для After Effects 2020+.  
Инструменты собраны на **настраиваемой сетке**: вы добавляете нужные кнопки, сохраняете пресеты раскладки, работаете на **macOS и Windows**.

Панель не заменяет стандартные скрипты File → Scripts — это **постоянно доступная панель** `Window → Extensions → AeHubTools` с ExtendScript/JSX backend и современным UI.

**Ключевые слова для поиска:** After Effects script, AE panel, CEP extension, motion graphics tools, keyframe tools, null object, precomp library, project organizer, ease in out, snap to frames, derusify, русские названия в AE.

---

## Скачивание и установка

1. Откройте [Releases](https://github.com/mujlax/AeHubTools/releases) и скачайте `animation_script_X.Y.Z.zip`.
2. Распакуйте архив в отдельную папку.
3. **Закройте After Effects.**
4. Запустите установщик из архива:
   - **Windows:** `Install-Windows.cmd`
   - **macOS:** `Install-macOS.command`
5. Откройте AE → **Window → Extensions → AeHubTools** (Окно → Расширения → AeHubTools).

Подробности — в файле `INSTALL.txt` внутри архива.

**Папка расширения после установки:**

| OS | Path |
|---|---|
| Windows | `%APPDATA%\Adobe\CEP\extensions\animation_script\` |
| macOS | `~/Library/Application Support/Adobe/CEP/extensions/animation_script/` |

Обновление: запустите установщик из нового ZIP — старая версия будет заменена автоматически.

---

## Инструменты и функции

### Организация проекта

| Инструмент | Назначение |
|---|---|
| **Библиотека композиций** | Сохранение comp с превью, исходниками и proxy; повторная вставка в другие проекты; выбор кадра превью |
| **Умная сортировка** | Правила, regex, автоматическая структура папок в Project |
| **Сортировка по папкам** | Audio, Video, Pic, Seq, Solids |
| **Структура папок** | Mat / Render / Guides и подпапки |
| **Распаковать прекомп** | Развернуть precomp в текущую композицию |
| **Переименовать компы** | Batch rename выбранных compositions |
| **Поиск текста** | Поиск text layers по проекту |
| **Заметки** | Заметки к проекту |
| **Проверка проекта** | Cyrillic, unused footage, структура, текст |

### Null, иерархия, rig

| Инструмент | Назначение |
|---|---|
| **Группа нулей** | Null для выделенных слоёв |
| **Root Null Scale** | Масштаб через root null |
| **Иерархия нулей / композиции** | Дерево parent links |
| **Масштаб по расстоянию** | Distance scale null |
| **Responsive Box** | Адаптивный rect + null rig |
| **Null в точку Rect** | Привязка null к углу shape |
| **Scatter Comp** | Разброс экземпляров comp |
| **TEMP Wrapper** | Временная обёртка comp для правок |

### Анимация и ключи

| Инструмент | Назначение |
|---|---|
| **Временная интерполация** | Ease In / Ease Out для keyframes |
| **Копирование/вставка Ease** | Copy/paste easing между ключами |
| **Snap Keyframes** | Привязка ключей к кадрам (frame snap) |
| **Timeline Skew** | Сдвиг ключей и слоёв по цепочкам |
| **Time Reverse** | Реверс keyframes по времени |
| **Якорная точка** | Reposition anchor point |
| **Привязка формы** | Sticky shape expressions |
| **Custom Expressions** | Библиотека пользовательских expressions |
| **Random 3D Comps** | Случайные 3D композиции |

### Размер, shape, media

| Инструмент | Назначение |
|---|---|
| **Поиск размера комп** | Comp Size Finder, duplicate & resize |
| **Подгонка формы под comp** | Fit to comp scale |
| **Размер слоя %** | Layer size in percent |
| **Split/Merge Shapes** | Разделение и слияние shape layers |
| **Дублировать маску** | Duplicate layer as mask |
| **Из буфера** | Paste image / SVG from clipboard |
| **Гайд + Lock** | Guide layers at 50% opacity |

### Текст и локализация

| Инструмент | Назначение |
|---|---|
| **Текст в settings** | Link text to settings comp |
| **Высота символа** | Text char height metrics |
| **Дерусификация** | Transliterate RU layer/asset names |
| **Проверка RU** | Audit Cyrillic names in project |
| **Подготовка к ТГ стикерам** | Rename for sticker export |

---

## Системные требования

- Adobe After Effects **2020+** (AEFT, CEP 7+)
- **macOS 10.14+** или **Windows 10+**
- Для неподписанной CEP-панели может потребоваться **PlayerDebugMode** (см. INSTALL.txt)

---

## История версий

Актуальный список релизов и changelog — в [Releases](https://github.com/mujlax/AeHubTools/releases) и в файле [`versions.json`](versions.json) (используется встроенным обновлением панели).

### v1.4.5 (2026-09-11)

- Библиотека композиций с превью, исходниками и повторной вставкой
- Выбор кадра превью при сохранении
- Исправления упаковки sequences/proxy и путей на Windows
- Корректный Undo при добавлении из библиотеки

---

## Для кого этот репозиторий

Этот GitHub-репозиторий — **канал распространения** готовых сборок AeHubTools (ZIP + `versions.json`).  
Исходный код разрабатывается отдельно; здесь публикуются только релизы для установки через панель обновлений.

---

## Поиск и теги

`After Effects` · `Adobe AE` · `CEP` · `ExtendScript` · `JSX` · `motion graphics` · `mograph` · `keyframes` · `ease` · `null object` · `precomp` · `composition library` · `project manager` · `script panel` · `AE tools` · `анимация` · `After Effects скрипт` · `панель After Effects` · `нулевой объект` · `ключевые кадры` · `сортировка проекта` · `библиотека композиций`

---

**AeHubTools** — ускорение рутины в After Effects: от ease и snap до библиотеки готовых comp.
