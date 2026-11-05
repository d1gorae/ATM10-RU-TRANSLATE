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

Итог сверки первых 50 глав: 2861 EN-ключей и 2895 RU-записей. 34 дополнительных RU-полей оставлены, поскольку соответствующие quest ID присутствуют в базовых файлах глав, хотя полей нет в EN overlay. Пропусков EN-ключей нет; 29 устаревших записей с ID, отсутствующими в актуальных базовых файлах, удалены. Дубликаты, ошибки плейсхолдеров и расхождения ссылок на изображения — 0; все 20 SNBT-файлов имеют сбалансированную структуру.

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


## Результаты четвёртой партии FTB Quests — 05.11.2026

Проверены главы: `generators`, `hostile_neural_networks`, `ice__fire`, `immersive_engineering`, `industrial_foregoing`, `integrated_dynamics`, `iron_spells_and_spellbooks`, `justdirethings`, `mahou_tsukai`, `mainquestline_part_1`. EN-ключей 1220, RU-записей 1245, дополнительных полей 25; все дополнительные поля соответствуют существующим quest ID в базовых SNBT. Удалена одна устаревшая запись Mahou Tsukai. Missing 0, duplicates 0, placeholders 0, image-reference mismatches 0, SNBT balance OK.

Коммит очистки Mahou Tsukai: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/02485dfd60e41cdeab21215ef5723005ba3bb782.

Следующая партия: `mekanism`, `mekanism_reactors`, `mi_digital`, `mi_electric`, `mi_endgame`, `mi_steam`, `modular_router`, `natures_aura`, `neo_vitae`, `occultism`. После неё останется 17 глав.


## Результаты пятой партии FTB Quests — 05.11.2026

Проверены главы: `mekanism`, `mekanism_reactors`, `mi_digital`, `mi_electric`, `mi_endgame`, `mi_steam`, `modular_router`, `natures_aura`, `neo_vitae`, `occultism`. EN-ключей 1228, RU-записей 1250, дополнительных полей 22; все дополнительные поля соответствуют существующим quest ID в базовых SNBT. Удалены 4 устаревшие записи Modern Industrialization. Missing 0, duplicates 0, placeholders 0, image-reference mismatches 0, RGB-color mismatches 0, SNBT balance OK.

Исправлены RGB-коды в MI Electric и цветовые обозначения мелков в Occultism. Коммиты: [MI Digital](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9f55f92595705a0a5d311ab7ec37ec589739c9a7), [MI Electric stale cleanup](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0c4617acce6caf62adccb4796edc777c376b808e), [MI Endgame](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/81eefe1a181903d608c9cee9bf4161696a2c9816), [MI Steam](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7dd31f8f204e40f6822c06b670d23df5029e2acc), [MI Electric RGB](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a63131867f9b87477e691ad5e4e86a02a6b8beed), [Occultism RGB](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c6276abfa8e10f3fe43d502d2aa84d632258d9b8).

Следующая партия: `oritech`, `pneumaticcraft`, `powah`, `productive_bees`, `productive_trees`, `pylons`, `railcraft`, `refined_storage`, `relics`, `silent_gear`. После неё останется 7 глав.


## Рабочая сессия 05.11.2026 — продолжение аудита FTB Quests

После завершения пятой партии (50 из 67 глав) начата следующая десятка: `oritech`, `pneumaticcraft`, `powah`, `productive_bees`, `productive_trees`, `pylons`, `railcraft`, `refined_storage`, `relics`, `silent_gear`.

В этой сессии запущена построчная сверка RU-глав с EN-оригиналами и базовыми SNBT, включая проверку ключей и ID, плейсхолдеров, ссылок на изображения и структуры SNBT. Для `oritech` и `relics` отдельно выполнялась проверка устаревших записей по базовым ID; потенциально удалённые записи не считаются завершённой главой без итоговой повторной проверки.

Дополнительно зафиксированы выполненные ранее исправления пятой партии: восстановление RGB-кодов в `mi_electric` и цветовых обозначений в `occultism`, а также удаление устаревших записей Modern Industrialization.

**Статус:** официально подтверждённый прогресс остаётся 50/67 глав. Следующая десятка пока не засчитывается как завершённая партия: перед обновлением счётчика требуется повторно получить сводные результаты всех десяти файлов, проверить каждую правку и записать точные коммиты. Осталось 17 глав по последнему полностью зафиксированному состоянию. Следующая точка продолжения — завершить и перепроверить текущую десятку, затем обработать последние 7 глав.


## Результаты шестой партии FTB Quests — 05.11.2026

Проверены и завершены 10 глав: `oritech`, `pneumaticcraft`, `powah`, `productive_bees`, `productive_trees`, `pylons`, `railcraft`, `refined_storage`, `relics`, `silent_gear`.

Сверка с актуальными EN overlay: **1583 ключа** в английских оригиналах и 1583 в русских файлах. По всем десяти главам: missing 0, extra 0, duplicates 0, placeholder mismatches 0. Проверка баланса кавычек и фигурных/квадратных скобок пройдена для всех 20 файлов.

