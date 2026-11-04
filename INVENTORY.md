# Инвентаризация локализаций ATM10

Дата сверки: **05.11.2026**  
Версия официальной сборки: **ATM10 8.5**  
Источник списка модов: [AllTheMods/ATM-10](https://github.com/AllTheMods/ATM-10), `config/crash_assistant/modlist.json`, ветка `main`.  
Русские файлы: текущая ветка `main` репозитория `d1gorae/ATM10-RU-TRANSLATE`, пути `assets/<namespace>/lang/ru_ru.json`.

## Сводка

| Показатель | Значение |
|---|---:|
| Записей в официальном modlist | 497 |
| Уникальных mod ID (без NeoForge) | 490 |
| Русских JSON-файлов | 383 |
| Mod ID с одноимённым русским namespace | 370 |
| Mod ID без одноимённого русского JSON | 120 |
| Из них вне FTB Quests | 119 |
| Дополнительных namespace без прямого совпадения | 13 |

Отсутствие одноимённого JSON не доказывает, что мод содержит переводимые строки. Для каждого кандидата нужно сверить фактический `en_us.json` в версии мода из ATM10 8.5. FTB Quests не трогать до самого конца проекта.

## Mod ID без одноимённого ru_ru.json

- `accelerateddecay`
- `ae2jeiintegration`
- `aiimprovements`
- `alltheleaks`
- `architectury`
- `athena`
- `atlas_api`
- `atmcompat`
- `attributefix`
- `bibliobiomes`
- `bibliocraft`
- `bibliowoods`
- `blueflame`
- `borderlesswindow`
- `botanypotsmystical`
- `botanytrees`
- `byzantine`
- `catjammies`
- `chipped`
- `chisel`
- `cleanswing`
- `cloth_config`
- `clumps`
- `cobweb`
- `colorwheel`
- `colorwheel_patcher`
- `connectivity`
- `corgilib`
- `crash_assistant`
- `cryonicconfig`
- `cupboard`
- `deimos`
- `dungeoncrawl`
- `dyenamicsandfriends`
- `edivadlib`
- `experiencelib`
- `explorify`
- `fastfurnace`
- `fastsuite`
- `ferritecore`
- `flickerfix`
- `formationsnether`
- `formationsoverworld`
- `framework`
- `ftbjeiextras`
- `ftbquests`
- `ftbranks`
- `ftbxmodcompat`
- `fuelgoeshere`
- `geckolib`
- `glodium`
- `hellish_trials`
- `herbsandharvest`
- `heyberryshutup`
- `iceberg`
- `illagerwarship`
- `immediatelyfast`
- `incontrol`
- `integratedscripting`
- `iris`
- `iris_search`
- `jumpboat`
- `konkrete`
- `kubejs`
- `lithostitched`
- `lmft`
- `logisticsnetworks`
- `melody`
- `modelfix`
- `monolib`
- `moredragoneggs`
- `moreredxcctcompat`
- `mousetweaks`
- `mysticalcustomization`
- `netherportalfix`
- `novillagerdm`
- `nullscape`
- `observerlib`
- `occultism_kubejs`
- `octolib`
- `ohthetreesyoullgrow`
- `omegaconfig`
- `openloader`
- `overlapless`
- `overloadedarmorbar`
- `pamhc2foodextended`
- `playeranimator`
- `polyeng`
- `ponderjs`
- `prickle`
- `prism`
- `rebind_narrator`
- `rechiseled`
- `rechiseled_chipped`
- `refurbished_furniture`
- `resourcefullib`
- `rhino`
- `smartbrainlib`
- `sodium`
- `sodium_extra`
- `sophisticatedbackpackscreateintegration`
- `sophisticatedstoragecreateintegration`
- `spark`
- `stevescarts`
- `structory`
- `structory_towers`
- `stylecolonies`
- `supermartijn642configlib`
- `sussysniffers`
- `t_and_t`
- `theurgy_kubejs`
- `towntalk`
- `underground_villages`
- `uranus`
- `valhelsia_core`
- `villagesandpillages`
- `wits`
- `xtonesreworked`
- `yeetusexperimentus`
- `yungsextras`

## Дополнительные namespace без прямого совпадения с mod ID

- `borderless`
- `cloth-config2`
- `dynamic_fps`
- `entityculling`
- `evilcraftcompat`
- `integrateddynamicscompat`
- `integratedterminalscompat`
- `irons_patreon_lib`
- `lambdynlights`
- `lollipop`
- `moreculling`
- `tempad_static`
- `vulkanmod`

Не удалять автоматически. Это могут быть алиасы, библиотеки, вспомогательные моды или namespace, предоставляемые другой зависимостью.

## Сверка Dropbox

Источник: папка `languages_ru_ru`, предоставленная пользователем.

- Всего обнаружено **773 элемента**: 512 папок и 261 файл.
- Среди файлов: **256 JSON** и **5 legacy-файлов `.lang`**.
- JSON-файлы охватывают **254 namespace**. Два namespace имеют по два файла разных версий: `allthemodium` и `computercraft`.
- До импорта в GitHub уже присутствовали 229 из 254 namespace; 25 отсутствовали.
- В репозиторий импортированы **20 существовавших Dropbox-переводов**. При импорте сохранялись только ключи, присутствующие в английском файле именно соответствующей версии, с непустыми значениями и совпадающими форматирующими плейсхолдерами.
- Всего импортировано **19 844 существующих значения**. Это не означает, что все файлы полностью переведены: отсутствующие ключи намеренно оставлены для последующего перевода, а одинаковые английскому значения требуют смысловой проверки.
- Для `allthemodium` объединены два Dropbox-файла с общим namespace: добавлены 307 ключей основного мода к существующему файлу; при одном конфликте сохранено значение из GitHub.
- Для `computercraft` Dropbox содержит две версии. Файл GitHub уже полнее (235 ключей против 181/188 в Dropbox), поэтому замены не делались.
- Ещё пять namespace из Dropbox не импортированы:
  - `ftbquests` — отложен до самого конца проекта;
  - `iris`, `iris_search`, `sodium_extra` — в английском репозитории не найден соответствующий языковой оригинал для безопасной сверки;
  - `integratedscripting` — Dropbox-файл содержит пустой объект `{}`.
- Пять файлов `.lang` сохранены в Dropbox как справочные материалы. Они не преобразовывались автоматически в JSON: у части старый формат ключей, а у части ключи не совпадают с текущими английскими ресурсами.

## Импортированные из Dropbox файлы

В рамках первого прохода до этой сверки уже были добавлены `advancedperipherals`, `mekmm` и `relics` (1 391 значение). В текущем проходе добавлены ещё 20 файлов (19 844 значения). Итого из Dropbox перенесены **23 файла и 21 235 существующих значений**. Это импорт уже имевшегося текста, а не завершённый перевод.

| Namespace | Импортировано ключей | Ключей в английском оригинале |
|---|---:|---:|
| `advancedperipherals` | 140 | 140 |
| `mekmm` | 704 | 704 |
| `relics` | 547 | 547 |
| `evilcraft` | 376 | 629 |
| `ars_nouveau` | 1 296 | 2 323 |
| `mekanism` | 1 605 | 3 239 |
| `iceandfire` | 1 193 | 1 809 |
| `sophisticatedstorage` | 256 | 425 |
| `irons_spellbooks` | 1 128 | 1 315 |
| `silentgear` | 616 | 1 191 |
| `mekanismgenerators` | 200 | 364 |
| `neovitae` | 256 | 3 652 |
| `productivetrees` | 3 832 | 4 149 |
| `pneumaticcraft` | 1 987 | 2 274 |
| `mekanismtools` | 185 | 800 |
| `twilightforest` | 1 475 | 2 061 |
| `industrialforegoing` | 584 | 683 |
| `aether` | 1 071 | 1 238 |
| `integrateddynamics` | 1 629 | 1 854 |
| `supplementaries` | 708 | 1 394 |
| `reliquary` | 307 | 551 |
| `ad_astra` | 685 | 831 |
| `regions_unexplored` | 455 | 933 |

Для импортированных файлов ключи, которых нет в английском оригинале, пустые значения и записи с несовпадающими форматирующими плейсхолдерами не переносились. Недостающие ключи не заполнялись автоматически: их перевод — отдельная будущая работа.

## Принцип использования Dropbox

Dropbox — вспомогательный источник ранее сделанных переводов, а не источник для безусловной замены GitHub. Многие файлы Dropbox старее или неполнее текущих GitHub-файлов. Совпадение количества ключей не гарантирует лучшего перевода; отличающиеся значения нельзя перезаписывать без смысловой проверки.

При переносе новых источников:
1. Проверять соответствие версии мода и namespace.
2. Сверять ключи с английским оригиналом ATM10 8.5.
3. Удалять устаревшие ключи, отсутствующие в текущем английском файле.
4. Не переносить пустые значения и записи с несовпадающими плейсхолдерами.
5. Сохранять более полные и качественные значения, уже находящиеся в GitHub.
6. Не менять Dropbox: он остаётся исходным архивом.

## Отдельно отложено

- `ftbquests` — не включать в текущую работу; перевод FTB Quests/SNBT остаётся на самый последний этап по прямому указанию пользователя.

## Ограничения точности

Эта инвентаризация считает файлы и namespace, но не объявляет все 120 отсутствующих namespace обязательными к переводу. Перед созданием нового файла нужно проверить, содержит ли мод собственные пользовательские строки, нет ли общего namespace и не являются ли оставшиеся записи служебными.
