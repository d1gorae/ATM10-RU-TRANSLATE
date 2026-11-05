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
