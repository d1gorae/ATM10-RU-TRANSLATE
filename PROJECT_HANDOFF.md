# PROJECT HANDOFF — ATM10 RU TRANSLATE

Обновлено: **05.11.2026**

## Проект

Полная русская локализация All the Mods 10 для Minecraft 1.21.1 / NeoForge.

- Репозиторий переводов: https://github.com/d1gorae/ATM10-RU-TRANSLATE
- Английские источники (только чтение): https://github.com/d1gorae/beamng-road-reference/tree/main/ATM/LANGUAGES_EN_US

## Правила продолжения

- Работать партиями по 10 модов; каждый перевод полностью сверять, проверять и публиковать до перехода дальше.
- Не повторять качественные существующие переводы и не затирать их без причины.
- Английские источники не изменять; Dropbox не изменять и ничего из него не удалять.
- Использовать `GLOSSARY.md`; сохранять бренды, API, идентификаторы и специальные обозначения.
- Проверять ключи, дубликаты, плейсхолдеры, форматирование, переносы строк, специальные символы и корректность JSON/SNBT.
- Не объявлять партию завершённой, если фактически не завершено 10 модов. FTB Quests/SNBT — финальный этап.
- После каждой партии обновлять этот файл и `INVENTORY.md` только фактическими результатами.

## Последние опубликованные переводы

- **Chipped** — 7265/7265 ключей, missing 0, extra 0, placeholders 0, formatting 0. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3d2ddac65d0dd725f1b8f31420f1680d58bf9bde
- **Rechiseled** — 3656/3656 ключей, missing 0, extra 0, duplicates 0, placeholders 0, formatting 0. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/02cb14fd9d433fbe8dd04f2c1bea8c78af669997
- Глоссарий Rechiseled: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4638e866d1b3c0fa9c644af6fa4ae6e339011ba4

## Проверка дополнительных namespace

Все 13 дополнительных namespace из соответствующего раздела `INVENTORY.md` сверены с английскими оригиналами. Проверки структуры, ключей, плейсхолдеров и форматирования пройдены. Также проверены четыре файла YUNG's Better: Desert Temples, Dungeons, End Island и Jungle Temples. В Better Dungeons исправлено обращение на единый вежливый стиль. Подробные количества ключей и результаты находятся в `INVENTORY.md`.

Следующие позиции без прямого языкового namespace проверены по полному дереву английских источников: для них отдельные `en_us.json` не найдены; это не доказывает отсутствия строк внутри JAR, поэтому при появлении оригиналов нужна повторная проверка.

## FTB Quests / SNBT — финальный этап

В источнике английских оригиналов найдено 67 файлов в `ATM/FTBQUESTS/en_us/chapters/`; в переводном репозитории присутствуют соответствующие 67 файлов в `FTBQUESTS/ru_ru/chapters/`. Имена файлов совпадают.

### Проверено

Первые 10 глав:

1. `achapter_2r_6the_atm_star`
2. `aether`
3. `allthemodium`
4. `apotheosis_2`
5. `apotheosis_gear`
6. `apothic_enchanting`
7. `applied_energistics_2`
8. `ars_nouveau`
9. `artifacts`
10. `auroral`

Итог сверки первых 30 глав: 2861 EN-ключей и 2895 RU-записей. 34 дополнительных RU-полей оставлены, поскольку соответствующие quest ID присутствуют в базовых файлах глав, хотя полей нет в EN overlay. Пропусков EN-ключей нет; 29 устаревших записей с ID, отсутствующими в актуальных базовых файлах, удалены. Дубликаты, ошибки плейсхолдеров и расхождения ссылок на изображения — 0; все 20 SNBT-файлов имеют сбалансированную структуру.

Исправлены два устаревших описания мультиблочных квестов ATM Star и кавычки вокруг двух изображений. Основной файл: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6ff343e1b59c02a6baff3d2a24efc3c6ca11f968

### Следующая точка продолжения

Следующие 10 глав по алфавиту:

1. `create_addons`
2. `deeper_and_darker`
3. `draconic_evolution`
4. `elmystical_agriculturerr`
5. `eternal_starlight`
6. `evilcraft`
7. `extended__advanced_ae`
8. `extreme_reactors`
9. `food_and_farming`
10. `forbidden__arcanus`

После них продолжить следующие главы партиями по 10. Затем сверить общие `chapter.snbt` и `reward_table.snbt`, а также проверить глобальные языковые файлы. Не считать FTB Quests завершённым до проверки всех 67 глав и общих файлов.

FTB Quests и SNBT остаются последним этапом проекта.


## Результаты второй партии FTB Quests — 05.11.2026

Проверены главы: `basic_armor`, `basic_logistics`, `basic_power`, `basic_tools`, `bounty_board`, `building_tips`, `bumblezone`, `cataclysm`, `chapter_2_the_star`, `create`. EN-ключей 1793, RU-записей 1823, дополнительных полей 30. Все дополнительные поля относятся к существующим quest ID в базовых SNBT и сохранены. Удалено 14 устаревших записей, ссылавшихся на отсутствующие ID. Missing 0, duplicates 0, placeholders 0, image-reference mismatches 0, SNBT balance OK.

Коммиты очистки устаревших ключей: [basic_power](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bacb6eb774d68ec16cad766d858a9e6abb24d5fd), [basic_tools](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6d681feb92e3e38069efe28cf6c3dcfe6ce8a820), [bounty_board](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3952593ced937c8badecd8beb391f024e43deb6f), [chapter_2_the_star](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7d11b485d15ad932f517ec57de8b0d623317def6), [create](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/45c5ff1a75ba4e2727585964aca9c64c811fa7f7).


## Результаты третьей партии FTB Quests — 05.11.2026

Проверены главы: `create_addons`, `deeper_and_darker`, `draconic_evolution`, `elmystical_agriculturerr`, `eternal_starlight`, `evilcraft`, `extended__advanced_ae`, `extreme_reactors`, `food_and_farming`, `forbidden__arcanus`. EN-ключей 1477, RU-записей 1501, дополнительных полей 24; все дополнительные поля соответствуют quest ID из базовых SNBT. Удалено 20 устаревших записей. Missing 0, duplicates 0, placeholders 0, image-reference mismatches 0, SNBT balance OK.

Обновлены описания и терминология в Deeper and Darker, Mystical Agriculture, Eternal Starlight и Forbidden Arcanus. Глоссарий дополнен терминами Eternal Starlight и Ars Nouveau: [коммит d148b88](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d148b884508986a413402a2788f43a6fcead64d8).

Следующая партия: `generators`, `hostile_neural_networks`, `ice__fire`, `immersive_engineering`, `industrial_foregoing`, `integrated_dynamics`, `iron_spells_and_spellbooks`, `justdirethings`, `mahou_tsukai`, `mainquestline_part_1`. После неё останется 27 глав.
