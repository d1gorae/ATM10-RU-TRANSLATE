# Перевод FTB Quests для ATM10

Эта часть локализации относится к заданиям сборки и **не является обычным ресурс-паком**. Файлы имеют формат SNBT, а не JSON.

## Структура

- `ru_ru/chapter.snbt` — названия глав и подзаголовки.
- `ru_ru/reward_table.snbt` — названия таблиц наград.
- `ru_ru/chapters/*.snbt` — переводы описаний и названий заданий отдельных глав.

## Установка для проверки

1. Закройте Minecraft и лаунчер сборки.
2. Откройте папку экземпляра ATM10, где находятся `mods`, `config` и `saves`.
3. Перейдите в `config/ftbquests/quests/lang/ru_ru/`.
4. Скопируйте туда файлы из каталога `ru_ru` этого проекта, сохраняя имена файлов.
5. Перед заменой собственных файлов сделайте резервную копию.

Путь и формат зависят от версии FTB Quests и конкретной сборки. Перед установкой нужно проверить структуру каталога в используемой версии мода.

## Состояние источников

В актуальном английском источнике ATM10 найдено **67 файлов глав**. В этом репозитории также присутствуют **67 русских файлов** с теми же именами; отсутствующих и лишних файлов на уровне списка нет.

## Проверка перевода — 05.11.2026

Полностью сверены первые 10 глав:

- `achapter_2r_6the_atm_star` — 77 EN-ключей, 79 RU-записей; два дополнительных RU-поля относятся к существующим quest ID в базовом SNBT.
- `aether` — 161/161.
- `allthemodium` — 116/116.
- `apotheosis_2` — 67/67.
- `apotheosis_gear` — 65/65.
- `apothic_enchanting` — 136 EN-ключей, 137 RU-записей; одно дополнительное RU-поле относится к существующему quest ID в базовом SNBT.
- `applied_energistics_2` — 175/175.
- `ars_nouveau` — 76 EN-ключей, 77 RU-записей; одно дополнительное RU-поле относится к существующему quest ID в базовом SNBT.
- `artifacts` — 149/149.
- `auroral` — 46/46.

Итого: 1068 EN-ключей и 1072 RU-записи. Пропущенных EN-ключей нет; четыре дополнительные RU-записи сохранены только потому, что соответствующие quest ID присутствуют в базовых файлах глав. Удалено 15 устаревших записей, ссылавшихся на отсутствующие в текущих базовых главах ID.

Во всех 10 файлах: дубликаты ключей 0, несоответствия плейсхолдеров 0, расхождения ссылок на изображения 0, SNBT-структура сбалансирована. В главе ATM Star исправлены два устаревших описания мультиблочных структур и повреждённые кавычки вокруг двух изображений.

**Ограничения:** проверка структуры не заменяет запуск FTB Quests в игре. Остаются 47 глав, общие `chapter.snbt` и `reward_table.snbt`, а также глобальные языковые файлы. FTB Quests не завершён и не готов к релизу.

## Следующая партия глав

`basic_armor`, `basic_logistics`, `basic_power`, `basic_tools`, `bounty_board`, `building_tips`, `bumblezone`, `cataclysm`, `chapter_2_the_star`, `create`.


## Вторая партия проверки — 05.11.2026

Проверены следующие 10 глав: `basic_armor`, `basic_logistics`, `basic_power`, `basic_tools`, `bounty_board`, `building_tips`, `bumblezone`, `cataclysm`, `chapter_2_the_star`, `create`.

| Глава | EN-ключи | RU-записи | Дополнительные RU-поля |
|---|---:|---:|---:|
| `basic_armor` | 347 | 347 | 0 |
| `basic_logistics` | 76 | 87 | 11 |
| `basic_power` | 96 | 96 | 0 |
| `basic_tools` | 110 | 110 | 0 |
| `bounty_board` | 54 | 54 | 0 |
| `building_tips` | 255 | 255 | 0 |
| `bumblezone` | 189 | 192 | 3 |
| `cataclysm` | 230 | 230 | 0 |
| `chapter_2_the_star` | 246 | 262 | 16 |
| `create` | 190 | 190 | 0 |
| **Итого** | **1793** | **1823** | **30** |

Все 30 дополнительных RU-полей относятся к quest ID, присутствующим в базовых SNBT-файлах, поэтому сохранены как дополнительные локализованные поля. Удалено 14 устаревших записей с ID, отсутствующими в актуальных базовых главах. Пропущенных EN-ключей нет; дубликаты 0, несоответствия плейсхолдеров 0, расхождения ссылок на изображения 0, все файлы имеют сбалансированную SNBT-структуру.

