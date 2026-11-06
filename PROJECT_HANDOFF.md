# PROJECT HANDOFF — ATM10 RU TRANSLATE

Обновлено: **06.11.2026**

## Проект

Полная русская локализация All the Mods 10 для Minecraft 1.21.1 / NeoForge.

- Репозиторий переводов: https://github.com/d1gorae/ATM10-RU-TRANSLATE
- Английские источники (только чтение): https://github.com/d1gorae/beamng-road-reference/tree/main/ATM/LANGUAGES_EN_US


## Сведение рабочих веток в main — 06.11.2026

Основная рабочая ветка `work/irons-spells-nov05` объединена в `main` через [PR #5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/pull/5). Перенесены все её 254 коммита поверх прежнего `main`, включая переводы, 25 партий JSON-аудита, `GLOSSARY.md`, `INVENTORY.md` и историю работы. Merge commit: [126db7b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/126db7b92aad3a9051427a565ff3e37517169dee).

Дополнительно заполнен ранее пустой файл `assets/bibliocraft/lang/ru_ru.json` содержимым из `work/bibliocraft-ru`: 2 021 ключ. В INVENTORY уже зафиксировано полное покрытие BiblioCraft base 2021/2021; после переноса файл присутствует в `main`. Коммит: [d4ac036](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d4ac0366b5dffe245c83506f350d3cef52575865).

Остальные старые ветки сверены по затронутым переводным файлам: Aether, Chisel, Dyenamics and Friends, Logistics Networks, Pam's HarvestCraft Food Extended и Chipped совпадают с файлами `main`; в ветке Mekanism Tools обнаружено одно пустое значение вместо непустого значения в `main`, поэтому её версия не переносилась. В `work/chipped-ru-ru` находятся временные файлы-разбиения, а итоговый Chipped JSON уже совпадает с `main`; временные части не добавлялись.

Ветка `work/atm10-batch-nov05` не объединялась поверх основной: в пяти общих JSON-файлах совпадают все наборы ключей и их количество, но есть 638 различий значений. Это альтернативные формулировки, а не недостающие ключи; автоматическое слияние перезаписало бы более поздние версии из основной рабочей ветки. Эту ветку сохранить как источник для точечной сверки при полировке, не сливать целиком.

**Текущая основная точка работы — `main`.** Следующая партия аудита остаётся прежней: `simplemagnets`, `simple_weather`, `simplylight`, `smithingtemplateviewer`, `solcarrot`, `sophisticatedbackpacks`, `sophisticatedcore`, `sophisticatedstorageinmotion`, `soulplied_energistics`, `starbunclemania`. Перед обработкой сверить их актуальные EN/RU файлы непосредственно в `main`.


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

## FTB Quests / SNBT — финальный этап (завершён; ниже сохранена история партий)

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

### План на момент первоначальной записи (исторический)

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

Этот план был актуален на момент первоначальной записи. Фактическое завершение всех 67 глав и общих файлов зафиксировано в итоговом разделе ниже.

FTB Quests и SNBT были последним этапом проекта; этап завершён, см. итоговую проверку ниже.


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

**Промежуточный результат на момент записи: 60/67 глав.** Затем проверены последние 7 глав и общие файлы; итог зафиксирован ниже.


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

**Промежуточный итог: все 67/67 глав сверены с EN overlay; 10 816 EN-ключей.** Общие файлы и глобальные языковые SNBT проверены отдельно в следующем разделе.


## Итоговая проверка общих файлов FTB Quests — 05.11.2026

- `chapter.snbt`: 78 EN / 78 RU ключей, missing 0, extra 0, duplicates 0, пустых значений 0. Три устаревших RU-only ключа удалены после поиска по всем 67 актуальным базовым файлам глав: соответствующие ID в них не найдены.
- `reward_table.snbt`: 51 EN / 51 RU ключ, missing 0, extra 0, duplicates 0, пустых значений 0. Переведены все пользовательские описательные части названий; бренды и технические обозначения сохранены.
- `chapter_group.snbt`: добавлен в переводной репозиторий; 13 EN / 13 RU ключей, missing 0, extra 0, duplicates 0.
- `file.snbt`: EN и RU-эталон содержат одинаковое название `All The Mods 10`; перевод не требуется.
- `ATM/FTBQUESTS/lang/en_us.snbt` и `lang/ru_ru.snbt` в источнике пустые (0 байт); переводимых строк нет.
- В глоссарий добавлены термины Powah и наград Mystical Agriculture.

Коммиты общих файлов:
- [chapter.snbt — перевести названия глав](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4d5fbba7ffa9b9429f97f0e8e5b1a88bc685d39f)
- [chapter.snbt — удалить устаревшие RU-only ID](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9c759e281930e098ec601a9ede6aaa3040ed9c32)
- [reward_table.snbt — перевести названия таблиц наград](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/780f1a639531bbe5b9c45675ea081f5e160610d4)
- [chapter_group.snbt — добавить русские названия групп](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a17c07a21188051a41fc9c849653e7ab3d6f7ed2)
- [Глоссарий — термины наград Powah и Mystical Agriculture](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bcb66aab106c7146e5ef83ee8d4f873187884546)

**FTB Quests/SNBT: файловая локализация завершена.** Проверены все 67 глав, `chapter.snbt`, `reward_table.snbt`, `chapter_group.snbt`, а также пустые глобальные языковые файлы. Ключи, плейсхолдеры, баланс кавычек/скобок и переносы строк проверены. Полноценный запуск сборки и внутриигровая проверка не проводились.

Следующая точка проекта — финальный аудит всего репозитория локализаций и сверка оставшихся namespace без одноимённого JSON с актуальными EN-источниками; не повторять уже закрытые переводы.


## Продолжение после заключительного аудита — 05.11.2026

Проверено текущее состояние GitHub после завершения FTB Quests/SNBT. Английский репозиторий остаётся только источником чтения; последний найденный коммит в нём датирован 02.11.2026. В переводном репозитории после завершения FTB Quests опубликованы дополнительные исправления:

- Create: Dragons Plus — 356/356 ключей. При повторной сверке найден один RU-only ключ `create_dragons_plus.fragile_fluid_tank.effect.infused_dragon_breath`; удалён. После исправления missing 0, extra 0, placeholder mismatches 0, empty values 0. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3a92c07d5c00d3a1ddd1d4c0272a17854ebf814d
- Sophisticated Storage — 425/425 ключей по актуальному EN-файлу, missing 0, extra 0, placeholder mismatches 0, empty values 0. Уточнение: актуальный файл содержит 425 ключей, а не 169.
- Mekanism Generators — 364/364 ключа, missing 0, extra 0. Сравнение плейсхолдеров не выявило реальных расхождений: знак процента в «100%» является обычным текстом, а не форматным параметром. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/513a0091918e9bfe9d232c1ea9d17bbabd61be3a
- Для Create: Dragons Plus и Sophisticated Storage подтверждены ранее опубликованные коммиты: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4d3541aaadf1799e82d11fed3413ff1b1be5ba52 и https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bc6146f25798f4a2102caf1bcfb257caf573e91f
- Три новых названия Allthemodium опубликованы: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/84ed22ff1846a0a3669e4be152e45fac0448d38d

### Подтверждённые неполные JSON-переводы

Сверка выполнена по фактическим файлам актуальной ветки `main` английского репозитория и соответствующим RU JSON в переводном репозитории:

| Мод | EN ключей | RU ключей | Отсутствует |
|---|---:|---:|---:|
| NeoVitae | 3652 | 256 | 3396 |
| Mekanism | 3239 | 1605 | 1634 |
| Ice and Fire | 1809 | 1193 | 616 |
| Mekanism Tools | 800 | 185 | 615 |
| Silent Gear | 1191 | 616 | 575 |
| Supplementaries | 1394 | 708 | 686 |
| Regions Unexplored | 933 | 455 | 478 |
| **Итого** | **13018** | **5018** | **8000** |

Во всех семи файлах лишних RU-ключей, пустых переводов и обнаруженных расхождений плейсхолдеров нет. Это не означает, что переводы завершены: перечисленные 8000 EN-ключей отсутствуют в RU JSON и требуют перевода.

**Следующая точка продолжения:** начать с NeoVitae, затем последовательно исправлять остальные шесть файлов. Не объявлять партию из 10 модов завершённой, пока фактически не будут завершены и проверены 10 модов; после закрытия этих семи определить следующие три незавершённые позиции по актуальному репозиторию. FTB Quests/SNBT повторно не обрабатывать.


### Дополнительная сверка с Dropbox — 05.11.2026

Dropbox использован только для чтения; файлы в нём не изменялись. Сравнение показало, что его копии в основном не закрывают текущие пропуски: часть ключей устарела, а некоторые значения имеют ошибки плейсхолдеров. Безусловно переносить весь файл нельзя.

В GitHub восстановлены только пять отсутствующих в RU-репозитории ключей, которые присутствуют в актуальном EN и имеют подходящий перевод с корректными плейсхолдерами:
- Mekanism — 3 ключа: служебный `_mekanism_force_utf8` и два описания механизмов. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/83b65e92f5fce0076f3a36ffc67d18713502be86
- Ice and Fire — 1 описание модификатора. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/88e319986aa1cf1244b722cf84274e9e38ec0124
- Silent Gear — 1 описание особенности. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2441db78ecd100ac81b40d92f4f1522109f72a56

Не перенесены:
- Mekanism `multiblock.mekanism.invalid_inner`: в Dropbox отсутствует плейсхолдер `%2$s`.
- Silent Gear: устаревшие ключи, а также значения с неправильными плейсхолдерами (`%d` вместо `%s`, отсутствующие параметры).
- Supplementaries: найденные Dropbox-значения для `item.supplementaries.bamboo_spikes_tipped.effect` и `message.supplementaries.cannon.maneuver` не сохраняют параметры EN.
- Ключи Dropbox, отсутствующие в актуальном EN, не импортировались.

### Актуальный остаток после восстановления пяти ключей

| Мод | EN | RU | Missing |
|---|---:|---:|---:|
| NeoVitae | 3652 | 256 | 3396 |
| Mekanism | 3239 | 1608 | 1631 |
| Ice and Fire | 1809 | 1194 | 615 |
| Mekanism Tools | 800 | 185 | 615 |
| Silent Gear | 1191 | 617 | 574 |
| Supplementaries | 1394 | 708 | 686 |
| Regions Unexplored | 933 | 455 | 478 |
| **Итого** | **13018** | **5023** | **7995** |

Повторная проверка всех семи файлов после изменений: extra 0, empty 0, placeholder mismatches 0. Ни один из семи переводов пока не считается завершённым.


## Последняя выполненная работа: аудит 108 модов без одноимённого RU JSON (05.11.2026)

Подготовлен и опубликован [NO_RU_JSON_AUDIT.md](NO_RU_JSON_AUDIT.md), синхронизирован раздел в INVENTORY.md.

Подтверждённый результат:
- Проверены все 108 mod ID из актуального INVENTORY и сопоставлены с JAR из официального modlist.
- 89 JAR из английской выгрузки не содержат извлечённого en_us.json.
- 5 найденных en_us.json пустые.
- ATM: Compat (10 ключей), Borderless Window (21) и Cloth Config (49) полностью покрыты уже существующими RU-файлами.
- FTB Quests (774 EN-ключа) не трогать до финального этапа проекта.
- Из 10 JAR, отсутствующих в исходной английской выгрузке, отдельно найдены upstream-языковые файлы у Bibliobiomes, Bibliowoods, Iris, IrisSearch, Sodium и Sodium Extra. Эти шесть модов остаются в очереди локализации.
- Colorwheel, Colorwheel Patcher, ImmediatelyFast и Uranus не требуют отдельного RU JSON по найденным ресурсам и назначению.

Важное ограничение: у Bibliobiomes/Bibliowoods текущие upstream-файлы дают предварительно 6 594 ключа, из которых 5 495 уже есть в общем `assets/bibliocraft/lang/ru_ru.json`, а 1 099 отсутствуют. До внесения изменений необходимо сверить эти ключи с точными JAR ATM10 (`bibliobiomes 1.6.1`, `bibliowoods 1.6.2`), поскольку текущие upstream-файлы могут быть новее установленных версий.

Следующая точка продолжения: получить точные English language resources из установленных версий шести модов, проверить покрытие Bibliocraft и затем перевести только реально отсутствующие ключи. Не создавать пустые JSON для модов, у которых нет пользовательских языковых строк. FTB Quests/SNBT оставить на самый конец.


## Последняя выполненная работа: завершение аудита 108 модов (05.11.2026)

После аудита локализованы все шесть модов, у которых обнаружились пользовательские языковые ресурсы:

- Bibliobiomes Legacy 1.6.1 — 9 577 ключей, полностью покрыты общим namespace `bibliocraft`.
- Bibliowoods Legacy 1.6.2 — 10 833 ключа, полностью покрыты общим namespace `bibliocraft`; добавлены 157 отсутствовавших переводов Mauve.
- Iris 1.8.14-beta.1 — 73/73 ключа; отдельный `assets/iris/lang/ru_ru.json`.
- IrisSearch 1.8.4 — 13/13 ключей; отдельный `assets/iris_search/lang/ru_ru.json`.
- Sodium 0.8.13 — 89/89 ключей; отдельный `assets/sodium/lang/ru_ru.json`.
- Sodium Extra 0.9.5 — 418/418 ключей; отдельный `assets/sodium-extra/lang/ru_ru.json`.

В четырёх отдельных файлах проверены точные ключи, отсутствие лишних/пустых значений и плейсхолдеры. В Sodium Extra исправлены три значения с потерянными `%s`, добавлены 38 недостающих переводов и удалены два устаревших ключа. В Iris добавлены недостающие переводы и удалены два лишних ключа. Для Biblio использован общий namespace, без создания лишних JSON.

Документация обновлена: `NO_RU_JSON_AUDIT.md`, `INVENTORY.md`, `GLOSSARY.md`, `README.md`. В инвентаризации: 399 RU JSON, 385 mod ID с одноимённым namespace, 105 без одноимённого JSON; 14 дополнительных namespace. Аудит 108 кандидатов закрыт; шесть модов локализованы, оставшиеся классифицированы как не требующие отдельного перевода или отложенные по правилам проекта.

Коммиты переводов:
- IrisSearch: `019d036c48a47e02bf2fb8cf42e9086e846c2b1f`
- Iris: `bffc2f0f74d0b7c8e21d3feab07278ce1a7dbd58`, затем синхронизация ключей `48b9fd53618da18c4f3e85fe9dc8306752a37518`
- Sodium: `f3242d9cade7069a592ed3cd0f205cbff7415fdf`
- Sodium Extra: `d3fe03c933e32030310cf8931b10360b79e4c3a1`
- Bibliocraft/Mauve: `b475976d16ac51bde7fc782326f490c7d60bb71c`

Коммиты документации: `44634f27f803eb39a68a4d5b09d7e0c00e2c0712` (глоссарий), `0e67dd598b8a4f9be906570728211fd6a302cbc4` (инвентаризация), `1b0d27d842de30710f54b100f5d8d291139bb048` (аудит), `42fc24ff87cf9d44a3828087319cb671c48ecc81` (README).

Следующая точка продолжения: вернуться к основной очереди неполных локализаций и продолжать партиями по 10 модов. Не возвращаться к закрытому списку 108 модов без реальных новых пробелов. FTB Quests/SNBT оставить на самый конец проекта.


## Дополнение: финальная правка Sodium Extra — 05.11.2026

После предыдущего обновления документации завершена дополнительная построчная локализация Sodium Extra 0.9.5. Актуальный файл `assets/sodium-extra/lang/ru_ru.json` содержит 418 ключей; сверка с upstream EN 1.21.1/stable: 418/418, missing 0, extra 0, duplicates 0, placeholder mismatches 0, newline mismatches 0, JSON корректен.

Опубликованные коммиты:
- [Полная локализация Sodium Extra](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6d8dc79d9e086898b14e764b2a07a03f45fb2253)
- [Уточнение описания атмосферного тумана](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/59976f841ca39a87963ddd70e1596b2eba36bb9c)

Оба коммита проверены в GitHub; второй является дочерним для первого и изменяет только описание одной настройки. Запись Sodium Extra в `INVENTORY.md` уже содержит итог 418/418 и не требует повторного изменения.

Следующая рабочая точка — основная очередь неполных JSON: NeoVitae, Mekanism, Ice and Fire, Mekanism Tools, Silent Gear, Supplementaries и Regions Unexplored. После завершения этих семи модов выбрать ещё три незавершённых по актуальному состоянию репозитория. FTB Quests/SNBT файлово завершён и повторной обработки не требует.


## Незавершённая рабочая ветка — Mekanism Tools (05.11.2026)

Создана ветка `work/mekanism-tools-ru` от актуального `main`. В неё добавлены 138 отсутствовавших переводов из официального upstream Mekanism (ветка `1.21.x`, файл `src/tools/resources/assets/mekanismtools/lang/ru_ru.json`). Существующие переводы ATM10 сохранены; официальные значения не перезаписывали имеющиеся строки.

Текущее состояние рабочей ветки: 323/800 ключей, missing 477, extra 0, placeholder mismatches 0. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e234376083ceda20c72803e77c1e41ef50f4f72f

**Мод не завершён и в main не опубликован.** Продолжать перевод оставшихся 477 ключей в этой ветке, затем выполнить полную сверку с EN 10.7.19.85 и только после завершения переносить результат в main. Следующие моды из очереди не начинать до закрытия Mekanism Tools.


## Завершение Mekanism Tools — 05.11.2026

Локализация `assets/mekanismtools/lang/ru_ru.json` завершена для версии ATM10 Mekanism Tools 10.7.19.85. Итоговая сверка с английским оригиналом: 800/800 ключей, missing 0, extra 0, дубликаты 0, несовпадения плейсхолдеров 0, несовпадения количества переносов строк 0. JSON повторно разобран без ошибок. Два значения оставлены на английском намеренно: `Mekanism: Tools` (название мода) и `HP: %1$s` (короткая техническая метка с плейсхолдером).

Перевод завершён в ветке `work/mekanism-tools-ru`. Последний коммит файла: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7c99da9865d49c717b0e770eb2a21803169e097f. Инвентаризация обновлена до 800/800.

Предыдущая запись о незавершённой ветке выше является исторической; её статус заменён этим разделом. Следующий мод определяется повторным чтением актуальной очереди и сверкой файлов в обоих репозиториях. Не считать FTB Quests/SNBT завершёнными только на основании старой формулировки handoff: по правилу проекта они остаются отложенными до самого конца, пока отдельная фактическая проверка не докажет обратное.


## Текущая рабочая точка — NeoVitae (05.11.2026)

Начата локализация следующего мода основной очереди — NeoVitae 1.1.51. Проверены актуальные файлы ATM EN и upstream: 3 652 ключа, английские файлы совпадают. Официальный upstream RU содержит только 256 ключей и полностью совпадает с текущим RU-файлом; полноценного альтернативного RU-файла не найдено.

Создана отдельная ветка `work/neovitae-ru`. Добавлены первые 25 новых переводов (в основном интерфейс Sanguine Crafter и достижения). Первоначальная точка 281/3652 ключей сохранена в истории ветки. Затем добавлено 600 новых переводов. Текущее состояние ветки после следующей партии: **1 481/3 652 ключей, missing 2 171**. Коммит с последними 600 переводами: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/caefcc90c6d795b1a5e6c5ea0721a0c68ea55cb3. Работа не завершена, в `main` не опубликована. Продолжать в этой ветке, сверяясь с `translations/glossary.csv` NeoVitae и общим `GLOSSARY.md`. Не переходить к следующему моду до полного закрытия NeoVitae.


### Контрольная точка — партия из 600 новых ключей NeoVitae (05.11.2026)

- Добавлено ровно **600 новых ключей** к исходным 281; всего RU 881/3652.
- Осталось 2771 ключ. NeoVitae не завершён; в `main` не публиковался.
- Проверки по актуальному `neovitae-1.21.1-1.1.51`: JSON корректен; missing 2771, extra 0, duplicates 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0.
- Исправлены 6 ранее существовавших строк руководства с повреждённым форматированием и/или смыслом.
- Продолжать в `work/neovitae-ru`; не переходить к следующему моду до полного перевода и публикации NeoVitae.


### Актуальная контрольная точка NeoVitae — 05.11.2026

- Вторая партия: добавлено **600 новых ключей** к состоянию 881/3652; текущее покрытие — **1481/3652**, осталось 2171.
- Проверки актуального EN `neovitae-1.21.1-1.1.51`: JSON корректен; missing 2171, extra 0, duplicates 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0; все 600 новых значений непустые и отличаются от EN.
- Коммит последней партии: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/caefcc90c6d795b1a5e6c5ea0721a0c68ea55cb3.
- Коммит исправления ранее существовавших форматирующих строк и перевода HUD Сигила провидца: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/caefcc90c6d795b1a5e6c5ea0721a0c68ea55cb3.
- NeoVitae не завершён и не опубликован в `main`. Продолжать в `work/neovitae-ru`; следующая партия — не менее 600 новых ключей. Не переходить к следующему моду до полного перевода и публикации NeoVitae.


### Актуальная точка продолжения NeoVitae — 05.11.2026

- Текущее состояние `assets/neovitae/lang/ru_ru.json`: **1 481/3 652 ключей**, отсутствует 2 171.
- Вторая партия добавила ровно **600 новых ключей** к предыдущей подтверждённой точке 881/3 652.
- Проверки актуального EN `neovitae-1.21.1-1.1.51`: JSON корректен; missing 2 171, extra 0, duplicates 0, empty 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0.
- Коммит с переводами партии: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/caefcc90c6d795b1a5e6c5ea0721a0c68ea55cb3. Последняя корректировка: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a071849f23746b49884813c3dd6f0a467185f888.
- NeoVitae не завершён и не опубликован в `main`. Продолжать в `work/neovitae-ru`; следующая партия — не менее 600 новых ключей. Не переходить к следующему моду до полного перевода и публикации NeoVitae.


### Актуальная точка продолжения NeoVitae — 05.11.2026

- Текущее состояние `assets/neovitae/lang/ru_ru.json`: **1 541/3 652 ключей**, отсутствует 2 111.
- После контрольной точки 881/3 652 добавлено 660 новых ключей: 600 ключей предыдущей партии и ещё 60 строк о ритуалах Deus, Якоре ритуала, основных ритуалах и Crystallum Fractura.
- Проверки актуального EN `neovitae-1.21.1-1.1.51`: JSON корректен; missing 2 111, extra 0, duplicates 0, empty 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0.
- Переводческий коммит последней порции: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1511d56ad647c1775190212599c8bcfde6397450.
- Инвентаризация обновлена до 1 541 ключа. NeoVitae не завершён и не опубликован в `main`. Продолжать только в `work/neovitae-ru`; следующая партия — не менее 600 новых ключей.


### Текущая точка продолжения NeoVitae — 05.11.2026

- `assets/neovitae/lang/ru_ru.json`: **1 541/3 652 ключей**, отсутствует 2 111.
- После контрольной точки 881/3 652 добавлено 660 новых ключей.
- Сверка с актуальным EN `neovitae-1.21.1-1.1.51`: JSON корректен; missing 2 111, extra 0, duplicates 0, empty 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0.
- Последняя корректировка форматирования: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1f08e2c2927ba91d7c856b8e41768b38bd714d0e.
- `INVENTORY.md` обновлён до 1 541 ключа. NeoVitae не завершён и не опубликован в `main`; продолжать в `work/neovitae-ru`, следующая партия — не менее 600 новых ключей.


## Частичная контрольная точка NeoVitae — 05.11.2026

После подтверждённого состояния 1 541/3 652 добавлено ещё 94 новых перевода в ветке `work/neovitae-ru`. Текущее покрытие: **1 635/3 652**, отсутствует **2 017** ключей. Это промежуточный результат: требование следующей партии (не менее 600 новых ключей) **ещё не выполнено**; NeoVitae не завершён и в `main` не переносился.

Проверка актуального EN `neovitae-1.21.1-1.1.51`: JSON корректен; RU extra 0, duplicates 0, empty 0. Для 94 добавленных ключей проверены плейсхолдеры, цветовые/форматирующие маркеры и переносы строк — расхождений 0. Существующие 1 541 переводов не заменялись; исправлены только форматирование двух переносов строк и один пропущенный цветовой маркер в новых записях.

Коммиты переводов: [2855440](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/28554406f30a219548fc40f2a57312a3f4e1c41b), [9f4454b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9f4454bffec44d1c51b51f5486de9347f98f35cb), [4ab63ef](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4ab63ef0f9eb9e82c074393f2b7535e47fd4f089), [9067416](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9067416f218f2ccd545f36f3520dbb471ec9a252). Финальная сортировка ключей и исправление форматирования: [3831712](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3831712f68f73f99953acb7056d232e62b564599).

Следующее действие: продолжить перевод NeoVitae в этой же ветке до добавления минимум 600 новых ключей относительно контрольной точки 1 541; не переходить к следующему моду и не переносить изменения в `main`.


## Результаты следующей партии NeoVitae — 05.11.2026

В ветке `work/neovitae-ru` добавлено **600 новых переводов** к контрольной точке 1 635/3 652. Текущее покрытие: **2 235/3 652**, осталось **1 417** ключей.

Проверка с актуальным английским оригиналом `neovitae-1.21.1-1.1.51`:
- JSON корректен.
- EN/RU ключи: missing 1 417, extra 0.
- Дубликаты: 0; пустые значения: 0.
- Для всех 600 новых значений проверены плейсхолдеры, цветовые маркеры и экранированные переносы строк: расхождений 0.
- 6 совпадений с английским сохранены осознанно: названия Lex Vitae, Spiritus, Crystallarium Maleficum и счётчик `%s / %s`; это имена собственные/техническое обозначение, а не пропущенный перевод.

Переводы опубликованы отдельными коммитами: [adb1a17](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/adb1a17dca8e60765353a6751d529ff92c3905c9), [8243092](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/82430920d5e8b8557ed529914c851e270ab0f221), [66b4b6b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/66b4b6b5217d7caf69c96d9769f90d5e47abf79a), [2675ac5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2675ac561fa0b9b9919ddb4e9a9455c0ed273f6c), [32d5879](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/32d5879d609fbdd0c7a1995febfa3ea342b9babd), [8f3fc90](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8f3fc90dc01e316c718e545581f8f7028b10e339), [fc4a90c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fc4a90c747dbcab6a8d25593cf2bdc67c0437fa4), [14fe72b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/14fe72b7cd5f7d4eee63bb6271e5d5f3a0b53672). Отдельно исправлено экранирование переносов: [3238e0b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3238e0b38565dfbe9870f6e77bfcc86db3ec8353).

Обновлены `INVENTORY.md` (2 235 ключей) и `GLOSSARY.md` (термины NeoVitae). Коммиты документации: [3cd56bf](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3cd56bfb07c238820cc269812059b7fd8fe9198b), [b34a2f7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b34a2f7bf60fca218dfff224d53a6ad5448fa5a3).

NeoVitae **не завершён** и изменения не переносились в `main`. Продолжать в `work/neovitae-ru`, не переходить к следующему моду. Следующая партия — ещё не менее 600 новых ключей; исходная контрольная точка этой партии — 2 235/3 652.


## Контрольная точка NeoVitae — 05.11.2026 (следующая партия)

К контрольному состоянию **2 235/3 652** добавлено ровно **600 новых ключей** в `work/neovitae-ru`. Теперь переведено **2 835/3 652**, осталось **817** ключей.

Сверка с английским оригиналом `neovitae-1.21.1-1.1.51`:
- JSON корректен.
- Отсутствуют 817 ключей; лишних ключей: 0.
- Дубликаты: 0; пустые значения: 0.
- Для всех 600 новых ключей проверены плейсхолдеры, цветовые маркеры и экранированные переносы строк: расхождений 0.
- 11 совпадений с английскими значениями оставлены намеренно: названия/идентификаторы Neo Vitae, термин Essentia Vitae, краткие обозначения аспектов и техническое обозначение EV.

Основные коммиты этой партии: [0d3b823](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0d3b8236c58eacb4cd47ec717a928caac0cb75c4), [f8cabc2](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f8cabc2e2a7ddf20f49afe5c6675eab05fcc2c7b), [bd264dd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bd264ddc85c2220e355efcb8d450641004ca190b). Дополнительно опубликованы названия 196 предметов и 177 строк интерфейса: [c9a3acb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c9a3acba8f10211c1a4bdd87f36d982b212b00fe), [2c96267](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2c96267a3b0def84e5a8bf5edd5d12adbcdb8bd3). `INVENTORY.md` обновлён: [fc43d05](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fc43d055f004f478f50d3eb219435b110e63481c).

NeoVitae ещё не завершён; в `main` ничего не переносилось. Следующая точка продолжения — **2 835/3 652** в ветке `work/neovitae-ru`. Продолжать этот мод, пока не будут переведены и проверены все ключи.


## Продолжение NeoVitae — 05.11.2026

От контрольной точки 2 835/3 652 добавлено 20 новых переводов. Проектный счётчик: **2 855/3 652**, осталось 797. Обновлены заряды Explosive Charges, разделы Hellfire Forge, Lex Vitae, Node Router и часть Ore Processing. Проверены все 20 новых строк: плейсхолдеры, цветовые маркеры и экранированные переносы соответствуют EN. Актуальная RU-структура: 2 898 записей, missing keys 754, extra 0, duplicates 0, JSON корректен. Разница между missing keys и проектным остатком — 43 уже существующих ключа, требующих проверки значений, а не добавления новых ключей.

Коммиты переводов: [2aac1c5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2aac1c5736292c8e4eea53be9385e7ce72ab5f5d), [5b40181](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5b401816eb57dccc4378dfd14090f5e2bd5a2d20), [9f0a2ff](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9f0a2ff95f5685aac32dcf1f42d8e9e48f9ddb7a).

Следующая точка продолжения — 2 855/3 652 в `work/neovitae-ru`. В `main` ничего не переносить до полного завершения и проверки NeoVitae.


## Завершение NeoVitae — 05.11.2026

В рабочей ветке `work/neovitae-ru` завершён перевод актуального `neovitae-1.21.1-1.1.51`: **3 652/3 652 ключа**. После контрольного состояния 3 383 ключа добавлены и опубликованы ещё 269 переводов, включая описания ритуалов, улучшения разумной брони, подсказки, аспекты Spiritus и оставшиеся записи книги.

Все ранее существовавшие совпадения RU=EN проверены отдельно. Сохранены только собственные имена, латинские названия аспектов/ритуалов, идентификаторы и технические строки; переведены обычные подписи интерфейса и термины, которые должны соответствовать GLOSSARY.md.

Финальная техническая сверка:
- JSON корректен.
- EN/RU: 3 652/3 652; missing 0; extra 0.
- Дубликаты ключей: 0; пустые значения: 0.
- Несовпадения плейсхолдеров: 0.
- Несовпадения переносов строк: 0.
- Несовпадения форматирующих кодов Minecraft (§): 0.

Последние коммиты переводов:
- [a862037](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a8620372d07b7d41b052347ed8ce3d36903d51d2) — 76 ключей.
- [1bec32b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1bec32b5c041812aba65078bba06c809e8dd1e44) — 99 ключей.
- [b2d7df3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b2d7df3a4c0e27b08a6bffb4a48681937b24174a) — 90 ключей.
- [407a3ef](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/407a3efdb1b1d41a83e4b6c4d80ddc06a5894205) — последние 4 ключа.
- [806e239](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/806e239fe80e7b576d034d7cf2e90390ce3b6313) — терминологическая правка 7 значений.
- [a3d1069](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a3d1069eaa33aceee4f1ce1ca8b1a5a83f1748e1) — обновление INVENTORY.md.

`INVENTORY.md` отражает полное покрытие 3 652/3 652. NeoVitae завершён в `work/neovitae-ru`; в `main` ничего не переносилось. Перед началом следующего мода проверить текущие ветки, PROJECT_HANDOFF.md, INVENTORY.md и GLOSSARY.md. FTB Quests и SNBT остаются на самый конец проекта.


## Завершение локализации Productive Trees — 05.11.2026

Productive Trees `1.21.1-1.1.1` полностью переведён в `work/productivetrees-ru`: **4 149/4 149 ключей**. В исходном RU-файле было 3 832 ключа; добавлено 317 переводов. Сверка с английским `en_us.json`: missing 0, extra 0, duplicates 0, placeholder mismatches 0, newline mismatches 0, Minecraft formatting-code mismatches 0. JSON корректен.

Оставлены без изменений только два латинских ботанических названия, исходное пустое значение `thunder_bolt.latin` и технический плейсхолдер `%s`; эти совпадения не являются непереведённым пользовательским текстом.

Коммиты:
- Переводы: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9c314b46f925358fdc01d66945f14bb88b482deb
- Глоссарий: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/55bdd44df2aef9edeff5610270231385af296521
- Инвентаризация: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9f49791e86d8f8870166413da22d27458bda7785

`main` не изменялся. Продолжать со следующего действительно незавершённого мода по актуальному INVENTORY.md; не повторять NeoVitae и Productive Trees. FTB Quests/SNBT остаются на финальном этапе.

## Контрольная сверка первых 25 RU-файлов — 05.11.2026

Для воспроизводимости взяты первые 25 `assets/*/lang/ru_ru.json` в алфавитном порядке актуальной `main`. У 24 файлов найден EN-оригинал в read-only репозитории; для `advancedperipherals` оригинал в выгрузке не найден.

Сверка 24 пар: EN 9 261 ключ, RU 8 958 записей; missing 313, extra 10, пустых значений 1, несовпадений плейсхолдеров `%s/%d/%i/%f` на общих ключах 0. Точные совпадения значений RU/EN — 273; они не приравниваются автоматически к ошибкам.

Реальные проблемы: `ad_astra` — 146 отсутствующих переводов (биомы, конфигурация, измерения, картины, жидкости, стороны подключения, теги); `aether` — 167 отсутствующих (конфигурация, подсказки, биомы, описания, эффекты, существа, субтитры); `actuallyadditions` — одно пустое значение и 82 совпадения с EN, среди которых есть непереведённые пользовательские строки конфигурации, подсказок, описаний, сетевых сообщений и интерфейса; `allthemodium` — 10 лишних ключей, отсутствующих в EN.

Значительная часть совпадений в `apothic_enchanting` (названия композиций, римские/арабские числа, символы), `apotheosis` (шаблоны, символы, авторы), `allthetweaks` (бренды, цветовой код, Discord, юридическое предупреждение) выглядит намеренной. В Ad Astra имена мода, символы, единицы измерения и шаблоны также требуют сохранения, но названия существ и субтитры — перевода.

Это диагностическая сверка, а не завершённая партия: файлы локализаций не изменялись и не публиковались. Следующий шаг — исправление реальных пробелов по правилам проекта; FTB Quests/SNBT остаётся финальным этапом.


## Завершение локализации Mekanism — 05.11.2026

Mekanism `1.21.1-10.7.19.85` полностью локализован в ветке `work/productivetrees-ru`: **3 239/3 239 ключей**. Исходный RU-файл содержал 1 608 ключей; добавлены недостающие переводы, включая проверенные значения из официальной русской локализации Mekanism, и вручную переведены новые настройки конфигурации, генерации мира, интерфейса и интеграции ProjectE. Существовавшие RU-значения не перезаписывались.

Финальная сверка с read-only EN-файлом `Mekanism-1.21.1-10.7.19.85/mekanism/en_us.json` (SHA `828f82d2f8739eefc1e7674fda04c835183110af`): JSON корректен; EN/RU 3 239/3 239; missing 0; extra 0; дубликаты ключей в исходном JSON 0; пустые значения 0; несовпадения плейсхолдеров 0; переносов строк 0; форматирующих кодов Minecraft (§) 0. 47 совпадений RU=EN оставлены как технические обозначения, единицы/форматы, идентификаторы и имена собственные; проверка внутриигрового отображения не проводилась.

Коммиты перевода и терминологии:
- [8ee7a79](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8ee7a797bbb10e27329e85bdcd204b1ac6b03c45) — финальная терминологическая правка.
- [4936c00](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4936c00996091d65f68c5702b1c4f7f55dfe6667) — перевод настроек генерации мира; покрытие 3 239 ключей.
- [6b4253c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6b4253ce09ff1f40b507bb11abac61687d684d83) — перевод общих настроек.
- [feab50c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/feab50c9f3d4d9635de69fc26f65bfca19d8cd81) — перевод настроек уровней.
- [7fa1e84](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7fa1e84df3cfd6221091bd6e9ad73a248c798b68) — перевод настроек снаряжения.
- [0338270](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0338270afbd117bca90b9236075556b0cd1f2fc3) — перевод хранения энергии и расхода энергии машин.
- [78ace09](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/78ace0917b7b80dabd9046484082044766447e94) — перевод интеграции ProjectE.

Глоссарий и инвентаризация обновлены отдельными коммитами. Работа находится в рабочей ветке; `main` не изменялся. Следующий мод по очереди — Ice and Fire. Внутриигровое тестирование Mekanism остаётся отдельной последующей проверкой.


## Завершение локализации Ice and Fire — 05.11.2026

Ice and Fire `2.1.4` полностью локализован в ветке `work/productivetrees-ru`: **1 809/1 809 ключей**. Было 1 194 существующих RU-записей; добавлено 615 недостающих переводов. Переведены новые настройки существ, брони и генерации мира, описания баннерных узоров, предметы, эффекты, Jade/EMI/JEI и обучающие подсказки. Существующие RU-значения сохранены.

Финальная сверка с read-only EN-файлом `iceandfire-2.1.4/iceandfire/en_us.json` (SHA `1bf20350cc8e852d35e0f8b2d4b71d6036e4f77f`): JSON корректен; EN/RU 1 809/1 809; missing 0; extra 0; дубликаты ключей 0; несовпадения плейсхолдеров 0; переносов строк 0; форматирующих кодов Minecraft (§) 0. Одно пустое значение сохранено, поскольку оно пустое и в английском оригинале. 9 совпадений RU=EN оставлены как технические обозначения, названия брендов/собственные имена или исходные пустые/служебные значения. Внутриигровое тестирование не проводилось.

Коммиты:
- [2525860](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/252586066157810bf8d9e6686cc49102c7e32954) — финальная правка пользовательских строк.
- [f160775](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f16077529c2f74690cecf75b60e3b91f8b3297c3) — перевод 245 параметров конфигурации.
- [c2905f6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c2905f61893059ec2b4e8657604440b29f6c0876) — перевод предметов, интерфейса и обучающих подсказок.
- [ee7b543](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ee7b543f341527e1e1610ac4d1c4bdc7f5424106) — перевод 304 названий баннерных узоров.

Глоссарий и инвентаризация обновлены. Следующий незавершённый мод по текущей инвентаризации — Silent Gear. Работа остаётся в рабочей ветке; `main` не изменялся.


## Завершение локализации Silent Gear — 05.11.2026

Silent Gear ATM10 8.5 полностью локализован в ветке `work/productivetrees-ru`: **1 191/1 191 ключ**. Исходный RU-файл содержал 617 ключей; добавлено 574 перевода, существовавшие значения сохранены. Переведены достижения, блоки, команды, интерфейсы машин, типы снаряжения, предметы и детали, JEI, материалы, характеристики, конфигурация и свойства.

Финальная сверка с read-only EN-файлом `silent-gear-1.21.1-neoforge-4.2.1.1/silentgear/en_us.json` (SHA `458a50aed74a049d099ab97bf14723b0fb91dc1b`): JSON корректен; EN/RU 1 191/1 191; missing 0; extra 0; дубликаты ключей 0; несовпадения плейсхолдеров 0; несовпадения кодов форматирования Minecraft (§) 0; несовпадения количества переносов строк 0. Три ранее совпадавших с EN описания достижений дополнительно переведены после смысловой проверки. Оставшиеся совпадения RU=EN — технические подписи, плейсхолдеры, название мода и буквенные/ранговые обозначения grade (A–E, S–SSS, MAX). Внутриигровое тестирование не проводилось.

Коммиты перевода: [4ae2a83](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4ae2a83cde5048aea1fc242a42b03adbd30ae04f), [5269ad8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5269ad88435aae15f3035ecd3aec35515e5fd185), [eaa0f20](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/eaa0f204c8d59459a3933f3ea5e4163135e8fc02), [e135d5b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e135d5b417c92e23b69414837ed8a21effd11f0e), [fa0a4f0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fa0a4f092ffb0414554c66329d7e621e1a729665), [d80af99](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d80af9995dfb5d98442ca28ac25391bf684332b3), [0a44d35](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0a44d3596f2bcb55d8d0ab41fa8b0e25610cd67c), [28e31bb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/28e31bb921f5dc0bda0762c7ba309005e9645391), [bd843c7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bd843c72bd123a157d4b03a2fc9c383e45651544), [0ca79f8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0ca79f848316918b55707c608135fec1195274cd) — финальная смысловая правка трёх достижений.

Обновлены `INVENTORY.md` и `GLOSSARY.md`: [27d43d6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/27d43d62a46efeee9f13da751b54f9a7ced2c4d7), [681f6cb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/681f6cb7d101cb7befe2dde100e3e6b3fbd10e46). `main` не изменялся. Следующая точка продолжения — Supplementaries, затем Regions Unexplored. FTB Quests/SNBT остаются на финальном этапе. Партия из десяти модов ещё не завершена.


## Завершение локализации Supplementaries — 05.11.2026

Supplementaries `4.0.2` полностью переведён в `work/productivetrees-ru`: **1 394/1 394 ключа**. Исходный RU-файл содержал 708 ключей; добавлено 686 переводов. Переведены оставшиеся пользовательские строки, включая 659 новых/обновлённых настроек конфигурации, субтитры, сущности, блоки, предметы, погоду и сообщения интерфейса.

Финальная сверка с read-only EN-файлом `supplementaries-1.21.1-4.0.2-neoforge/supplementaries/en_us.json`: JSON корректен; EN/RU 1 394/1 394; missing 0; extra 0; дубликаты 0; пустые значения 0; несовпадения плейсхолдеров 0; несовпадения кодов форматирования Minecraft (§) 0; несовпадения переносов строк 0. Десять совпадений RU=EN оставлены как технические подписи/плейсхолдеры, название мода и имена авторов картин.

Последний коммит перевода: [e86223b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e86223bcd60c6ce714a05dd6c75b80a5911a4397). Обновлены `INVENTORY.md` и `GLOSSARY.md`; финальный коммит инвентаризации: [2d4beb5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2d4beb5a20053a9f7ab38174014bbbf48315ff71), глоссария: [4048672](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4048672d84d0009daebf60467cf64cb0883cc492).

Шесть из семи модов текущей очереди завершены: NeoVitae, Mekanism, Ice and Fire, Mekanism Tools, Silent Gear и Supplementaries. Следующая точка продолжения — Regions Unexplored. Это ещё не партия из десяти модов; после Regions Unexplored выбрать следующие незавершённые моды по актуальному репозиторию. `main` не изменялся. FTB Quests/SNBT остаются на финальном этапе.


## Regions Unexplored завершён — 05.11.2026

Regions Unexplored 0.6.3-neoforge-21.1: **933/933 ключа**. Исходный RU-файл содержал 455 ключей; добавлено 478 переводов. EN/RU сверка: missing 0, extra 0, duplicates 0, empty 0, placeholder mismatches 0, formatting mismatches 0, newline mismatches 0; JSON корректен. Единственное RU=EN совпадение — название мода в творческой вкладке.

Перевод: [7affad8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7affad8265968599924b64d9fff82e25b42208c9). Глоссарий: [c844fe5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c844fe56b5115795d82fc4c9b59793f7b80fe7d5). Инвентаризация: [b80e87b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b80e87ba53ff7aaf70c0483858d16361b6654b8e).

Завершены 7 модов текущей очереди: NeoVitae, Mekanism, Ice and Fire, Mekanism Tools, Silent Gear, Supplementaries и Regions Unexplored. Партия из десяти ещё не завершена. Следующий шаг — определить три следующих незавершённых мода по актуальным INVENTORY.md и EN-источникам. main не изменялся. FTB Quests/SNBT оставить на самый конец.


## Партия из десяти модов завершена — 05.11.2026

Подтверждено 10/10 завершённых локализаций: NeoVitae, Mekanism, Ice and Fire, Mekanism Tools, Silent Gear, Supplementaries, Regions Unexplored, Explorer's Compass, Measurements и Nature's Compass. Для последних трёх восстановлены только пропущенные служебные поля _comment; пользовательские строки уже были переведены.

Explorer's Compass: 68/68, commit [9cfe773](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9cfe773670b156ea801e8a53c2a9feeb6fcbc1e8). Measurements: 15/15, commit [9c6c48a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9c6c48a3a76b66b7827d2871525da9ec2e08870a). Nature's Compass: 44/44, commit [1b1cb11](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1b1cb114c2a8fd8bd22212e99fe9e9f445c5451d). Во всех трёх файлах missing 0, extra 0, duplicates 0, placeholder mismatches 0, formatting mismatches 0, newline mismatches 0.

Обновлена инвентаризация: [4ea2fd3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4ea2fd3bf85c437d8572734dbd0cbaa976730c40). Следующая партия начинается с Ad Astra: EN 831, RU 685, missing 146, extra 0. Также обнаружен недостающий служебный ключ ZeroCore: EN 50, RU 49. Перед следующими модами сверить свежие состояния репозиториев и определить следующую очередь по INVENTORY.md. `main` не изменялся. FTB Quests/SNBT оставить на самый конец.


## Актуальная точка проекта — 05.11.2026

### Завершённая партия JSON-локализаций: 10/10

После интеграции PR #4 и завершения Aether и Mekanism Tools в `main` подтверждены следующие полные локализации:

| Мод | EN/RU | Missing | Extra | Плейсхолдеры |
|---|---:|---:|---:|---:|
| Ad Astra | 831/831 | 0 | 0 | 0 |
| Mekanism | 3239/3239 | 0 | 0 | 0 |
| Ice and Fire | 1809/1809 | 0 | 0 | 0 |
| NeoVitae | 3652/3652 | 0 | 0 | 0 |
| Productive Trees | 4149/4149 | 0 | 0 | 0 |
| Silent Gear | 1191/1191 | 0 | 0 | 0 |
| Supplementaries | 1394/1394 | 0 | 0 | 0 |
| Regions Unexplored | 933/933 | 0 | 0 | 0 |
| Aether | 1238/1238 | 0 | 0 | 0 |
| Mekanism Tools | 800/800 | 0 | 0 | 0 |
| **Итого** | **19236/19236** | **0** | **0** | **0** |

Для файлов проверены корректность JSON, наборы ключей и плейсхолдеры. Для ранее завершённых в рабочей ветке файлов также были проверены дубликаты, форматирование Minecraft (§) и переносы строк. В Mekanism Tools заполнено последнее пустое значение `configuration.mekanismtools.server.gear_spawn_chance.refined_glowstone.chance.multiple_piece` — «Шанс появления нескольких частей брони».

Публикация:
- PR #4, объединение восьми локализаций и документации: https://github.com/d1gorae/ATM10-RU-TRANSLATE/pull/4 ; merge commit `a49e7659d0c8eded7295a92b95d3a8c5f5087a46`.
- Aether 1238/1238: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/30bbf0d4b3f4386cf846d45d458fffe0b94bd185.
- Mekanism Tools — устранено последнее пустое значение, 800/800: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cb9049377678f3ed0479f6fe922ae25e5398cc32.

**Следующая очередь по актуальным данным:** Ars Nouveau, EvilCraft, Iron's Spellbooks, PneumaticCraft, Twilight Forest, Industrial Foregoing, Integrated Dynamics и Reliquary имеют подтверждённые отсутствующие EN-ключи. Дополнительно требуется смысловой аудит совпадений с английским в Actually Additions. Перед началом следующей партии проверить ещё незакрытые namespace по текущему EN-дереву, чтобы выбрать ровно десять действительно нуждающихся в работе модов.

FTB Quests/SNBT не затрагивать до заключительного этапа. Dropbox и английский репозиторий остаются read-only.


## Текущая рабочая сессия — 05.11.2026

Начата следующая партия JSON-аудита. На текущий момент полностью завершены и опубликованы 2 мода; партия из 10 не закрыта.

- **Actually Additions** — 1026/1026 ключей. Missing 0, extra 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0. Переведены 62 пользовательские строки, ранее совпадавшие с EN. Остальные совпадения — бренд, обозначения CF/NBT/ESD, числовые значения и служебные комментарии. Ключ `info.actuallyadditions.gui.the` оставлен пустым намеренно: английский артикль в русском не требуется. Коммиты: [6146656](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/61466567329721c466729420646696fb7504c3b2), [c74229a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c74229a20476239869f02082311d8d99b8fafc61); глоссарий [0d29e45](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0d29e450f1a95ec400661d698468a3d07bac44c3).
- **Industrial Foregoing** — 683/683 ключа. Missing 0, extra 0, empty 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0. После смысловой проверки переведены все оставшиеся пользовательские строки; восемь EN/RU совпадений сохранены только для бренда, единицы FE и служебных комментариев. Коммиты: [23032f0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/23032f0d5ad06fcb3afefa9b560b702b82f552bd), [7a3f978](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7a3f97825e6b1a29346d171fd553e3772edb27a8); глоссарий [ae17226](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ae1722667226116b21dd6af1e7b556a3b572f758).

**Следующая точка продолжения:** Iron's Spells 'n Spellbooks — в main 1128/1315 ключей, missing 187, extra 0. Не переносить файл из upstream целиком: его ru_ru.json также неполон и содержит отдельные несовпадения плейсхолдеров. Сохранять существующие переводы и дополнять только проверенными значениями. После завершения модов продолжить текущую десятку по подтверждённой очереди: EvilCraft, PneumaticCraft, Twilight Forest, Integrated Dynamics, Reliquary и Ars Nouveau; сверить оставшиеся namespace для точного состава партии из 10. FTB Quests/SNBT не трогать до заключительного этапа.

## Завершение локализации EvilCraft — 05.11.2026

EvilCraft полностью переведён и проверен: **629/629 ключей**, добавлено 253 значения к существовавшим 376. Missing 0, extra 0, RU duplicates 0, empty 0, placeholders 0, newlines 0, Minecraft/guidebook formatting codes 0. В EN-оригинале обнаружено 9 повторных объявлений ключей; RU-файл содержит уникальный набор из 629 ключей.

Коммиты: переводы [4427380](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/44273800b06b8b7c692e2495a50ef16039243333), [1929218](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/192921836e3b2959eac96f3d4d5f58d2dd77a31c), [676c20e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/676c20e82fd9a2b2e64bd1ef6ac293e95ac06c8b), [afd8bcf](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/afd8bcfdce25aae5e5a06d4d2eaa6b21c9f89444), [29f0a59](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/29f0a5934ee0ab3246d2441c365be9943bbf7754), [2be1727](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2be1727a45f1b1313608b62ef122c07c2b1751d7). Глоссарий [${gUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${gUp.result.commit_sha}); INVENTORY [${iUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${iUp.result.commit_sha}).

Текущая партия: **4/10** — Actually Additions, Industrial Foregoing, Iron's Spells 'n Spellbooks, EvilCraft. Следующий мод — PneumaticCraft: Repressurized; затем Twilight Forest, Integrated Dynamics, Reliquary и Ars Nouveau. После этих подтверждённых кандидатов проверить актуальное EN-дерево и выбрать ещё четыре действительно незавершённых мода. FTB Quests/SNBT не затрагивать до финального этапа.

## Завершение локализации PneumaticCraft — 05.11.2026

PneumaticCraft: Repressurized полностью переведён и проверен: **2 274/2 274 ключа**, добавлено 287 значений. Missing 0, extra 0, duplicates 0, empty 0, placeholders 0, newlines 0, Minecraft formatting 0. Восстановлены корректные переводы ряда старых подсказок и сообщений, включая GPS-инструменты, фильтр сущностей, Amadron и жидкостную воронку.

Коммиты: переводы [f83e2ed](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f83e2ed07c312f5376dd783ae727cb34fb210d1c), [fb749b5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fb749b5e45ed4d48f6ae0e34e2d23a0a2309a8c4), [59dc0f2](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/59dc0f279846eb0155b8ee085275696427a8853b), [2d8c0bf](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2d8c0bf2e3d618587c857fbcab924ea0bf206eb0). Глоссарий [${gUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${gUp.result.commit_sha}); INVENTORY [${iUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${iUp.result.commit_sha}).

Текущая партия: **5/10** — Actually Additions, Industrial Foregoing, Iron's Spells 'n Spellbooks, EvilCraft, PneumaticCraft: Repressurized. Следующий мод — Twilight Forest (`1 475/2 061`, по последней инвентаризации missing 586). Затем Integrated Dynamics, Reliquary и Ars Nouveau; после них сверить актуальное EN-дерево и выбрать ещё три действительно незавершённых мода. FTB Quests/SNBT не затрагивать до финального этапа.

## Завершение локализации Twilight Forest — 05.11.2026

Twilight Forest полностью переведён и проверен: **2 061/2 061 ключ**, добавлено 586 значений. Missing 0, extra 0, duplicates 0, empty 0, placeholders/order 0, newlines 0, formatting 0, `${...}` 0, trailing whitespace mismatches 0.

Коммиты: переводы [4ee350b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4ee350b29b217ed85f5466fcf8feebfddd8a5d79), [4095f18](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4095f18ce3a0e6da8acf3317910a3f1e5fd1da32), [137ddde](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/137ddde891f3c955df1b068b61a536e656ef82e9), [0776c50](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0776c50e2722cc7b821964adc43435d59fbf2eae), [3b83005](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3b83005dac8dbd9483775837ce6d56ea9c9c26d1), [2cc21eb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2cc21eb25c39707c087e23f405e6576c94fb02d1), [c95129b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c95129bd7029aea85842c0d015bb4d1996e5c43b). Глоссарий [${gUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${gUp.result.commit_sha}); INVENTORY [${iUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${iUp.result.commit_sha}).

Текущая партия: **6/10** — Actually Additions, Industrial Foregoing, Iron's Spells 'n Spellbooks, EvilCraft, PneumaticCraft: Repressurized, Twilight Forest. Следующий мод — Integrated Dynamics (`1 629/1 854`, по последней инвентаризации missing 225). Затем Reliquary и Ars Nouveau; после них сверить актуальное EN-дерево и выбрать ещё два действительно незавершённых мода. FTB Quests/SNBT не затрагивать до финального этапа.

## Завершение локализации Integrated Dynamics — 05.11.2026

Integrated Dynamics полностью переведён и проверен: **1 854/1 854 ключа**, добавлено 225 значений. Missing 0, extra 0, duplicates 0, empty 0, placeholders 0, newlines 0, formatting 0, interpolation 0, trailing whitespace mismatches 0. EN содержит два повторных объявления ключей; RU-файл без дубликатов.

Коммиты: переводы [d65e0f7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d65e0f74aba6fea851920893f4ad18151d97ddaf), [2882337](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2882337cf799a7ad8d4e0d913c9880ee65d6f0ce), [c0be297](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c0be297cb38fdd9a0d2f51c4263ca00a4c204a0a), [aa16aa2](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/aa16aa2f4a35f3b49b6632c93a137a121b76c5d4), [eb47cde](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/eb47cdeff037a1afac580b0be98bbe63cea128c0). Глоссарий [${gUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${gUp.result.commit_sha}); INVENTORY [${iUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${iUp.result.commit_sha}).

Текущая партия: **7/10** — Actually Additions, Industrial Foregoing, Iron's Spells 'n Spellbooks, EvilCraft, PneumaticCraft: Repressurized, Twilight Forest, Integrated Dynamics. Следующий мод — Reliquary (`307/551`, по последней инвентаризации missing 244). Затем Ars Nouveau; после него сверить актуальное EN-дерево и выбрать ещё один действительно незавершённый мод. FTB Quests/SNBT не затрагивать до финального этапа.

## Завершение локализации Reliquary — 05.11.2026

Reliquary полностью переведён и проверен: **551/551 ключ**, добавлено 244 значения. Missing 0, extra 0, duplicates 0, empty 0, placeholders 0, newlines 0, formatting 0, trailing whitespace mismatches 0. Исправлены старые лишние переносы строк в описаниях предметов и рецептов.

Коммиты: переводы [af1e379](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/af1e37920f13865a8fe6742cf139a0782f9ba79c), [e715c2c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e715c2c290a43059bc4f71ceadb8e80a4b8c4b0e), [4df0756](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4df0756a43456af1bdf1267326fc08a44f526905), [318476b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/318476b356d0dbbabb8712997d579161acb00ebb), [b408fb1](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b408fb151c36ffd3333d208f0aafda5bb1f09047), [fff4284](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fff4284c96f785496544bfba6f627b1d3b5024dc). Глоссарий [${gUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${gUp.result.commit_sha}); INVENTORY [${iUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${iUp.result.commit_sha}).

Текущая партия: **8/10** — Actually Additions, Industrial Foregoing, Iron's Spells 'n Spellbooks, EvilCraft, PneumaticCraft: Repressurized, Twilight Forest, Integrated Dynamics, Reliquary. Следующий мод — Ars Nouveau (`1 296/2 323`, по последней инвентаризации missing 1 027). После него сверить актуальное EN-дерево и выбрать ещё два действительно незавершённых мода. FTB Quests/SNBT не затрагивать до финального этапа.

## Завершение локализации Ars Nouveau — 05.11.2026

Ars Nouveau полностью переведён и проверен: **2 323/2 323 ключа**, добавлено 1 027 значений. Missing 0, extra 0, duplicates 0, placeholders 0, newlines 0, formatting 0, whitespace mismatches 0. Единственное пустое значение совпадает с пустым значением EN.

Коммиты: переводы [a113ce3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a113ce37d8c8d606044fbcb6f49e4270ee30ff13), [0caf1ed](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0caf1ed8221fd735439d73ba2ee87a8d873e1069), [0fd225f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0fd225f8864fe9467974c0cd3504af5a302d6bd4), [0034bf5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0034bf5a9a323dc175aa86edf611aa9d067e7f35), [8ee5c50](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8ee5c5074bfdfca9e4d5829529a89b0b2a9cc8f9), [69cbd0c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/69cbd0c905a152e81e659599ea5d7a60905ef996), [3efa0af](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3efa0af633db83f7a775738493dea38549631031), [57e04a6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/57e04a6adf82e0ca09e6e41b8956f654fd4663d1), [f3905da](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f3905da73702a4322c8653cc8a4d086d7228d957), [ca25b56](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ca25b563231658461f3d8650cec519acea0c9330), [36bf355](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/36bf355a621d8b8e7ec3ed3af8ba9275b55e3fb1), [08ff5e3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/08ff5e32a9d506732e41835c5bc62007d4e392a8), [af9a658](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/af9a658bd97e6c8faff5a402f527ea326691a12b), [921037e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/921037e879ddf2573d07aaf825f7e9486f6203d3), [155e7fd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/155e7fda7e5fd56a5a1f85edb6e617e0897b4022). Глоссарий [${gUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${gUp.result.commit_sha}); INVENTORY [${iUp.result.commit_sha.slice(0,7)}](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/${iUp.result.commit_sha}).

Текущая партия: **9/10** — Actually Additions, Industrial Foregoing, Iron's Spells 'n Spellbooks, EvilCraft, PneumaticCraft: Repressurized, Twilight Forest, Integrated Dynamics, Reliquary, Ars Nouveau. Для завершения партии нужен ещё один действительно незавершённый мод; следующий шаг — полный аудит INVENTORY и EN namespaces, затем выбрать мод с неполной локализацией. FTB Quests/SNBT не затрагивать до финального этапа.


## Партия JSON-локализаций завершена — 06.11.2026

**Подтверждено 10/10 модов:** Actually Additions, Industrial Foregoing, Iron's Spells 'n Spellbooks, EvilCraft, PneumaticCraft: Repressurized, Twilight Forest, Integrated Dynamics, Reliquary, Ars Nouveau и Mekanism: MoreMachine.

Mekanism: MoreMachine (`mekmm`) завершён последним в партии: **704/704 ключа**. В импортированном файле все ключи уже присутствовали, однако 223 пользовательских значения совпадали с EN и были переведены. Итоговая проверка актуального EN `mekmm-1.21.1-1.4.2/mekmm/en_us.json`: missing 0, extra 0, duplicates 0, empty 0, точных RU=EN совпадений 0, placeholder mismatches 0, formatting mismatches 0, newline mismatches 0, interpolation mismatches 0, whitespace mismatches 0; JSON корректен.

Коммиты Mekanism: MoreMachine: перевод [5087a5c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5087a5c90e2907574d447a4ab81d771de073237b), уточнения [7bbcfd5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7bbcfd52197ae7edfa150f33e6146bd228f8259c) и [16b0934](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/16b0934e9562cc90ccf77f1d06490ca5d95e51d1); глоссарий [e445dbf](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e445dbfc5064f8946f25216fac6435bb2918bdcc); инвентаризация [a5d4172](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a5d417243d1e55421716653b83fe65bbfd55842b).

Суммарное число ключей по десяти модам: **13 420**. Переводы и документация опубликованы в ветке `work/irons-spells-nov05`; `main` не изменялся. Следующая точка продолжения — заново сверить актуальные состояния обоих репозиториев, `INVENTORY.md` и `GLOSSARY.md`, затем выбрать следующую десятку по фактическим пропускам. FTB Quests/SNBT оставить на заключительный этап.


## Вторая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** Ad Astra: Giselle Addon, Additional Lights, Advanced AE, Advanced Peripherals, Applied Energistics 2, AE2 Crafting Tree, AE2 Import Export Card, AE2 Network Analyser, AE2 Wireless Terminals Library и AE Infinity Booster.

Итог: **1 869/1 869 ключей**. Во всех десяти файлах JSON корректен; missing 0; extra 0; duplicates 0; empty 0; placeholder mismatches 0; formatting mismatches 0; newline mismatches 0; interpolation mismatches 0; whitespace mismatches 0. 17 совпадений RU=EN оставлены намеренно: названия/бренды, FE, OpenComputers, P2P, служебный `_eof` и шаблоны с плейсхолдерами. Обычных непереведённых пользовательских строк среди совпадений нет.

В Advanced Peripherals исправлены формулировки достижений и подсказок NBT Storage, Block Reader, Colony Integrator, ME Bridge и RS Bridge; унифицировано обращение. В Advanced AE исправлена подсказка Evasion и лишний пробел. В Applied Energistics 2 исправлены формулировки команд, SCS, выбора ЦП и названия фиолетового стеклянного МЭ-кабеля. Глоссарий дополнен терминологией AE2.

Коммиты: Advanced Peripherals [585f167](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/585f167ee7e7e2a2cbbacbb9647a9d60ab4d7ea4), [e26d9bb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e26d9bb351e0558a7fadd43857d3396f7d3e5274); Applied Energistics 2 [d9d7687](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d9d768712dd2f5cd0e9b0d70a2d1baf26918dee2); Advanced AE [475187a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/475187a9e7bf4ea5f4ebc6b1ceb54b3e158ed3ac); глоссарий [2f0416a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2f0416adfd15844ba2994f4be858c848a2905548); INVENTORY [1d0c960](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1d0c9600b239288aaaa96bbaa2bc511d7076e614).

В двух последних партиях подтверждено **20/20 модов**, суммарно **15 289 ключей**. Работа опубликована в ветке `work/irons-spells-nov05`; `main` не изменялся. Следующая точка продолжения — продолжить проверку по актуальному дереву английских источников и инвентаризации после `aeinfinitybooster`, выбрать следующие десять непроверенных namespace. FTB Quests/SNBT оставить на заключительный этап.


## Третья партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** Akashic Tome, All The Arcanist Gear, AllTheCompressed, Allthemodium, AllTheOres, All The Tweaks, All the Wizard Gear, Almost Unified, Amendments и Apotheosis.

Итог: **3 851/3 851 ключ**. Во всех десяти файлах JSON корректен; missing 0; extra 0; duplicates 0; empty 0; placeholder mismatches 0; formatting mismatches 0; newline mismatches 0; interpolation mismatches 0; whitespace mismatches 0. 27 совпадений RU=EN оставлены намеренно: названия модов/брендов, авторы картин, шаблоны плейсхолдеров, кнопка X и цветовое значение. Обычных непереведённых пользовательских строк среди совпадений не осталось.

В Apotheosis унифицировано обращение на «вы» в обучении, подсказках, описаниях аффиксов и достижениях; исправлена формулировка подсказки достижения и сохранены 20 завершающих пробелов в названии достижения по EN-оригиналу. В All The Tweaks переведены два предупреждения о косметических функциях Valhelsia. Глоссарий дополнен терминами Apotheosis.

Коммиты: Apotheosis [423a2bd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/423a2bdbdab7c3a2ddfb130a64277193210fc10a), [65f0248](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/65f024888f80249bc5d54ce7a0bcef22cb58731c), [a758e5d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a758e5d9aa4ec6c0b5c1c2d7f9605edf43a6de8e); All The Tweaks [cf5c28c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cf5c28c31bf2364f8bf00dd2c24be2bcbe84d671); глоссарий [77d202e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/77d202e7eb82a6bece3317421472bdb1ee616463); INVENTORY [c9b4a8f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c9b4a8fc144672058337c1bd70d840e423664c18).

В трёх последних партиях подтверждено **30/30 модов**, суммарно **19 140 ключей**. Работа опубликована в ветке `work/irons-spells-nov05`; `main` не изменялся. Следующая точка продолжения — продолжить проверку по актуальному дереву EN-источников и инвентаризации после `apotheosis`, выбрать следующие десять непроверенных namespace. FTB Quests/SNBT оставить на заключительный этап.


## Четвёртая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** Apothic Attributes, Apothic Enchanting, Apothic Spawners, Applied Flux, AppleSkin, Applied Mekanistics, Aquaculture, Ars Additions, Ars Controle и Ars Creo.

Итог: **1 398/1 398 ключей**. Во всех десяти файлах JSON корректен; missing 0; extra 0; duplicates 0; empty 0; placeholder mismatches 0; formatting mismatches 0; newline mismatches 0; interpolation mismatches 0; whitespace mismatches 0. 144 совпадения RU=EN сохранены намеренно: названия/бренды, имена авторов и музыкальные композиции, римские обозначения уровней зачарования, FE/QIO, Shift/Ctrl, XNOR/XOR, служебный комментарий EMI и шаблоны с плейсхолдерами. Обычных непереведённых пользовательских строк среди совпадений нет.

В Ars Additions полностью переведены смешанные англо-русские описания Memory Crystal и Source Spawner, подсказка сохранения/загрузки и Warp Index; официальное имя мода восстановлено в группе предметов. В Apothic Spawners исправлено название корневого достижения. В Ars Controle улучшено описание пульта и согласован термин «круговое меню». Глоссарий дополнен терминологией Ars Additions и связанных модов.

Коммиты: Ars Additions [982b74b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/982b74b5d993da0c3d33b091c657e976c5daf587), [4257af8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4257af80ac6c60cf53cc8d096c4801a6fee2a843); Apothic Spawners [e57660d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e57660d082537663e188d6aca2495608cc491701); Ars Controle [afcf57c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/afcf57c68abbf6632e043af2605c199bfb23fe66); глоссарий [b6ed8fd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b6ed8fd7090f7ba478406ccc82dd13566d524df9), [f890452](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f890452656f803a89b5ee472bbb64ae9956b953a); INVENTORY [6b21ffc](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6b21ffc154b99a228fb1d5af1d8504a2e2135783).

В четырёх последних партиях подтверждено **40/40 модов**, суммарно **21 936 ключей**. Работа опубликована в ветке `work/irons-spells-nov05`; `main` не изменялся. Следующая точка продолжения — продолжить проверку по актуальному дереву EN-источников и инвентаризации после `ars_creo`, выбрать следующие десять непроверенных namespace. FTB Quests/SNBT оставить на заключительный этап.


## Пятая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace** после `ars_creo`: `ars_elemancy`, `ars_elemental`, `ars_ocultas`, `ars_technica`, `ars_unification`, `arseng`, `artifacts`, `auroral`, `auroras`, `balm`. Всего **1 722 ключа**. JSON корректен во всех файлах; missing 0, extra 0, duplicates 0, placeholder/format/newline/whitespace mismatches 0. Два пустых значения Ars Elemental совпадают с EN и сохранены. Необоснованных совпадений пользовательского текста RU=EN не обнаружено; существующие переводы не переписывались.

## Шестая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `bhc`, `bellsandwhistles`, `betteradvancedtooltips`, `betteradvancements`, `betterfortresses`, `bettermineshafts`, `betteroceanmonuments`, `betterstrongholds`, `betterwitchhuts`, `bigreactors`. Всего **717 ключей**. Во всех файлах JSON корректен; missing 0, extra 0, duplicates RU 0, empty 0, placeholder/format/newline/whitespace mismatches 0. В EN Big Reactors повторяется только служебный ключ `_comment` (31 объявление); иных дубликатов нет.

В Big Reactors переведены 13 оставшихся пользовательских строк энергизатора и подпись Name. Добавлены термины Extreme Reactors в глоссарий. Коммиты: [64aa65e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/64aa65e1036b819ff400c362917d370cf7be4ca7), [91bccf6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/91bccf6fb0b383c8d5c7f2f701e42977d043ee5), [d312883](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d3128835dddef70e1303370e1cae75baa0bbccbb).

**Итого за две партии: 20/20 namespace, 2 439 ключей.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Следующая точка продолжения — после `bigreactors` сверить следующие namespace по актуальному EN-дереву и исключить ранее проверенные YUNG's Better Desert Temples, Dungeons, End Island и Jungle Temples. FTB Quests/SNBT не затрагивать до заключительного этапа.


## Седьмая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `extremesoundmuffler`, `farmersdelight`, `fastbench`, `fluxnetworks`, `framedblocks`, `gateways`, `glassential`, `gmut`, `hostilenetworks`, `immeng`. Всего **1 668 ключей**. JSON корректен; missing 0, extra 0, duplicates RU 0, placeholder mismatches 0. Единственное пустое значение Hostile Neural Networks совпадает с EN. Все переносы строк и пробелы после исправлений совпадают с оригиналами. Семь дополнительных серых `§8` маркеров в FramedBlocks сохранены как намеренное оформление обозначений направлений. В EN Hostile Neural Networks повторяется только служебный ключ `_comment` (9 объявлений).

В Hostile Neural Networks исправлены переносы, формулировки и неточности описаний мобов; в Gateways восстановлен завершающий перенос; в FramedBlocks удалён лишний пробел и уточнено название блока. Глоссарий дополнен терминологией трёх модов. Коммиты: [FramedBlocks](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fb74887bbcd2a0702285445d9b0b0c0bf35e8fe2), [Gateways](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d190753758117d33ab676f3e3b51c36a5fc6b676), [Hostile Neural Networks](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8dafd6385d8f0b43fa16bacb9dcdc1adadea0d06), [глоссарий](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a805b6080e5371cfa054e7b76f1f8723e7c26a57).

**Итого за три партии после Ars Creo: 30/30 namespace, 4 107 ключей.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Следующая точка продолжения — сверка следующих namespace после `immeng` с актуальным EN-деревом и INVENTORY, исключая уже проверенные локализации. FTB Quests/SNBT не затрагивать до заключительного этапа.


## Восьмая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `immersiveengineering`, `ironjetpacks`, `jade`, `jei_mekanism_multiblocks`, `justenoughprofessions`, `keybindspurger`, `cataclysm`, `measurements`, `moderndynamics`, `modern_industrialization`. Всего **5 197 ключей**. JSON корректен; missing 0, extra 0, duplicates RU 0, placeholder/format/newline/whitespace mismatches 0. Два пустых значения совпадают с EN. В EN Cataclysm повторяется `maledictus_hurt.sub`; корректным является последнее значение `Maledictus dies`, и RU содержит его перевод. В EN Measurements трижды встречается только служебный `_comment`.

В Cataclysm удалён лишний завершающий пробел в названии Abyss Portal; термин добавлен в глоссарий. Коммиты: [Cataclysm](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/903d7cc3cce5dccb858f7a79bb49c14460f6c897), [глоссарий](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2897448949ff6b2a8582f8b818099b190fb678ce).

**Итого за четыре партии после Ars Creo: 40/40 namespace, 9 304 ключа.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Позже при сверке порядка EN-дерева обнаружен пропущенный блок B–C перед `extremesoundmuffler`; он проверен в девятой партии ниже. Актуальная точка продолжения после `caelus`. FTB Quests/SNBT не затрагивать до заключительного этапа.


## Девятая партия JSON-аудита завершена — 06.11.2026

После повторной проверки порядка namespace по EN-дереву выявлен пропущенный блок B–C между `bigreactors` и ранее обработанным `extremesoundmuffler`. Проверены **10/10 namespace**: `biomeswevegone`, `blockui`, `bookshelf`, `botanypots`, `brandonscore`, `bridgingmod`, `buildinggadgets2`, `bwncr`, `cabletiers`, `caelus`. Всего **2 143 ключа**. JSON корректен; missing 0, extra 0, duplicates 0, placeholder/format/newline/whitespace mismatches 0. Семь пустых значений Bookshelf/Botany Pots совпадают с EN и относятся к служебным разделителям/метаданным. Необоснованных совпадений пользовательского текста RU=EN не обнаружено. Изменения переводов не потребовались.

**Итого за пять партий после Ars Creo: 50/50 namespace, 11 447 ключей.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Актуальная следующая точка — после `caelus`; продолжить сверку EN/RU namespace по порядку, пропуская только те файлы, которые уже документально проверены. Ранее обработанные `extremesoundmuffler`–`modern_industrialization` остаются завершёнными и не требуют повторной работы. FTB Quests/SNBT не затрагивать до заключительного этапа.


## Десятая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `camol`, `charginggadgets`, `chisel`, `chromacarvings`, `cloudglass`, `cobblegengalore`, `codechickenlib`, `colorfulhearts`, `comforts`, `common_storage_lib`. Всего **2 999 ключей**. JSON корректен; missing 0, extra 0, duplicates 0, empty 0, placeholder/format/newline/whitespace mismatches 0. Пять совпадений RU=EN — название Chisel, обозначение RF и технический шаблон. Изменения переводов не потребовались.

**Итого за шесть партий после Ars Creo: 60/60 namespace, 14 446 ключей.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Актуальная следующая точка — после `common_storage_lib`; продолжить с `commoncapabilities`, исключая ранее проверенные namespace. FTB Quests/SNBT не затрагивать до заключительного этапа.


## Одиннадцатая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `commoncapabilities`, `compactmachines`, `connectedglass`, `constructionstick`, `controlling`, `cookingforblockheads`, `copycats`, `cosmeticarmorreworked`, `crafting_on_a_stick`, `craftingtweaks`. Всего **728 ключей**. JSON корректен; missing 0, extra 0, duplicates RU 0, placeholder/format/newline/whitespace mismatches 0. Три пустых значения совпадают с EN. В EN Common Capabilities повторяется только служебный `_comment` (3 объявления). В Cooking for Blockheads восстановлены две экранированные последовательности `\\n` из оригинала; коммит [5223759](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/522375983dbeb003719b937ad7ec01759c712396).

**Итого за семь партий после Ars Creo: 70/70 namespace, 15 174 ключа.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Актуальная следующая точка — после `craftingtweaks`; блок C–C завершён в двенадцатой партии ниже. FTB Quests/SNBT не затрагивать до заключительного этапа.


## Двенадцатая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `crashutilities`, `create`, `create_aquatic_ambitions`, `create_enchantment_industry`, `create_hypertube`, `createaddition`, `creeperoverhaul`, `cristellib`, `crystalix`, `curios`. Всего **4 805 ключей**. JSON корректен; missing 0, extra 0, duplicates 0, placeholder/format/newline/whitespace mismatches 0. Семь пустых значений Create совпадают с EN; порядок плейсхолдеров во всех файлах проверен отдельно и совпадает.

В Create Enchantment Industry переведены 332 ранее полностью английских значения; четыре оставшихся совпадения являются техническими шаблонами. Исправлены пробелы в Create и порядок аргументов в двух сообщениях Curios. Обновлён глоссарий. Коммиты: [Create Enchantment Industry](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/23759eeabfb0f3119424de610551fe5d6fcfd9ce), [Create](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ebce9d7983f266e5eefb388ba62f5ad5fec83133), [Curios](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9921f5d7c878ca73eecf959d42845002f123d6da), [глоссарий](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9f96cd8fcd9b490e71de53c87fc963029bb6e1a4).

**Итого за восемь партий после Ars Creo: 80/80 namespace, 19 979 ключей.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Актуальная следующая точка — после `curios`; блок D–E проверен в тринадцатой партии ниже. FTB Quests/SNBT не затрагивать до заключительного этапа.


## Тринадцатая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `darkmodeeverywhere`, `deeperdarker`, `dungeons_arise`, `easy_villagers`, `elevatorid`, `enderstorage`, `extendedae`, `enderdrives`, `endermanoverhaul`, `enderio`. Всего **1 728 ключей**. JSON корректен; missing 0, extra 0, duplicates 0, empty 0, placeholder/format/newline/whitespace mismatches 0. В Ender IO переведены три пользовательские подписи слотов фильтров; глоссарий обновлён. Коммиты: [Ender IO](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4f1d56b283223434b20c2ef7541572db199ac09e), [глоссарий](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c3e9a24a11d2c1c1aa72ee553d71beea0ba08389).

**Итого за девять партий после Ars Creo: 90/90 namespace, 21 707 ключей.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Актуальная следующая точка — после `enderio`; блок FTB и Functional Storage проверен в четырнадцатой партии ниже. FTB Quests/SNBT не затрагивать до заключительного этапа.


## Четырнадцатая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `farmingforblockheads`, `ftbchunks`, `ftbessentials`, `ftbfiltersystem`, `ftblibrary`, `ftbteams`, `ftbultimine`, `functionalstorage`, `fusion`, `mcwfurnitures`. Всего **1 708 ключей**. JSON корректен; missing 0, extra 0, duplicates 0, empty 0, placeholder/format/newline/whitespace mismatches 0. В FTB Ultimine исправлен перенос строки в описании настройки. `ftbjeiextras` и `ftbxmodcompat` исключены из подсчёта: EN-файлы содержат пустые JSON-объекты без ключей. FTB Quests не затрагивался. Коммит [FTB Ultimine](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e3dbc2e3e1d133526319528848c437519f0023e6).

**Итого за десять партий после Ars Creo: 100/100 namespace, 23 415 ключей.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Актуальная следующая точка — после `mcwfurnitures`; блок мебели и JourneyMap завершён в пятнадцатой партии ниже.


## Пятнадцатая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `refurbished_furniture`, `guideme`, `handcrafted`, `jearchaeology`, `jei`, `jeistuff`, `journeymap`, `jupiter`, `justenoughbreeding`, `justzoom`. Всего **1 847 ключей**. JSON корректен; missing 0, extra 0, duplicates 0, empty 0, placeholder/format/newline/whitespace mismatches 0.

В JourneyMap переведены 819 пользовательских значений из 868 совпадавших с английским оригиналом. Оставшиеся 49 значений — намеренно сохранённые бренды, домены, координатные обозначения, цветовые сокращения, единицы и технические шаблоны. Заключительная проверка выявила и исправила три расхождения переносов/описаний. История изменений: [коммиты ветки](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commits/work/irons-spells-nov05), [последняя коррекция](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ab6d3095d1cc13969053534faee9c1a5e5fce5f4), [глоссарий](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e5064d64f5c3ee4ddf77c46fbe89d56d6e5973b8).

**Итого за одиннадцать партий после Ars Creo: 110/110 namespace, 25 262 ключа.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Актуальная следующая точка — после `justzoom`; блок K–L завершён в шестнадцатой партии ниже.


## Шестнадцатая партия JSON-аудита завершена — 06.11.2026

Проверены **10/10 namespace**: `keybindbundles`, `kubejstweaks`, `laserbridges`, `laserio`, `lionfishapi`, `little_big_redstone`, `livingthings`, `logisticsnetworks`, `lootr`, `luminax`. Всего **1 729 ключей**. JSON корректен; missing 0, extra 0, duplicates 0, empty 0, placeholder/format/newline/whitespace mismatches 0. Все совпадения RU=EN являются техническими/брендовыми или математическими обозначениями. Изменения переводов не потребовались.

**Итого за двенадцать партий после Ars Creo: 120/120 namespace, 26 991 ключ.** Работа опубликована в `work/irons-spells-nov05`; `main` не изменялся. Актуальная следующая точка — после `luminax`; продолжить с Mahou Tsukai и следующими namespace, пропуская ранее проверенные. FTB Quests/SNBT оставить на заключительный этап.

## Семнадцатая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** Mahou Tsukai, McJtyLib, Macaw's Bridges, Macaw's Doors, Macaw's Holidays, Macaw's Lights, Macaw's Fences, Macaw's Paths, Macaw's Stairs и Macaw's Windows. Всего **3 918 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликаты RU 0; несовпадения плейсхолдеров, форматирования, переносов строк и пробелов — 0. В Mahou Tsukai 81 пустое значение совпадает с EN; 14 непустых совпадений RU=EN являются брендом, именами, пунктуацией и буквенными обозначениями. В McJtyLib два совпадения — служебный комментарий и название библиотеки. В остальных восьми namespace совпадений RU=EN нет.

В Mahou Tsukai удалён один лишний ключ, исправлены два лишних плейсхолдера и согласованы термины Caliburn, Borrowed Authority и несколько названий техник. В Macaw's Windows исправлен перевод Window Key по описанию предмета. Глоссарий дополнен терминологией обеих групп.

Коммиты:
- Mahou Tsukai: перевод [26f8fc0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/26f8fc007bfebe544363e5d9782ff20da8cc6a8b), глоссарий [9859cc3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9859cc3ccbbb9d14fc22b1b90fbd37c76100e484).
- Macaw's Windows: перевод [c0b64dd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c0b64ddd06df2eb03c8870189a739d709734ab82), глоссарий [58b2e98](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/58b2e980a733ef98ba606e5a40d2262543206db4).
- Остальные восемь namespace проверены; исправления не требовались.

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: mcwroofs, mcwtrpdoors, megacells, mekanismcovers, mekanisticrouters, memorysettings, merequester, merrymaking, mffs, mifa. Уже завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## Восемнадцатая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** Macaw's Roofs, Macaw's Trapdoors, MegaCells, Mekanism Covers, Mekanistic Routers, Memory Settings, ME Requester, Merrymaking, MFFS и MIFA. Всего **1 657 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликаты RU 0; несовпадения плейсхолдеров, форматирования, переносов строк и начальных/конечных пробелов — 0. В EN Merrymaking один ключ повторён с тем же значением; RU содержит его один раз. Единственное пустое значение Merrymaking совпадает с EN. Совпадения RU=EN в Merrymaking/MFFS — пустая строка и технические обозначения.

Исправлены терминология и форматирование в MegaCells, Mekanistic Routers, Memory Settings, ME Requester, Merrymaking и MFFS. Глоссарий дополнен соответствующими терминами. В Macaw's Roofs, Macaw's Trapdoors, Mekanism Covers и MIFA исправления не потребовались.

Коммиты переводов: MegaCells [addd475](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/addd475bab0bc2a977eeaffb379d5607cefb5bb6); Mekanistic Routers [e597e87](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e597e8712f611a7cd413d249f6db5477d1f6a10b), [e85eb01](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e85eb01d30e3b97970f542338617d3f8ab32331c); Memory Settings [9e329e4](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9e329e4d04764ec4642d158bbc4a93eff6e4d496); ME Requester [9120c52](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9120c52c6fe50f0ada44ae0a400e03834508be03); Merrymaking [38a53dc](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/38a53dcff5f807841a720556a84ae799c245e813), [b20f1cd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b20f1cd2f088287097996a8a84928e6ae623d8c9), [cc3ad21](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cc3ad21ca85ee3123cb92a405c64642d6b198c18); MFFS [a8eb5f8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a8eb5f8cecc96ab7a954912c2f4bef354729dc60), [988d6a8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/988d6a8975ffaeaac16d35b8a2206e9d51915f5e). Глоссарий [5fb453b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5fb453b56630d2d1343e9b50b1e4a7a6d20c984f), [6704118](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/67041181eda9efeed639cbf98770896bd6437039).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: minecolonies, mininggadgets, mob_grinding_utils, modernfix, modonomicon, modularrouters, modularbees, mes, mns, mss. Ранее завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## Девятнадцатая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** MineColonies, Mining Gadgets, Mob Grinding Utils, ModernFix, Modonomicon, Modular Routers, Modular Bees, Moog's End Structures, Moog's Nether Structures и Moog's Soaring Structures. Всего **4 994 ключа**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликаты RU 0; несовпадения плейсхолдеров, форматирования, переносов строк и пробелов — 0. В EN Mob Grinding Utils повторяется служебный ключ _comment (10 раз); последнее значение — Item Tool tips, RU содержит его перевод. Пять пустых значений совпадают с EN. Оставшиеся совпадения RU=EN являются брендами, техническими шаблонами, единицами, символами операторов и смайликом.

В Modular Routers переведены оставшиеся пользовательские строки и исправлены неполные подсказки. В MineColonies исправлены шесть расхождений пробелов. В Mob Grinding Utils переведён служебный комментарий. В ModernFix исправлено описание кэширования состояний блоков и восстановлен абзац. Глоссарий дополнен.

Коммиты: Modular Routers [c400bd5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c400bd551ce455078c04e8cdb54e23b3629394ce), [4f2964c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4f2964c75f47603c2b773f253f053df76ca55aa0); MineColonies [87d8bf6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/87d8bf6dfcfdd74cf933795f3320ff2a85ba0a38); Mob Grinding Utils [2cb4b64](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2cb4b64ac6f62d14e2528f23d84d7013e554249f); ModernFix [788024a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/788024ac9fede2b6bec4117cda97378ec8f3a277); глоссарий [6b5515c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6b5515c3074bddf54f656e18575040010730a61b), [8c1ad18](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8c1ad185cc02d9d1548a43eea93e97d9838d1403), [ae1ab43](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ae1ab43b0222a30682fa605904021ecf0cf4b241).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: moogs_structures, mvs, moonlight, moreoverlays, morered, mostructures, multipiston, mysticalagradditions, mysticalagriculture, naturesaura. Ранее завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## Двадцатая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** Moog's Structure Lib, Moog's Voyager Structures, Moonlight, More Overlays Updated, More Red, Mo' Structures, Multi-Piston, Mystical Agradditions, Mystical Agriculture и Nature's Aura. Всего **1 497 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликаты 0; несовпадения плейсхолдеров, форматирования, переносов строк и пробелов — 0. 21 совпадение RU=EN — названия модов/сервисов, координатные обозначения, числовые уровни и технические шаблоны.

Исправлены термины ресурсных уровней Mystical Agriculture, согласование названий трёх предметов и Ancient Log в Nature's Aura. Глоссарий дополнен.

Коммиты: Mystical Agradditions [00dfc30](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/00dfc300d95d2ed3095374efadef68107d307bc9); Mystical Agriculture [c975d3a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c975d3a0b00d21a8d78517bda1e39131f1b5cb6e), [795fd3a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/795fd3a54db0c6f7700600ee510f89b01ce3aec4); Nature's Aura [a959245](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a9592457d1a721de736a1dccefa61b09be3a9fd2); глоссарий [dbadc93](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/dbadc93e7ffb574d9bfe6f21590a14785a45360c).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: neo_auth, nochatreports, notenoughanimations, not_enough_glyphs, observable, oracle_index, owo, pamhc2crops, pamhc2foodcore, pamhc2foodextended. Nature's Compass, NeoVitae, Occultism, Biomes We've Gone, Oritech и PneumaticCraft уже завершены и пропускаются. FTB Quests/SNBT оставить на заключительный этап.

## Двадцать первая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** NeoAuth, No Chat Reports, Not Enough Animations, Not Enough Glyphs, Observable, Oracle Index, owo-lib, Pam's HarvestCraft 2 Crops, Food Core и Food Extended. Всего **2 030 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликаты верхнего уровня 0; несовпадения плейсхолдеров, форматирования, переносов строк и пробелов — 0. В OWO сохранена структура JSON-компонентов и индексные плейсхолдеры. Единственное пустое значение Not Enough Glyphs совпадает с EN. 17 совпадений RU=EN — бренды/названия модов, технические идентификаторы, клавиши, алгоритмы и числовые/структурные шаблоны.

В No Chat Reports исправлены 12 буквальных последовательностей \\n, которые вместо переносов строк отображались как текст. Глоссарий дополнен терминами Pam's HarvestCraft.

Коммиты: No Chat Reports [d07da48](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d07da48559be4f0b4e7e064d31674aa87d6dd9bc); глоссарий [8f098d5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8f098d567b89e46220b4e04fb5b5250faf73965c).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: pamhc2trees, patchouli, pipez, placebo, pocketstorage, polylib, polymorph, potionsmaster, productivebees и productivemetalworks. Productive Bees ранее уже переводился; не перезаписывать существующие значения, только сверить и исправить подтверждённые ошибки. FTB Quests/SNBT оставить на заключительный этап.

## Двадцать вторая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** Pam's HarvestCraft Trees, Patchouli, Pipez, Placebo, PocketStorage, PolyLib, Polymorph, Potions Master, Productive Bees и Productive Metalworks. Всего **1 899 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликаты 0; несовпадения плейсхолдеров, форматирования, переносов строк и пробелов — 0. 16 совпадений RU=EN — названия модов, технические идентификаторы, клавиши и плейсхолдеры.

В Productive Bees локализованы 117 продвинутых ульев и 117 расширителей ульев с вариантами пород древесины; исправлены достижения и подсказки. В Pipez согласованы названия уровней улучшений, в Placebo — косметические эффекты для спонсоров. В Pam's HarvestCraft Trees восстановлены три завершающих пробела. Глоссарий дополнен.

Коммиты: Productive Bees [f7fa64c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f7fa64c66fa40d78093fbfba148858696dfff573), [c62cb6b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c62cb6bbf267d04e5d09cf28079a9963f18730b5); Pipez [311aae7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/311aae7c4f7b55de5814a4ca12684191b33d2411); Placebo [a10a081](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a10a0816e7d7f525b9062b6ea8535b6a8149e5e4); Pam's HarvestCraft Trees [cd33c14](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cd33c14c752157f1dc910c211c7115c0b8462255); глоссарий [d0c2ecd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d0c2ecdd5cd4a246db21d4c025a1ac9de8de648a), [6ed7ef1](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6ed7ef1066ba364d91882c2265e95831d3257cbf).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: rangedpumps, rechiseledcreate, redstonepen, refinedtypes, refinedfluidsubstitution, refinedstorage_curios_integration, refinedstorage_jei_integration, refinedstorage_mekanism_integration, refinedstorage, refinedstorage_quartz_arsenal. Ранее завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## Двадцать третья партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** Ranged Pumps, Rechiseled Create, Redstone Pen, Refined Types, Refined Fluid Substitution, Refined Storage Curios Integration, Refined Storage JEI Integration, Refined Storage Mekanism Integration, Refined Storage и Refined Storage Quartz Arsenal. Всего **1 349 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликаты 0; несовпадения плейсхолдеров, форматирования, переносов строк и пробелов — 0. 12 совпадений RU=EN — названия модов/интеграций, JEI, клавиши/технические идентификаторы и шаблон плейсхолдеров.

В Redstone Pen исправлены переносы и коды форматирования в трёх подсказках RLC. В Refined Storage переведены десять оставшихся пользовательских строк и исправлены три лишних переноса. Глоссарий дополнен.

Коммиты: Redstone Pen [15732cd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/15732cdd82eda464e288e88f0c7905afffeea311); Refined Storage [d42aa73](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d42aa738c30c9e9000cb5379299e9d68985c6df8), [4274337](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4274337b955cae44af83dd53b21477cdc3e529c1); глоссарий [edb01da](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/edb01dae26cac69495c4635a5ea354f065584f13).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: rsinsertexportupgrade, reliquified_artifacts, repeatable_trial_vaults, repurposed_structures, resourcefulconfig, restrictions, rftoolsbase, rftoolsbuilder, rftoolspower, rftoolsstorage. Ранее завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## Двадцать четвёртая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** RS Insert Export Upgrade, Reliquified Artifacts, Repeatable Trial Vaults, Repurposed Structures, Resourceful Config, Restrictions, RFTools Base, RFTools Builder, RFTools Power и RFTools Storage. Всего **1 078 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликаты 0; несовпадения плейсхолдеров, форматирования, переносов строк и пробелов — 0. Пять совпадений RU=EN — названия модов/категорий и техническая подпись UUID.

В Reliquified Artifacts исправлен порядок %2$s и %3$s в описании Shock Pendant: теперь дальность и количество перескоков соответствуют EN-оригиналу.

Коммит: Reliquified Artifacts [b5f8ba3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b5f8ba34bc9d8f47bbf172129806dc4945b6d43e).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: rftoolsutility, rootsclassic, sawmill, searchables, sgearmetalworks, shiny, shrink, silentlib, silentgems и simplebackups. Silent Gear уже завершён и пропускается. FTB Quests/SNBT оставить на заключительный этап.

## Двадцать пятая партия JSON-аудита завершена — 06.11.2026

**Подтверждено 10/10 namespace:** RFTools Utility, Roots Classic, Sawmill, Searchables, Silent Gear Metalworks, Shiny, Shrink, Silent Lib, Silent Gems и Simple Backups. Всего **1 178 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликаты 0; несовпадения плейсхолдеров, форматирования, переносов строк и пробелов — 0. Два пустых значения Roots Classic совпадают с EN. Шесть совпадений RU=EN — название Roots Classic, плейсхолдер, save-all/Mc2Discord и технические обозначения.

В Roots Classic удалён лишний начальный пробел в заголовке Wildwood Boots. Коммит: [51e15d7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/51e15d76edd4c431bd998535f0c375cbcd742327).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: simplemagnets, simple_weather, simplylight, smithingtemplateviewer, solcarrot, sophisticatedbackpacks, sophisticatedcore, sophisticatedstorageinmotion и soulplied_energistics, starbunclemania. Sophisticated Storage уже завершён и пропускается. FTB Quests/SNBT оставить на заключительный этап.


## Точечная сверка альтернативных формулировок batch — 06.11.2026

Начата ручная сверка альтернативных значений из сохранённой ветки `work/atm10-batch-nov05` с текущими переводами `main` и английскими оригиналами. В пяти файлах обнаружено 638 отличающихся значений; различия не являются пропущенными ключами. Автоматическое массовое копирование не выполнялось: выбор делается только там, где альтернативная формулировка действительно лучше и сохраняет смысл оригинала.

В `assets/evilcraft/lang/ru_ru.json` улучшены две формулировки по результатам сравнения: Bare Rod переведён как «заготовка стержня» вместо буквального «голый стержень»; описание Булавы искажения переформулировано для естественного описания накопления сферы. Термины Bare Rod, Brush и Cap добавлены в `GLOSSARY.md`.

Коммиты main: EvilCraft [8c4e205](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8c4e2058b3b89b6ec2d890fddb58c772bc0e8159); GLOSSARY [48766e3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/48766e3d69eb25ab7eb32d82fe782caac4b23955).

Сверка 638 отличий ещё не завершена. Ветки `main` и `work/atm10-batch-nov05` сохранены; batch не сливать целиком. Следующий шаг — продолжить ручную сверку оставшихся отличий в EvilCraft, затем Integrated Dynamics, Iron's Spells 'n Spellbooks, PneumaticCraft и Reliquary, перенося в main только подтверждённые улучшения.


Дополнительно в `assets/pneumaticcraft/lang/ru_ru.json` переработаны подсказки GPS Tool и GPS Area Tool: инструкции сокращены до компактных пошаговых команд ПКМ/ЛКМ и SHIFT + прокрутка колёсика, при этом сохранены все действия из английского оригинала.

Коммит main: PneumaticCraft [a488a1d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a488a1d95ed6ee91b1047d880bcdc51ae022f52f).


## Завершение отбора улучшений из work/atm10-batch-nov05 — 06.11.2026

Сопоставлены альтернативные формулировки пяти RU-файлов из `work/atm10-batch-nov05` с актуальными EN-оригиналами и текущими версиями `main`. Batch не объединялся целиком: в нём много более ранних формулировок с неточностями, лишними пояснениями, неестественными кальками и несогласованной капитализацией. В `main` перенесены только выбранные улучшения; остальные альтернативы не дают оснований заменять более точные текущие значения.

Внесённые улучшения:
- **EvilCraft:** уточнено описание Булавы искажения; унифицированы краткие подсказки управления через ПКМ; улучшено описание Колоссального кровавого сундука.
- **Integrated Dynamics:** `Logic Programmer` последовательно переименован в «Программатор логики» (включая портативный вариант и записи книги); улучшены описание вычитания составных NBT-тегов, подсказки копирования настроек/аспектов гаечным ключом и инструкция по смещениям.
- **Iron's Spells 'n Spellbooks:** исправлена формулировка сообщения о смерти от брошенного предмета.
- **PneumaticCraft:** сокращены обозначения кнопок в подсказке Ghost Slot; уточнено название настройки анимации таблички с афоризмами.
- **Reliquary:** уточнены названия Rending Gale («Раздирающий вихрь») и Mob Charm («Оберег от мобов»).
- **GLOSSARY.md:** добавлены 31 термин из альтернативной партии; уточнены Logic Programmer, Rending Gale и Mob Charm.

Контроль актуальных файлов в main после изменений: JSON корректен; ключи EN/RU совпадают полностью; missing 0; extra 0; дубликаты 0; несовпадения плейсхолдеров 0; несовпадения токенов форматирования Minecraft 0.

| Файл | Ключей EN/RU | Missing | Extra | Дубликаты | Placeholders | Format tokens |
|---|---:|---:|---:|---:|---:|---:|
| EvilCraft | 629/629 | 0 | 0 | 0 | 0 | 0 |
| Integrated Dynamics | 1854/1854 | 0 | 0 | 0 | 0 | 0 |
| Iron's Spells 'n Spellbooks | 1315/1315 | 0 | 0 | 0 | 0 | 0 |
| PneumaticCraft | 2274/2274 | 0 | 0 | 0 | 0 | 0 |
| Reliquary | 551/551 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **6623/6623** | **0** | **0** | **0** | **0** | **0** |

Коммиты main:
- EvilCraft: [8c4e205](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8c4e2058b3b89b6ec2d890fddb58c772bc0e8159), [e04fb9e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e04fb9e863769cf26c8dfe5b870c039a30825e0c), [74c3f66](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/74c3f66b2f7f9acebe5c3af78fec4d389042257e).
- Integrated Dynamics: [c2c0fc8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c2c0fc870ab3760880bdae14956e07f5b86b2e9a), [27bc693](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/27bc6932a5bac813034f94f583c91fc25f1353a6).
- Iron's Spells 'n Spellbooks: [5b9b269](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5b9b2694410bac0c9f46f0d8b8130d4e142047b9).
- PneumaticCraft: [f02d276](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f02d27612dd1add368a67462e9980874fa1be4c3), [1357e48](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1357e48a0b399a8536002ea050e06e8ab7d6d178).
- Reliquary: [681a1df](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/681a1df4137be362a99d312146a1acc398641874).
- GLOSSARY: [caf1bdd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/caf1bdd2c4455f67be8d15a64e0886ed15dd512e).

Ветка `work/atm10-batch-nov05` больше не нужна для дальнейшей работы: её полезные терминологические дополнения и отобранные формулировки перенесены в main; неперенесённые варианты не содержат недостающих ключей и не должны автоматически заменять текущие переводы. После удаления ветки продолжать работу только в `main`.


## Полный круг технической и смысловой вычитки — партия 1 после StarbuncleMania — 06.11.2026

Завершена ручная смысловая вычитка и повторная техническая сверка следующих **10 namespace** непосредственно в `main`:

| Namespace | EN/RU ключей | Missing | Extra | Дубликаты | Плейсхолдеры (с позициями) | Форматирование | Переносы | Краевые пробелы |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| simplemagnets | 38/38 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| simple_weather | 19/19 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| simplylight | 192/192 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| smithingtemplateviewer | 1/1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| solcarrot | 60/60 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| sophisticatedbackpacks | 407/407 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| sophisticatedcore | 318/318 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| sophisticatedstorageinmotion | 8/8 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| soulplied_energistics | 4/4 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| starbunclemania | 150/150 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **1 197/1 197** | **0** | **0** | **0** | **0** | **0** | **0** | **0** |

Во всех десяти JSON корректны. Проверены точные наборы ключей, дубликаты, пустые значения относительно EN, порядок и типы позиционных плейсхолдеров, коды форматирования, количество переносов строк и начальные/конечные пробелы. В StarbuncleMania одно пустое значение оставлено пустым, поскольку оно пустое и в EN-оригинале. Пропусков и лишних ключей нет.

### Результаты смысловой вычитки и исправления

- **Simply Light:** исправлена большая группа названий блоков с ошибками рода и капитализации: панели, плиты, лампочки, блоки, стержни и колонны. Исправлены описания световых блоков/панелей/стержня, нижнего и верхнего краевого светильника, подсказка клавиши Shift. Убраны оставшиеся фрагменты машинного перевода.
- **Simple Weather:** исправлена смысловая ошибка настройки AABB: EN `Calculate AABB`, RU теперь «Рассчитывать AABB», а не «Использовать кэшированный AABB».
- **SoL Carrot:** «Boring Foods Tasted» уточнено как «Попробовано непитательных блюд».
- **Sophisticated Backpacks:** исправлены описания загрузки/выгрузки и пополнения, механики переплавки/плавки, батареи и резервуара, насоса, мультиинструмента и ловца мобов. Термин Stack Upgrade приведён к смыслу увеличения вместимости слота; Inception Upgrade — к вложению рюкзаков. Уточнены статусы ловца мобов, шаблоны и ряд конфигурационных подписей.
- **Sophisticated Core:** выправлены формулировки Ender Linker, фильтров, переполнения, помпы опыта, настроек вкладок и экспорта SNBT. Исправлены единицы мБ и сообщения о вместимости. В сообщении с переставленными аргументами сохранена точная позиционная адресация `%1$d`, `%2$s`, `%3$s`.
- **StarbuncleMania:** термин Starbuncle унифицирован с GLOSSARY как «звездоух», Drygmy — «дригми». Исправлены газовая единица измерения, Sourcelink/Source Condenser и связанные строки на «Исток», а также несколько описаний книги.
- **Simple Magnets, Smithing Template Viewer, Sophisticated Storage In Motion и Soulplied Energistics:** проверены по EN-контексту; смысловых правок, требующих внесения, не обнаружено.
- **GLOSSARY.md:** дополнены термины Simply Light и Sophisticated Storage, уточнены Stack Upgrade и добавлена Fluid Sourcelink.

### Коммиты main

- Simply Light: [0443afc](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0443afc4ea879061ab80900c851ded2342dbc021), [744ba9a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/744ba9a0ddb15ce9689bec638b2f7d2cd9daae43).
- Simple Weather: [c7f4115](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c7f41159d4893feb3b0b79c0d226c395df6abd44).
- SoL Carrot: [b7f979d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b7f979d7f853509a1c2badbd9b1fecd6d866cb53).
- Sophisticated Backpacks: [67742f2](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/67742f2716405be091e7aae809cf7e651355eb3d), [4e35920](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4e3592087eebab69c5e4cd9977ce283fd2cebf44), [0bf7d8d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0bf7d8d93fb3fe27d4e0252a63b04b03cc331661).
- Sophisticated Core: [f871599](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f871599f4a404728ce67fa1c530279d67a366201), [12e8cbd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/12e8cbd317b8844fdff90107d4b6ef9c0d759b0e), [ebe12f9](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ebe12f94648182fa5f3a75b97c711f3415d548ef), [38854bd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/38854bde8c7c23f827141f777c13a53c3ca116b6).
- StarbuncleMania: [9396737](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/939673754c223aaf04640c2ae468db140adb5b82), [9ab3233](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9ab3233f938129172a53dd7b62a076262b6b2221), [52c04c2](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/52c04c2315bae602db2983fccb172499d7246ed3), [2ee876d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2ee876d6d08046dd1dc90e0a42102937b5cd5a53), [0a0e992](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0a0e992e8d349116b3ee647e787f6113ecf66a7b).
- GLOSSARY: [a380e9e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a380e9e4be041f82a53dc16c120a00e8099b4a65), [6d371fd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6d371fdcf326977be4ffdc3475cf1c34eaa2f901).

Следующая незавершённая десятка по текущему дереву RU/EN: `stepcrafter`, `storagedelight`, `structurize`, `supermartijn642corelib`, `sushigocrafting`, `terrablender`, `the_bumblezone`, `theurgy`, `tiab`, `titanium`. Ранее проверенные `stevescarts`, `supplementaries`, `tempad` и `tempad_static` повторно не включать. Продолжать в `main`.


## Историческая контрольная точка перед паузой — 06.11.2026

> Эта запись описывает состояние до возобновления работ. Все незавершённые пункты ниже закрыты в следующем разделе «Завершение полной вычитки партии stepcrafter—titanium». Актуальная точка продолжения указана в конце последнего раздела.

Пользователь остановил работу и попросил зафиксировать состояние до следующего продолжения. Ничего не считать завершённым сверх того, что подтверждено ниже.

### Завершённая первая партия вычитки

Первая десятка после StarbuncleMania (simplemagnets, simple_weather, simplylight, smithingtemplateviewer, solcarrot, sophisticatedbackpacks, sophisticatedcore, sophisticatedstorageinmotion, soulplied_energistics, starbunclemania) уже описана выше: 10 namespace, 1197 ключей, техническая проверка без зарегистрированных расхождений. Смысловые правки опубликованы в main.

### Состояние следующей десятки на момент паузы

В работе/частично вычитаны следующие namespace: stepcrafter, storagedelight, structurize, sushigocrafting, the_bumblezone, theurgy, titanium. По ним есть реальные опубликованные смысловые правки; это **не означает**, что вся десятка завершена. По supermartijn642corelib, terrablender и tiab завершение не подтверждено. Полный повторный технический аудит этой десятки ещё не зафиксирован.

Подтверждённые коммиты в main:
- StepCrafter: [86e4505](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/86e45058364041c5f25a37eda43763b12012c9f1) — уточнено название улучшения слотов.
- Storage Delight: [c28ba9a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c28ba9a9885a00a1d3400b18eba729028e791180), [0e2e828](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0e2e82834f2008b1a6aef607b2eb2c9c4c372f2c), [bab298b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bab298bcad2f152e85c0c2735f46350bd669901b) — сверены/очищены ключи относительно EN и исправлены названия кухонных блоков.
- Structurize: [5dc80a4](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5dc80a4a6a121caf57c327c571a8b3789c27a301), [68938b0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/68938b01f4c39ac3a65b332b65c53f8b57d8ed1e) — уточнены подсказки инструмента сканирования, интерфейса схем и конфигурации.
- Sushi Go Crafting: [67b02c5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/67b02c5f49433aaef1c13818d92cc89871a4388f) — улучшена пищевая терминология.
- The Bumblezone: [caa9e7c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/caa9e7cc78cbb8cba0d0b39b991566dd7584cb82), [730c8cd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/730c8cdc213165d7bfbf0047c94d97f81266308e) — вычитаны описания и конфигурационные строки, сохранены исходные пробелы.
- Theurgy: [82239c7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/82239c73eaa11876398729251eab62bc0b1f2b3d), [755004c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/755004c58eab408ee553e142110017cb6d76005e) — исправлены оставшиеся английские/искажённые формулировки руководства и справочная категория аппарата. Ранее в этой сессии также были внесены крупные исправления названий аппаратов, терминов ртути/серы/нашатыря, чанов и гадательных жезлов. **Финальная проверка внутренних ссылок и разметки Theurgy не завершена/результат не зафиксирован**; обязательно вернуться к ней.
- Titanium: [de96d64](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/de96d64e1a9cb007dbf85b6c6adcc714c45f0ff6) — уточнены формулировки подсказок резервуара и названия тестового блока.

### Следующая точка продолжения

1. Сначала перечитать этот handoff, INVENTORY.md и GLOSSARY.md, а также проверить свежие main обоих репозиториев.
2. Продолжить именно текущую десятку, не повторять уже внесённые правки.
3. Завершить Theurgy: проверить все ссылки вида `item://`, `entry://`, `category://`, синтаксис форматирования книги, плейсхолдеры и смысл относительно EN; затем повторить полный JSON-аудит.
4. Провести полную смысловую и техническую вычитку остальных namespace этой десятки, включая supermartijn642corelib, terrablender и tiab; не объявлять десятку завершённой до закрытия всех десяти.
5. Только после полного аудита обновить сводные результаты и перейти к следующей партии.

Dropbox не изменялся. Все изменения локализации, перечисленные выше, находятся в GitHub main. На момент этой записи новая партия не объявляется завершённой.


## Завершение полной вычитки партии stepcrafter—titanium — 06.11.2026

**Партия завершена: 10/10 namespace, 5 205 ключей.** Эта запись заменяет предыдущую контрольную точку, где партия ещё считалась незавершённой. Все изменения опубликованы напрямую в main; Dropbox не изменялся.

| Namespace | EN/RU ключей | Missing | Extra | Дубликаты | Плейсхолдеры/порядок | Форматирование | Переносы строк | Краевые пробелы |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| stepcrafter | 79/79 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| storagedelight | 178/178 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| structurize | 236/236 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| supermartijn642corelib | 1/1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| sushigocrafting | 108/108 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| terrablender | 2/2 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| the_bumblezone | 1 800/1 800 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| theurgy | 2 744/2 744 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| tiab | 4/4 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| titanium | 53/53 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **5 205/5 205** | **0** | **0** | **0** | **0** | **0** | **0** | **0** |

Во всех десяти JSON проверены корректность разбора, точное совпадение наборов ключей, отсутствие дубликатов, пустые значения относительно EN, плейсхолдеры и их порядок, коды форматирования, число переносов строк и начальные/конечные пробелы. Для Theurgy и The Bumblezone дополнительно сверены внутренние ссылки item://, entry:// и category://. Все проверки завершились без расхождений.

### Смысловая вычитка

- **StepCrafter:** уточнено название улучшения слотов; сохранены технические обозначения формул и параметров.
- **Storage Delight:** проверены названия кухонных блоков, шкафов, ящиков и их вариантов; сохранены правильные состояния блоков и древесные породы.
- **Structurize:** уточнены формулировки инструмента сканирования, интерфейса схем, предварительного просмотра и конфигурации.
- **SuperMartijn642CoreLib:** единственная строка проверена по оригиналу; правка не потребовалась.
- **Sushi Go Crafting:** выровнена терминология еды и эффектов; Small Bites передано как шанс сохранить съедаемое блюдо, Itamae — «итамаэ».
- **TerraBlender:** обе строки команд проверены; правки не потребовались.
- **The Bumblezone:** вычитаны описания Шмеллиафана, корневиков, часовых, медовых слизней, блоков сот с расплодом, медовых кристаллов, сахарной воды, маточного молочка, эссенций, брони и аксессуаров. Исправлены конфигурации появления пчёл и спавнеров, совместимость с другими модами, названия эффектов и структур, тексты достижений и торговые теги. Унифицированы термины «Жужжилище», «Шмеллиафан», «Корневик», «блок сот с расплодом», «Опчеление».
- **Theurgy:** выправлены описания аппаратов и книжное руководство; исправлены логика реформации, трансмутации и возвышения, категории нитера, рецепты и инструкции, гадательные жезлы, ртутная логистика, загрузчики/извлекатели. Пересмотрены названия исходных материалов: бревна, древесина, породы, пищевые культуры, минералы и блоки. Исправлены ошибки вроде Common Metals → «обычные металлы», Mossy Cobblestone/Infested Cobblestone, Netherrack, End Stone, Glow Ink Sac, Lettuce, Date, Kale и другие. Ссылки книги и разметка сверены с EN.
- **TIAB:** все четыре строки сверены; правки не потребовались.
- **Titanium:** уточнены подсказки взаимодействия с резервуаром и название тестового блока.
- **GLOSSARY.md:** добавлены единые термины для загрузчиков/извлекателей Theurgy, уровней нитера и ключевых существ, эффектов, блоков и структур The Bumblezone.

### Коммиты main

- StepCrafter: [86e4505](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/86e45058364041c5f25a37eda43763b12012c9f1).
- Storage Delight: [c28ba9a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c28ba9a9885a00a1d3400b18eba729028e791180), [0e2e828](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0e2e82834f2008b1a6aef607b2eb2c9c4c372f2c), [bab298b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bab298bcad2f152e85c0c2735f46350bd669901b).
- Structurize: [5dc80a4](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5dc80a4a6a121caf57c327c571a8b3789c27a301), [68938b0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/68938b01f4c39ac3a65b332b65c53f8b57d8ed1e).
- Sushi Go Crafting: [67b02c5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/67b02c5f49433aaef1c13818d92cc89871a4388f), [644957f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/644957fc68cfdad5fba3e283209d296f35892683).
- The Bumblezone: [caa9e7c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/caa9e7cc78cbb8cba0d0b39b991566dd7584cb82), [44b4667](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/44b46671d370cd53d7614f910053167eaab50486), [730c8cd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/730c8cdc213165d7bfbf0047c94d97f81266308e), [ad77e4d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ad77e4dd8b3d191fb857f7e668f687abeff5975f), [df91f16](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/df91f16e5bb3db448d5f9d9173665867e8bf2fcf), [29cd1ea](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/29cd1eab5ec3cb32f7171389d3deeca37fd379f8), [3d604e9](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3d604e970a71b42b45b8ebff1e803ae75c4f1568), [e7f07d3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e7f07d3b30ec8c94f84b5db89aff559aad308efc), [458aa82](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/458aa823b32bc38b7f1237e7dc8b50697ecfc126), [a2cc19c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a2cc19c56a813326da5e020284e26c2b22b6fe8c), [26ecbf9](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/26ecbf99ba58252f942396773cfdae11d9908ced), [8d4ded0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8d4ded098211275befd0e23f881724724e21d3cc), [bb5c371](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bb5c3710e92779b7396415c747b5481e82eceddc), [7f7ba8d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7f7ba8dd7e924346f8b4062cbfb8139b3a2f37b4), [6cc0714](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6cc071476a25f6b7cf4af71beb21cd1da4096203).
- Theurgy: [a53c8ee](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a53c8ee5a31fab9936f9577c97754eb7c5192723), [413e847](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/413e847842445bb9b5f5739625c10c658dee620a), [73e79c0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/73e79c0344d98e4bc59d7b74e31a828f13b7ca89), [29dc8bb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/29dc8bb9080cf4e9803966d3c225fabad0bd8acd), [ceb4b99](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ceb4b99475545d7ea498491166d3a441c64a94ea), [ca8121e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ca8121e50107b74a740d097260d7c61abb408d08), [bec8f13](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bec8f13b988d87c360f5dce69753f939f0e0912f), [5ee6999](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5ee699913fea0b3c6db519fab3e767e0ed280c08), [e8b5521](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e8b5521d1c96987c4f33d24a50686eab50d2e274), [478d354](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/478d3540311c9b622a07061d447728385aafccbb), [3cec024](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3cec024203acd0e8e3132d23219702c8bf3ab3bd), [51d0218](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/51d0218e703ac0b1c46ccd80fc8b7d8f8aeaa070), [dc790c0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/dc790c0eec072d000f2c15646fed99aead4cdd13), [e020d5b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e020d5b2831d25db1ba11329673e7843bc060de1), [113984b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/113984b42ecc2935e5ad6f313b156ee51c7498b1), [f76ddd8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f76ddd826c4ec74cc96b511109c4b46fe9e5d457), [399601d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/399601dfb5d8597fff978a3285b608164c3335e6), [6787784](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6787784ed2a59ff6628bc316f2e132e2539a2e27), [7cb82d3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7cb82d39b06852b662c66f127421eb23c997b731), [31b4af6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/31b4af6039aed55520db9d7accb858caae26165d).
- Titanium: [de96d64](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/de96d64e1a9cb007dbf85b6c6adcc714c45f0ff6).
- GLOSSARY: [f2d3579](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f2d35794e753de50d7b8dd93ca782364291e084c).

У supermartijn642corelib, terrablender и tiab после сверки с EN правки не потребовались; их JSON включены в общий технический аудит.

### Следующая точка продолжения

Следующая десятка по порядку английских источников после titanium (Twilight Forest уже завершён и пропускается): toastcontrol, tombstone, toolbelt, torchmaster, transfer_labels, trashcans, trashslot, treetap, trophymanager, universalgrid.

У всех десяти RU-файлы уже существуют, а первичная сверка показывает совпадение наборов ключей с EN. Их не нужно создавать заново: следующая задача — повторная смысловая вычитка и полный технический аудит этих существующих файлов. После universalgrid следующими по дереву источников идут utilitarian и utilityvest.

Перед новой партией перечитать актуальные PROJECT_HANDOFF.md, INVENTORY.md, GLOSSARY.md, проверить свежие main обоих репозиториев и не повторять завершённые namespace. FTB Quests/SNBT оставить на самый конец проекта.

## Дополнение к завершённым проверкам и новая партия — 06.11.2026

### Дополнительные исправления после аудита stepcrafter—titanium

После завершения партии внесены ещё несколько подтверждённых смысловых исправлений:
- **Theurgy:** уточнены описания аппаратов и EMI-подсказки, приведены к глоссарию категории нашатыря и ртути, исправлено согласование «алхимическая сера».
- **The Bumblezone:** выправлены описания медовых предметов и компаса, тексты достижений и команд, названия настроек; восстановлено исходное форматирование § и количество переносов строк.
- **StepCrafter:** улучшено описание рекурсивного автокрафта и формулировка энергопотребления улучшения слота.
- **Structurize:** уточнены подсказки сканирования, якорных блоков, заполнителей, телепортации и выполнения операций.

Коммиты: Theurgy [d95c3c0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d95c3c0e73fe3208f3a89f756604f459eaaa5281), [bafb1a8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bafb1a8d21bf3c2fc1450a5f7a2f6e11a9b2c74a), [ea92c80](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ea92c80a0c01fc943d87a1d9f9460fe10fc8f283); The Bumblezone [7a85940](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7a859402462c1ba26ab6976665e59850eee989eb), [948d455](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/948d4559d7af88508b127052396fe97e676187b9), [de5d287](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/de5d28780065a80418e1ae6b20fc36a2d7554e20), [07e66fa](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/07e66fac25ced476688091e4ad594fcbc7af06c9), [6df0f62](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6df0f62322120af5bff5fc0825bd699ba39a62d4); StepCrafter [d438d7c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d438d7c6c080c6050cadaf70514b4b905446b93b); Structurize [26571f2](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/26571f27eb3863630062aeb080c12a44c2958b11).

Повторный технический аудит всех 5 205 ключей этой партии завершился без расхождений: ключи, плейсхолдеры и их порядок, форматирование, переносы строк, краевые пробелы и пустые значения соответствуют EN.

### Завершена партия toastcontrol—universalgrid

**Завершено 10/10 namespace, 1 413 ключей.** Все десять файлов сверены с актуальными оригиналами в `ATM/LANGUAGES_EN_US`.

| Namespace | EN/RU ключей | Missing | Extra | Дубликаты | Плейсхолдеры | Форматирование | Переносы | Краевые пробелы |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| toastcontrol | 2/2 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| tombstone | 1 240/1 240 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| toolbelt | 13/13 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| torchmaster | 42/42 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| transfer_labels | 21/21 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| trashcans | 34/34 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| trashslot | 24/24 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| treetap | 8/8 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| trophymanager | 13/13 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| universalgrid | 16/16 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **1 413/1 413** | **0** | **0** | **0** | **0** | **0** | **0** | **0** |

Все JSON корректны. Совпадение наборов ключей полное; дубликатов, пропусков, лишних ключей, несовпадений плейсхолдеров, форматирования, переносов строк, краевых пробелов и пустых значений нет.

Смысловые исправления:
- **Tombstone:** исправлены ошибочные и неполные статьи компендиума (мировоззрение, молитвы, Знание смерти, костяная игла, души и сосуды, зачарования, скрижали и магические книги); уточнены инструкции предметов, тексты достижений, названия памятной таблички и подсказки. Терминология сведена к единому виду.
- **Tool Belt:** проверены названия пояса, подсумка, слотов и действий с инструментами.
- **Torchmaster:** Feral Flare Lantern унифицирован как «светильник дикого пламени» во всех названиях и настройках.
- **TreeTap:** Tap уточнён как «кран для подсочки», Sap Collector — «сборщик древесного сока».
- **ToastControl, Transfer Labels, Trash Cans, TrashSlot, Trophy Manager и Universal Grid:** строки проверены по контексту; подтверждённых дополнительных смысловых ошибок не осталось.

Совпадения с английским оставлены только там, где это оправдано: название Torchmaster в группе предметов, модификаторы клавиш SHIFT/CTRL в Trash Cans, название категории TrashSlot и имя мода Universal Grid.

Коммиты текущей партии:
- Tombstone: [b025a7b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b025a7b23855a09375b8ad1c48d6e078b3625e09), [a62d1fd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a62d1fdf144e726142f3c1b5cd43112670a139d8), [b238777](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b238777726d354cac6ab60b241992fa04ff8a9a8), [d59f80d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d59f80d8559aa9f0e051f386262b32e1b587b50e), [8080261](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8080261e0490851214f01155349db2d75a39a67d), [78f1828](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/78f182866aa91d21b2ce93d75099a27d08123b93), [1dfc691](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1dfc6914a073c47c6cce4bd0c531a0539691987f), [1c3127d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1c3127ded512f5eaa283743e80de3ec3f1959180), [4964293](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/49642933fb84c264aa0ffe2ce89be20e1877694f), [09dfcb9](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/09dfcb94eb6c35cfab8d82388b63c0f969c20ad7), [b851b49](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b851b497f4614086f0974c6033a61d155b2168a8).
- Tool Belt: [34b8469](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/34b8469774997346b58c0855fcd97588a6860057).
- Torchmaster: [cb9e5e9](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cb9e5e994066dfbd7405047077679269cdeb468c).
- TreeTap: [ebc1dbc](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ebc1dbc28cc6cea238cf470d7a6614972e98038e), [9dc74e5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9dc74e56265440e55039612a2c245c75647bf6d3).
- Universal Grid: [36b7447](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/36b744783b82c803c69a99f2d23bb4696a75064f).
- GLOSSARY: [c93d634](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c93d6342041ca53fb1686120be96e83cf7c99c36), [8fa512b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8fa512b8354997594cb0ea7a9245f16b1a0d2ca6).

Dropbox не изменялся.

### Следующая партия

Следующие десять namespace по порядку английских источников:
`utilitarian`, `utilityvest`, `variantsandventures`, `waystones`, `wirelesschargers`, `xnet`, `xtonesreworked`, `xycraft_core`, `xycraft_machines`, `xycraft_override`.

После них остаются `xycraft_world` и `yet_another_config_lib_v3`. Перед началом следующей партии проверить актуальные файлы и версии в обоих репозиториях; уже сделанные правки не повторять.

## Завершена партия utilitarian—xycraft_override — 06.11.2026

**10/10 namespace, 1 858 ключей.** Все RU-файлы сверены с актуальными EN-оригиналами.

| Namespace | EN/RU |
|---|---:|
| utilitarian | 111/111 |
| utilityvest | 36/36 |
| variantsandventures | 128/128 |
| waystones | 361/361 |
| wirelesschargers | 23/23 |
| xnet | 186/186 |
| xtonesreworked | 547/547 |
| xycraft_core | 106/106 |
| xycraft_machines | 225/225 |
| xycraft_override | 135/135 |
| **Итого** | **1 858/1 858** |

**Техническая проверка:** JSON корректен; missing 0, extra 0, duplicates 0, empty mismatch 0, placeholder/type/position mismatch 0, formatting mismatch 0, newline mismatch 0, edge whitespace mismatch 0, link mismatch 0. В трёх командах Waystones использованы позиционные плейсхолдеры, чтобы аргументы оставались на своих местах при перестановке слов.

**Смысловые правки:** Utilitarian — выровнены обращения, уточнены подсказки и настройки подавления стартовых сообщений; Utility Vest — исправлены сообщение об отклонённой записи и подсказка фильтра; Variants&Ventures — унифицированы имена мобов и исправлены формы в настройках появления; Waystones — переведены цвета Sharestone, уточнены настройки видимости и команды; XNet — исправлены подписи антенн, названия коннекторов и единицы мБ; XyCraft — уточнены описания машин, модулей, многоблочных конструкций и тегов. Wireless Chargers и Xtones Reworked проверены, дополнительных смысловых ошибок не обнаружено.

Оставлены намеренные совпадения с EN: имена Variants&Ventures, XNet, XyCraft, BlueMap, NBT, Xynergy, группа Xtones Reworked и 34 оригинальных имени палитр Xtones. GLOSSARY дополнен терминами Waystones, Variants&Ventures и XyCraft. Dropbox не изменялся.

Коммиты: Utilitarian [9eead33](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9eead33e3a53a09a12d37b4708e357049e7ba34f); Utility Vest [1b4a073](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1b4a073a697d724795cc6fd64a0f4019d8a80342); Variants&Ventures [0f60058](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0f600583f651a7adcb939de3c6f73891f758ed7c), [ac949d9](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ac949d9296afd46a8bb7bded52eac9719f8d5e75), [c54e89a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c54e89acb382939932f9ba0e74f5a69c8884ac02); Waystones [b9a7112](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b9a711207dfff52d7a153ade482f9384334b4851), [1a5736a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1a5736aa0749abe3ad693be13df02eb7d425df46), [68269d8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/68269d8aecb5ba1a034451a64b8d27e19508bfa3); XNet [f042dfb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f042dfbc6ee5bbba2425a4c6e43f847f13613bbc); XyCraft Machines [5a51b89](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5a51b891c298a7bc6461f51c9c8ff8438589744b), [85c7d44](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/85c7d4412c8a86079c4fc01d4492dfa5b59a810b), [bd240e9](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bd240e9f93d29f767410e768443446c10a9e9567), [f787b27](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f787b27bed06b6a92979b453ff51407a702c0ff9); XyCraft Core [d883efa](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d883efa96bd6881f38b66475ce8feb9fb352a713); XyCraft Override [0c75348](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0c753487610cb0b745d10c1440523e95c4da98eb); GLOSSARY [32682ad](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/32682adc0aebbd689dca8e64decdf61ccf7ee701), [8f126f6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8f126f623a9ba3a3142381a6d43e68884348a43c).

### Следующий шаг

В английском каталоге после `xycraft_override` остаются два обычных namespace: `xycraft_world` и `yet_another_config_lib_v3`. После них — финальные специальные задачи FTB Quests и SNBT. FTB Quests уже имеет перевод 67/67 глав, но оставлен для итоговой проверки в конце проекта.

## Финальный хвост обычных локализаций — 06.11.2026

После партии utilitarian—xycraft_override закрыты последние два обычных namespace: **xycraft_world** и **yet_another_config_lib_v3**. Это финальный остаток, не отдельная десятка: **2/2 namespace, 350 ключей**.

| Namespace | EN/RU |
|---|---:|
| xycraft_world | 324/324 |
| yet_another_config_lib_v3 | 26/26 |
| **Итого** | **350/350** |

Техническая проверка: JSON корректен; missing 0, extra 0, duplicates 0, placeholder/type/position mismatch 0, formatting mismatch 0, newline mismatch 0, edge whitespace mismatch 0, empty mismatch 0.

Смысловые исправления XyCraft World: исправлены формы цветов и согласование в названиях ламп, блоков Оури, алюминиевых и ксикориевых блоков; «Light» приведено к значению «светлый», Glass Viewer — к «смотровому стеклу», уточнены названия породы Киви и хранилищ самоцветов. В YACL улучшены подсказки сохранения и отмены изменений.

Коммиты: XyCraft World [be4094c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/be4094c9e306d6d05b7424040a6291aa26a79552), [5d25540](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5d25540abf3a22eb1de65f75fb9f650b31f2107c); YACL [662e0e6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/662e0e60b5d2f8e30814b12c22e87bf182b91334); GLOSSARY [a77536a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a77536a8fa396be38f69e4af0ce40228aebec345).

## Финальная проверка FTB Quests / SNBT

По текущему дереву EN/RU совпадают имена **67/67 глав FTB Quests**. Английский репозиторий не менялся после коммита `1f1bb082612226447ad674ae6045fc4b28001b09` от 02.11.2026. Последний зафиксированный полный аудит FTB Quests/SNBT: 67 глав, общие языковые файлы и **20 SNBT-файлов**; структура SNBT сбалансирована, пропусков ключей и ошибок плейсхолдеров не обнаружено. В этой сессии FTB Quests/SNBT не изменялись.

Обычные namespace английского дерева закрыты. Полноценный запуск сборки и внутриигровая проверка локализации по-прежнему не выполнялись. Dropbox не изменялся.

## Контроль документации после завершения локализаций — 06.11.2026

После финальной проверки обновлён `README.md`: отражены завершение обычных namespace, аудит FTB Quests/SNBT и отсутствие внутриигрового тестирования. Коммит README: [47d01f6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/47d01f609365e42c262616b1552a0310d3312ec2). В `INVENTORY.md` исправлена устаревшая формулировка о том, что FTB Quests ещё нужно оставить на конец: специальный этап уже завершён. Коммит: [0ab0b2e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0ab0b2e6444a7de829b5d1f62f3dcb52e2501c32).

**Следующая точка продолжения:** подготовка и проведение внутриигрового тестирования на ATM10 8.5 / Minecraft 1.21.1 / NeoForge. Проверить загрузку ресурс-пака, применение `ru_ru.json`, отображение кириллицы, длинные строки и подсказки GUI, команды Waystones, страницы компендиума Tombstone, интерфейсы YACL и FTB Quests. Не объявлять внутриигровую проверку выполненной до фактического запуска сборки. После теста фиксировать только воспроизводимые проблемы и исправлять их в `main`.

## Дополнительная правка по скриншоту — 06.11.2026

При визуальной проверке публичной папки Google Drive `BEAMNG EARTH` обнаружен английский текст описания квеста Block Filter в главе Pylons. Сверка с EN-оригиналом подтвердила ключ `quest.77B185799366ACD2.quest_desc`: в `ATM/FTBQUESTS/ru_ru/chapters/pylons.snbt` он отсутствовал, хотя английское описание присутствует в `ATM/FTBQUESTS/en_us/chapters/pylons.snbt`. Добавлен русский перевод с сохранением структуры SNBT и переносов строк.

Коммит исправления: [f52411d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f52411dfe77780d7e1678a94e160f55eac256fd2).

В папке Google Drive обнаружено 9 PNG. Визуально удалось проверить только `Dh2EiniP1F.png`; остальные 8 изображений пока не просмотрены из-за сбоев предпросмотра Google Drive. Поэтому этот осмотр не считается полным аудитом скриншотов.


## Локализация названий глав FTB Quests — 06.11.2026

По просьбе пользователя локализованы названия **74 глав** в `FTBQUESTS/ru_ru/chapter.snbt` и все **13 названий групп** в `FTBQUESTS/ru_ru/chapter_group.snbt`. Переведены также четыре подзаголовка глав. Англоязычные названия модов сохранены там, где это помогает узнать мод, но дополнены понятным русским описанием; названия глав основной цепочки и форматирующие коды Minecraft сохранены.

Сверка с актуальными EN-файлами: chapter title IDs 74/74, missing 0, extra 0, duplicates 0; chapter group IDs 13/13, missing 0, extra 0. Проверка структуры SNBT: фигурные скобки и кавычки сбалансированы. Это проверка файлов, а не отдельное подтверждение отображения обновлённых заголовков в игре.

Коммиты:
- Названия глав и подзаголовки: [e02ccea](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e02ccea1f29c396cff0b835c15d4fba87570ac6d).
- Названия групп глав: [c22a98e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c22a98ec12dd239b58f3ba97610987ff93f70964).

Для установки обновления скопировать из репозитория файлы `chapter.snbt` и `chapter_group.snbt` в `config/ftbquests/quests/lang/ru_ru/`, заменив старые версии этих двух файлов. Остальные языковые файлы не трогать.


## Подготовка пользовательской страницы и дистрибутивов — 07.11.2026

Обновлён корневой `README.md`: он теперь ориентирован на обычных игроков и объясняет разделение установки на два комплекта — Minecraft Resource Pack и локализацию FTB Quests. Добавлены инструкции для папки `resourcepacks` и для `config/ftbquests/quests/lang/ru_ru/`, включая правильное расположение `chapter.snbt` и `chapter_group.snbt`. Также добавлены подсказки по открытию папки экземпляра в Prism Launcher и CurseForge, предупреждение о резервном копировании и ссылки на раздел Releases.

Коммит README: [b65e584](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b65e58428a3cf8f8cfbeda76cf7d7d3185eed10b).

**Что ещё не выполнено:** пользовательские ZIP-архивы Resource Pack и FTB Quests не собраны и не опубликованы; GitHub Releases пока пуст. Поэтому README прямо сообщает, что загрузки появятся после подготовки архивов, и не выдаёт исходный ZIP репозитория за готовый комплект установки. Отдельно требуется закончить аудит/перевод изображений FTB Quests и проверить фактическую структуру обоих архивов перед первым релизом.

Текущая структура исходников проверена: корневые `assets/` вместе с `pack.mcmeta` образуют исходную структуру Minecraft Resource Pack; `FTBQUESTS/ru_ru/` содержит общие SNBT-файлы и папку `chapters/`. Рабочие исходники пока не перемещались и не удалялись. Английский репозиторий и Dropbox не изменялись.