Дополнительно сверены image ID с базовыми SNBT:
- Удалён устаревший RU image key Productive Trees.
- Удалены 21 устаревший RU image key Railcraft.
- В Relics заменены 10 старых image ID на актуальные ID из базового файла; подписи переведены по соответствующим EN изображениям.
- В Relics исправлены названия Roller Skate и Ring of the Seven Deadly Sins, описание мест появления реликвий и названия измерений.
- В Productive Bees восстановлено предложение о необходимости блоков расширения для поддержки улучшений.
- В Oritech уточнён маршрут получения малой плутониевой пыли; в Railcraft исправлено форматирование описаний раздатчиков.
- В глоссарий добавлены термины Nether, The End, Overworld, Stronghold и Nether Fortress.

Коммиты:
- [Oritech — маршрут плутониевой пыли](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b1e1109d1e33da591524131a5b765c9099c98da6)
- [Railcraft — восстановление форматирования](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8a28034bae042e43514fb1aab3a6f74895c15084)
- [Productive Trees — удаление устаревшего image key](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cf4c98aa880b8c36a3765eb2a90ee04958f7643b)
- [Railcraft — удаление устаревших image keys](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6f8c4db8edb0ba50181691f91c6210fa908b27e3)
- [Relics — исправление названий реликвий](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e6ecc40bfc900d580348e30039201cbeedd36d28)
- [Relics — синхронизация image ID](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/69aa06cbcfac8d5f2a8246daaaeae43e90677b36)
- [Relics — описание мест появления и измерения](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/119c9ff9525d52e94c1e532710433b0530e02af1)
- [Productive Bees — дополнение описания блоков расширения](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4f106b09ed342d41d426c18a1e2a5bc55dbb2c06)
- [Глоссарий — термины измерений и структур](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/231f910182c81a4dc5e52e60fda7b2bb31e171fd)
- [Глоссарий — термины Oritech, Productive Trees и Relics](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5261c98569c2b53cf4d277b001d06f4ac25b03cf)

**Итого подтверждено: 60/67 глав. Осталось 7 глав.** Следующая точка продолжения — последние 7 глав, затем общие `chapter.snbt`, `reward_table.snbt` и глобальные языковые SNBT-файлы. Не считать FTB Quests завершённым до финальной общей проверки.


## Результаты заключительной партии глав FTB Quests — 05.11.2026

Завершены последние 7 глав: `storage`, `theurgy`, `tips_and_tricks`, `twilight_forest`, `undergarden`, `welcome`, `xycraft`.

В английских оригиналах — **654 ключа**, в русских файлах — 654. Проверки: missing 0, extra 0, duplicates 0, placeholder mismatches 0, пустых переводов 0. Для всех 14 overlay-файлов проверены кавычки и баланс скобок; расхождений по двойному экранированию переносов строк не осталось.

Исправления:
- `storage`: заполнено пустое описание фильтра рюкзака.
- `tips_and_tricks`: восстановлена информация о подключении Building Gadgets к сети AE2; исправлено экранирование переносов строк и цвет Steam Drill.
- `twilight_forest`: исправлено двойное экранирование переносов строк.
- `undergarden`: восстановлено полное описание получения кристалла утерита, исправлены названия/форматирование отдельных существ и нормализованы переносы строк.
- `welcome`: удалена посторонняя рекламная вставка, отсутствующая в английском оригинале; естественнее переведено описание kitchen-sink pack.
- В глоссарий добавлены термины The Undergarden, включая Utheric, Rogdorium, Rot, Depths, Dreadrock, Gronglet, Stoneborn и Denizen.
- `theurgy` и `xycraft` прошли сверку без необходимости менять текст.

Коммиты:
- [Storage — заполнить описание фильтра](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c3bbb96f3d6a337ebbbf2e58816980fe4a7d5f29)
- [Tips and Tricks — восстановить описание AE2 и исправить переносы](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8d7f7d08eeed9d0981bce112cb5f406b82d91f33)
- [Tips and Tricks — сохранить цвет Steam Drill](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f8b57468af203020e8d5c101fa58b93d991e63a0)
- [Twilight Forest — исправить экранирование](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/532c8f2515858c950392aa929d7c115f587c7da7)
- [Undergarden — восстановить описание утеритового кристалла](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/be50d9ec1a60f8bdc65c5977b7067a81e08c6707)
- [Undergarden — исправить Gronglet](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2f28c3dc8cbcf1f3882089843c22dbe2c1831e6a)
- [Undergarden — сохранить цвет Stoneborn и Mog](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/959ce011e4063e945cd26137cd3453aa595145ea)
- [Welcome — исправить вступительное описание](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ea8d0ec8f2b8a2625d6cff232817b87fa3cc77a3)
- [Глоссарий — термины The Undergarden](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/769924f8cded0a6adc3265f1fa0e4175b94a0c9b)

**Итого: все 67/67 глав FTB Quests сверены с EN overlay.** Суммарно по 67 главам — 10 816 EN-ключей. Это не означает завершение всего FTB Quests: остаются общие `chapter.snbt`, `reward_table.snbt` и глобальные языковые SNBT-файлы. Их проверка — следующая точка продолжения.