Итого проверено 40 из 67 глав; осталось 27. Следующая партия: `create_addons`, `deeper_and_darker`, `draconic_evolution`, `elmystical_agriculturerr`, `eternal_starlight`, `evilcraft`, `extended__advanced_ae`, `extreme_reactors`, `food_and_farming`, `forbidden__arcanus`.


## Третья партия проверки — 05.11.2026

Проверены главы: `create_addons`, `deeper_and_darker`, `draconic_evolution`, `elmystical_agriculturerr`, `eternal_starlight`, `evilcraft`, `extended__advanced_ae`, `extreme_reactors`, `food_and_farming`, `forbidden__arcanus`.

| Глава | EN-ключи | RU-записи | Дополнительные RU-поля |
|---|---:|---:|---:|
| `create_addons` | 112 | 114 | 2 |
| `deeper_and_darker` | 91 | 91 | 0 |
| `draconic_evolution` | 254 | 254 | 0 |
| `elmystical_agriculturerr` | 267 | 272 | 5 |
| `eternal_starlight` | 299 | 299 | 0 |
| `evilcraft` | 78 | 94 | 16 |
| `extended__advanced_ae` | 91 | 91 | 0 |
| `extreme_reactors` | 70 | 70 | 0 |
| `food_and_farming` | 92 | 92 | 0 |
| `forbidden__arcanus` | 123 | 124 | 1 |
| **Итого** | **1477** | **1501** | **24** |

Все 24 дополнительных RU-поля относятся к существующим quest ID в базовых SNBT-файлах. Удалено 20 устаревших записей с отсутствующими ID. Пропусков EN-ключей нет; дубликаты 0, несоответствия плейсхолдеров 0, расхождения ссылок на изображения 0, все 10 файлов имеют сбалансированную SNBT-структуру.

В Deeper and Darker восстановлены две пропущенные иллюстрации и уточнено описание моба. В Mystical Agriculture добавлен отсутствовавший подзаголовок. В Eternal Starlight термины приведены к существующему переводу мода, исправлены устаревшие описания и восстановлены две иллюстрации. В Forbidden Arcanus унифицирован термин «Исток», исправлены грамматика и оставшаяся английская вставка.

Итого проверено 30 из 67 глав; осталось 37. Следующая партия: `generators`, `hostile_neural_networks`, `ice__fire`, `immersive_engineering`, `industrial_foregoing`, `integrated_dynamics`, `iron_spells_and_spellbooks`, `justdirethings`, `mahou_tsukai`, `mainquestline_part_1`.


## Четвёртая партия проверки — 05.11.2026

Проверены главы: `generators`, `hostile_neural_networks`, `ice__fire`, `immersive_engineering`, `industrial_foregoing`, `integrated_dynamics`, `iron_spells_and_spellbooks`, `justdirethings`, `mahou_tsukai`, `mainquestline_part_1`.

| Глава | EN-ключи | RU-записи | Дополнительные RU-поля |
|---|---:|---:|---:|
| `generators` | 95 | 100 | 5 |
| `hostile_neural_networks` | 28 | 29 | 1 |
| `ice__fire` | 173 | 178 | 5 |
| `immersive_engineering` | 245 | 246 | 1 |
| `industrial_foregoing` | 106 | 107 | 1 |
| `integrated_dynamics` | 54 | 54 | 0 |
| `iron_spells_and_spellbooks` | 197 | 197 | 0 |
| `justdirethings` | 164 | 175 | 11 |
| `mahou_tsukai` | 71 | 71 | 0 |
| `mainquestline_part_1` | 87 | 88 | 1 |
| **Итого** | **1220** | **1245** | **25** |

Все 25 дополнительных RU-полей относятся к quest ID, присутствующим в базовых SNBT-файлах. Удалена одна устаревшая запись Mahou Tsukai с отсутствующим ID. Пропусков EN-ключей нет; дубликаты 0, несоответствия плейсхолдеров 0, расхождения ссылок на изображения 0, все 10 файлов имеют сбалансированную SNBT-структуру.

Итого проверено 40 из 67 глав; осталось 27. Следующая партия: `mekanism`, `mekanism_reactors`, `mi_digital`, `mi_electric`, `mi_endgame`, `mi_steam`, `modular_router`, `natures_aura`, `neo_vitae`, `occultism`.
