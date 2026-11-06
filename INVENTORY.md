# Инвентаризация локализаций ATM10

Дата сверки: **06.11.2026**  
Версия официальной сборки: **ATM10 8.5**  
Источник списка модов: [AllTheMods/ATM-10](https://github.com/AllTheMods/ATM-10), `config/crash_assistant/modlist.json`, ветка `main`.  
Базовый снимок русских файлов: актуальная ветка `main` репозитория `d1gorae/ATM10-RU-TRANSLATE`, пути `assets/<namespace>/lang/ru_ru.json`. Рабочие переводы из `work/irons-spells-nov05` перенесены в `main` 06.11.2026; актуальная точка продолжения — `main`.


## Сведение рабочих веток — 06.11.2026

Основная рабочая ветка объединена в `main` через PR #5. Файл `assets/bibliocraft/lang/ru_ru.json` заполнен из рабочей ветки `work/bibliocraft-ru` (2 021 ключ); покрытие BiblioCraft base 2021/2021 уже отражено в инвентаризации. Остальные проверенные старые ветки содержат дублирующие версии уже имеющихся файлов; альтернативные значения из `work/atm10-batch-nov05` требуют выборочной смысловой сверки и не были автоматически перенесены.

## Сводка

| Показатель | Значение |
|---|---:|
| Записей в официальном modlist | 497 |
| Уникальных mod ID (без NeoForge) | 490 |
| Русских JSON-файлов | 399 |
| Mod ID с одноимённым русским namespace | 385 |
| Mod ID без одноимённого русского JSON | 105 |
| Из них вне FTB Quests | 105 |
| Дополнительных namespace без прямого совпадения | 14 |

Отсутствие одноимённого JSON не доказывает, что мод содержит переводимые строки. Для каждого кандидата нужно сверить фактический `en_us.json` в версии мода из ATM10 8.5. FTB Quests не трогать до самого конца проекта.

## Mod ID без одноимённого ru_ru.json

- `accelerateddecay` — EN-файл проверен, 0 ключей; отдельный RU-файл не нужен.
- `ae2jeiintegration`
- `aiimprovements`
- `alltheleaks`
- `architectury`
- `athena`
- `atlas_api`
- `atmcompat` — все 10 ключей уже есть в `assets/allthemodium/lang/ru_ru.json`.
- `attributefix`
- `bibliobiomes` — переведён, 9577/9577 ключей покрыты общим `assets/bibliocraft/lang/ru_ru.json`; отдельный namespace не создавать.
- `bibliowoods` — переведён, 10833/10833 ключей покрыты общим `assets/bibliocraft/lang/ru_ru.json`; добавлены 157 отсутствовавших переводов Mauve. Отдельный namespace не создавать.
- `blueflame`
- `borderlesswindow`
- `botanypotsmystical`
- `botanytrees`
- `byzantine`
- `catjammies`
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
- `ftbjeiextras` — EN-файл проверен, 0 ключей; отдельный RU-файл не нужен.
- `ftbquests` — FTB Quests локализован через SNBT: 67/67 глав, `chapter.snbt` 78/78, `reward_table.snbt` 51/51, `chapter_group.snbt` 13/13; глобальные языковые файлы пустые.
- `ftbranks`
- `ftbxmodcompat` — EN-файл проверен, 0 ключей; отдельный RU-файл не нужен.
- `fuelgoeshere`
- `geckolib`
- `glodium`
- `hellish_trials`
- `heyberryshutup`
- `iceberg`
- `illagerwarship` — EN-файл проверен, 0 ключей; отдельный RU-файл не нужен.
- `immediatelyfast`
- `incontrol`
- `jumpboat`
- `konkrete`
- `kubejs`
- `lithostitched`
- `lmft`
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
- `playeranimator`
- `polyeng`
- `ponderjs`
- `prickle`
- `prism`
- `rebind_narrator`
- `rechiseled_chipped` — EN-файл проверен, 0 ключей; отдельный RU-файл не нужен.
- `resourcefullib` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `rhino` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `smartbrainlib` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `sodium_extra` — переведён, 418/418 ключей в `assets/sodium-extra/lang/ru_ru.json`; в namespace используется дефис вместо подчёркивания, поэтому файл указан как дополнительный namespace.
- `sophisticatedbackpackscreateintegration` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `sophisticatedstoragecreateintegration` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `spark` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `structory` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `structory_towers` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `stylecolonies` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `supermartijn642configlib` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `sussysniffers` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `t_and_t` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `theurgy_kubejs` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `towntalk` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `underground_villages` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `uranus` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `valhelsia_core` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `villagesandpillages` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `wits` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `yeetusexperimentus` — в актуальном дереве английских источников отдельный `en_us.json` для namespace не найден; отдельный RU-файл пока не требуется.
- `yungsextras` — отдельный `en_us.json` с таким namespace не найден; в источнике YUNG's API и отдельные модули YUNG представлены самостоятельными namespace.

## Дополнительные namespace без прямого совпадения с mod ID

- `borderless` — проверен: 21/21 ключ, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0.
- `cloth-config2` — проверен: 49/49 ключей, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0; клавиши Alt/Ctrl/Shift оставлены без перевода.
- `dynamic_fps` — проверен: 85/85 ключей, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0.
- `entityculling` — проверен: 27/27 ключей, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0; название мода сохранено.
- `evilcraftcompat` — проверен: 29/29 ключей, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0; исправлено написание бренда Baubles.
- `integrateddynamicscompat` — проверен: 213/213 ключей, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0; исправлено `Is RS Сеть` → `Сеть RS`.
- `integratedterminalscompat` — проверен: 19/19 ключей, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0; восстановлен отсутствовавший служебный ключ `_comment`.
- `irons_patreon_lib` — проверен: 2/2 ключа, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0.
- `lambdynlights` — проверен: 63/63 ключа, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0.
- `lollipop` — проверен: 50/50 ключей, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0.
- `moreculling` — проверен: 55/55 ключей, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0.
- `sodium-extra` — проверен: 418/418 ключей, missing 0, extra 0, placeholders 0, пустых значений 0; namespace мода Sodium Extra использует дефис.
- `tempad_static` — проверен: 84/84 ключа, missing 0, extra 0, placeholders 0, formatting 0, дубликатов ключей верхнего уровня 0; вложенные JSON-массивы и компоненты проверены рекурсивно.
- `vulkanmod` — проверен: 89/89 ключей, missing 0, extra 0, placeholders 0, formatting 0, duplicates 0.

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
- Ещё пять namespace из Dropbox не импортированы (это не означает отсутствие локализации в GitHub):
  - `ftbquests` — Dropbox-копия не импортировалась; локализация выполнена напрямую по актуальным GitHub SNBT и завершена;
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
| `mekanism` | 3 239 | 3 239 |
| `iceandfire` | 1 809 | 1 809 |
| `sophisticatedstorage` | 256 | 425 |
| `irons_spellbooks` | 1 128 | 1 315 |
| `silentgear` | 616 | 1 191 |
| `mekanismgenerators` | 200 | 364 |
| `neovitae` | 3 652 | 3 652 |
| `productivetrees` | 4 149 | 4 149 |
| `pneumaticcraft` | 1 987 | 2 274 |
| `mekanismtools` | 800 | 800 |
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

- Нет. FTB Quests/SNBT — заключительный этап проекта — завершён на уровне файлов; внутриигровой тест не проводился.

## Ограничения точности

Эта инвентаризация считает файлы и namespace, но не объявляет все 120 отсутствующих namespace обязательными к переводу. Перед созданием нового файла нужно проверить, содержит ли мод собственные пользовательские строки, нет ли общего namespace и не являются ли оставшиеся записи служебными.


## Добавлено после инвентаризации

### Пять новых локализаций, опубликованных 05.11.2026

| Namespace | Ключей | EN SHA | RU SHA | Коммит |
|---|---:|---|---|---|
| logisticsnetworks | 729 | `5237f7fd5d6846951375993fa781c4b9b06dd2d4` | `5da3d204799c23d4feab9fa773b397c56a0ca2ab` | [781e6d4](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/781e6d45645533a15311dac05a6d615659f61642) |
| pamhc2foodextended | 872 | `aba87691a39599c72e488efd456c59c947a43694` | `a9686a0129c819f9d63e68cd671e82f9c9b5f9c9` | [b66ad57](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b66ad571e7381562e57683b247f6f83e36844a86) |
| bibliocraft | 2021 | `d07816ab738feebeca49447e6de17540cdb2c392` | `fcc810c00974131f9586b6ce46f03c383a83935c` | [9510851](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/95108517bd67bb6599fa935a54fccd8d118ba5ec) |
| chisel | 2774 | `7651fb2f601fe28b4799a902ce1a3fea81f6f0fc` | `c02df7d373234fddbcb0796a7f53c5bc5074bf52` | [e5a1408](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e5a14083c03e079a730a253aee9145100e2661f8) |
| dyenamicsandfriends | 2090 | `dc59a3530285256bd5cc8f2db1e350d8fdaae7a5` | `9848e3d3a0cc4b32f0351e7a51ec61897c33e072` | [ae1effb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ae1effb1a0d2d6deb690b3362b7c9c8154ee7d11) |

### Пять ранее опубликованных локализаций, прошедших повторную проверку

| Namespace | Ключей | EN SHA | RU SHA | Последние исправления |
|---|---:|---|---|---|
| herbsandharvest | 879 | `f45325eafcccea6ff336954362d9666f6b9c5f17` | `25e01bb5b88018d2407df8cbd55b73a8e9bb4506` | [5563f70](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5563f70aeaedae92ae6751f69dd98e74ea8fd218), [975b08d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/975b08d226ecd3e6ba7c7bac1dd58d6b59c34155) |
| refurbished_furniture | 654 | `94f97e020cbcdc6afc60fea7e873f994ea565628` | `777c238a1551705ed4f185aab0d0d33e8be98c27` | [322c0c7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/322c0c756e8dfe8ae6bbc7cb3ede3c11749ac3b4), [247d997](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/247d997db7f09f32b032d05a0fc34f9dee67a07b) |
| stevescarts | 709 | `37289cc36ea1ed3e42ed0bcb84479bd3fe4a70ce` | `db0c443e1c37bdc24699473780f8c7fb6d3d51c3` | [9cedcec](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9cedcec761bd8452f9f56e75ce9d6b30b98f1e1d) |
| integratedscripting | 210 | `7ea575fac87c3e8613653010bf57fa9e1b7af210` | `8a4b2f8d0fcb3ed257d50f99fd45fc6059513390` | [49d802f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/49d802fe2a9e36062efbe74c61c468fe30af4752) |
| xtonesreworked | 547 | `9bf94d41801d263b90e7f6eae7ca527ccb562da0` | `bd04b55fb7cf1b11105a81e90fc9a5da907b682c` | Проверен повторно, исправления не потребовались |

Итого по завершённой десятке: **11 485 ключей**. Во всех десяти файлах подтверждены корректный JSON, полное совпадение наборов ключей, отсутствие лишних/пропущенных ключей, дубликатов JSON-ключей и расхождений плейсхолдеров. Проверка форматирования § и переносов строк также не выявила расхождений.

### Выявленные особенности очереди

- bibliobiomes: локализация завершена и объединена с assets/bibliocraft/lang/ru_ru.json. EN: 9577 ключей; итоговый RU-файл содержит 11 598 ключей (2021 BiblioCraft + 9577 Bibliobiomes). Все прежние 2021 значения BiblioCraft сохранены без изменений. EN SHA: `5e0f1c9b49566cb0353cc4e24869cb9f12f31a76`; итоговый RU blob SHA: `d6ff8512a9cc4f67163131f79958afc607a52148`; commit: [3d6fa0f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3d6fa0f4a5d43d7d8eff60d5bed70d566f4935f6). Проверки: missing 0, прежние значения BiblioCraft не изменены, дубликаты 0, placeholders 0, formatting 0, нижний регистр в названиях блоков/предметов не найден, непредусмотренных латинских строк не найдено.
- bibliowoods: EN-файл найден, но пуст (0 ключей).
- atmcompat: EN-файл содержит 10 ключей namespace allthemodium; все 10 уже присутствуют в опубликованном русском файле allthemodium.
- accelerateddecay: EN-файл найден, но пуст (0 ключей).
- ftbquests: локализация SNBT завершена; все 67 глав и общие языковые файлы проверены.

Chipped — переведён: `assets/chipped/lang/ru_ru.json`, 7265/7265 ключей, missing 0, extra 0, placeholders 0, formatting 0, непереведённых английских пользовательских строк 0. Коммит: [3d2ddac](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3d2ddac65d0dd725f1b8f31420f1680d58bf9bde). Следующая рабочая точка: `rechiseled` (3656 ключей, EN SHA `ed99e24fab965e740dcdcad021a76e7c7787c84e`).

## Проверка языковых источников — 05.11.2026

- BiblioCraft, Bibliobiomes и BiblioWoods используют общий namespace `bibliocraft`. Файл `assets/bibliocraft/lang/ru_ru.json` содержит 23 059 ключей (2021 + 9577 + 11461). Коммиты добавления дополнений: [3d6fa0f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3d6fa0f4a5d43d7d8eff60d5bed70d566f4935f6), [a3f3b0d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a3f3b0db5c5a5efb5ebc91330d0e5b097b5b4012). Общий blob SHA: `78e3da9f8afcc82ac062093b46bb4b9503bd01e6`.
- BiblioCraft base: 2021/2021 ключей, missing 0, placeholders 0; 12 EN/RU совпадений сохранены намеренно.
- Bibliobiomes: 9577/9577, missing 0, placeholders 0, formatting 0, duplicates 0, exact English matches 0.
- BiblioWoods: 11461/11461, missing 0, placeholders 0, formatting 0, duplicates 0, exact English matches 0.
- KubeJS Tweaks: исправлен файл `assets/kubejstweaks/lang/ru_ru.json`; теперь 4/4 ключа, missing 0, extra 0, placeholders 0. Коммит: [9ab2fda](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9ab2fdaf634bd81a22a10e45148e3af748540d50).
- ATM Compat: 10/10 ключей уже присутствуют в `assets/allthemodium/lang/ru_ru.json`; файл не менялся.
- Accelerated Decay, FTB JEI Extras, FTB XMod Compat, Illager Warship и Rechiseled Chipped: английские файлы пусты (0 ключей); отдельные пустые русские файлы не создавались.
- Следующий реальный перевод: Rechiseled (3656 ключей, EN SHA `ed99e24fab965e740dcdcad021a76e7c7787c84e`). Chipped завершён и опубликован. FTB Quests/SNBT — самый последний этап.


### Rechiseled — завершён 05.11.2026

- Файл: `assets/rechiseled/lang/ru_ru.json`, опубликован в [коммите 02cb14f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/02cb14fd9d433fbe8dd04f2c1bea8c78af669997).
- Английский оригинал: `ATM/LANGUAGES_EN_US/rechiseled-1.2.6-neoforge-mc1.21/rechiseled/en_us.json`, SHA `ed99e24fab965e740dcdcad021a76e7c7787c84e`.
- 3656/3656 ключей; missing 0, extra 0, дубликаты 0, placeholders 0, форматирование § и переносы строк 0.
- Использован ReRT-v3.zip из Dropbox. Из 3770 ключей основного JSON оставлены только 3656 ключей текущего EN-оригинала; 114 дополнительных ключей (в основном Pale Oak и несколько Quartz connecting) исключены как отсутствующие в версии ATM10.
- Исправлены отдельные UI-термины; терминология Rechiseled добавлена в `GLOSSARY.md` (коммит [4638e86](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4638e866d1b3c0fa9c644af6fa4ae6e339011ba4)).
- Интеграционные файлы AE2/Cobblemon из архива не включены в эту локализацию: их версии и полные наборы EN-ключей отдельно не сверялись.

Следующая рабочая точка определяется по актуальному `INVENTORY.md`; FTB Quests/SNBT остаются на самом конце проекта.


### Проверка следующих 10 mod ID — 05.11.2026

Проверены по полному дереву `ATM/LANGUAGES_EN_US` актуальной ветки `main` репозитория английских источников (406 файлов `en_us.json`, 403 уникальных namespace). Для следующих десяти mod ID отдельные английские языковые файлы в источнике не обнаружены; переводимые ключи по предоставленному источнику отсутствуют, отдельные русские JSON-файлы не создавались:

- `resourcefullib`
- `rhino`
- `smartbrainlib`
- `sodium`
- `sodium_extra`
- `sophisticatedbackpackscreateintegration`
- `sophisticatedstoragecreateintegration`
- `spark`
- `structory`
- `structory_towers`

Это означает отсутствие отдельного языкового источника в репозитории, а не подтверждение отсутствия строк внутри самих JAR. Если появится соответствующий EN-файл, эти позиции нужно перепроверить.


### Проверка ещё 10 mod ID — 05.11.2026

По полному дереву английских языковых источников проверены следующие позиции. Отдельных `en_us.json` для них не найдено; новые RU-файлы не создавались:

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

Отсутствие файла в репозитории источников не доказывает отсутствие строк внутри JAR; при появлении оригиналов позиции подлежат повторной проверке.


### Проверка десяти позиций — 05.11.2026

Три mod ID без отдельного языкового источника: `wits`, `yeetusexperimentus`, `yungsextras` (для YUNG's в источнике представлены отдельные namespace модулей). Семь дополнительных namespace, уже имеющих русские файлы, сверены с английскими оригиналами: `borderless` 21, `cloth-config2` 49, `dynamic_fps` 85, `entityculling` 27, `evilcraftcompat` 29, `integrateddynamicscompat` 213, `integratedterminalscompat` 19 ключей. Всего 443 ключа; после исправлений во всех семи файлах missing 0, extra 0, placeholders 0, formatting 0, duplicates 0.


### Завершение проверки дополнительных namespace — 05.11.2026

Сверены оставшиеся шесть дополнительных namespace: `irons_patreon_lib` (2), `lambdynlights` (63), `lollipop` (50), `moreculling` (55), `tempad_static` (84), `vulkanmod` (89). Все ключи соответствуют EN-оригиналам; пропусков, лишних ключей, ошибок плейсхолдеров и форматирования нет. Для Tempad проверены вложенные массивы/компоненты JSON; дубликатов ключей верхнего уровня нет.

Дополнительно проверены уже существующие переводы четырёх модулей YUNG's: `betterdeserttemples` (13), `betterdungeons` (86), `betterendisland` (13), `betterjungletemples` (11). Во всех четырёх файлах совпадают ключи, плейсхолдеры и форматирование. В Better Dungeons исправлено обращение «Установи» на единый вежливый стиль «Установите».


### FTB Quests / SNBT — финальный этап, состояние на 05.11.2026

- В английском источнике и основном RU-репозитории присутствуют все 67 файлов глав; имена файлов совпадают, отсутствующих и лишних файлов нет.
- Полностью сверены первые 10 глав: `achapter_2r_6the_atm_star`, `aether`, `allthemodium`, `apotheosis_2`, `apotheosis_gear`, `apothic_enchanting`, `applied_energistics_2`, `ars_nouveau`, `artifacts`, `auroral`.
- EN: 1068 ключей; RU: 1072 записи, включая 4 дополнительных перевода полей существующих quest ID, которых нет в EN overlay, но которые присутствуют в базовых файлах глав. Пропусков EN-ключей нет; 15 устаревших записей с отсутствующими ID удалены.
- Во всех 10 файлах: дубликаты 0, несоответствия плейсхолдеров 0, расхождения ссылок на изображения 0, SNBT-структура сбалансирована.
- Исправлены устаревшие описания двух мультиблочных квестов ATM Star и повреждённые кавычки вокруг двух изображений в массиве SNBT.
- Остальные 57 глав, общие `chapter.snbt` и `reward_table.snbt`, а также глобальные языковые SNBT-файлы ещё требуют проверки. FTB Quests не завершён.


### FTB Quests — вторая партия SNBT, 05.11.2026

Проверены главы: `basic_armor`, `basic_logistics`, `basic_power`, `basic_tools`, `bounty_board`, `building_tips`, `bumblezone`, `cataclysm`, `chapter_2_the_star`, `create`. Всего 1793 EN-ключей и 1823 RU-записей, включая 30 дополнительных RU-полей для quest ID, присутствующих в базовых SNBT. Missing 0, stale extra 0, duplicates 0, placeholders 0, image mismatches 0, все SNBT-файлы структурно сбалансированы. Удалено 14 устаревших записей с отсутствующими в базовых главах ID. Всего проверено 20/67 глав; осталось 47. Следующая партия: `create_addons`, `deeper_and_darker`, `draconic_evolution`, `elmystical_agriculturerr`, `eternal_starlight`, `evilcraft`, `extended__advanced_ae`, `extreme_reactors`, `food_and_farming`, `forbidden__arcanus`.


### FTB Quests — третья партия SNBT, 05.11.2026

Проверены главы: `create_addons`, `deeper_and_darker`, `draconic_evolution`, `elmystical_agriculturerr`, `eternal_starlight`, `evilcraft`, `extended__advanced_ae`, `extreme_reactors`, `food_and_farming`, `forbidden__arcanus`. EN-ключей 1477, RU-записей 1501, дополнительных RU-полей 24; все дополнительные поля ссылаются на quest ID, присутствующие в базовых SNBT. Удалено 20 устаревших записей. Missing 0, stale extra 0, duplicates 0, placeholders 0, image mismatches 0, SNBT balance OK. Всего проверено 30/67 глав; осталось 37. Следующая партия: `generators`, `hostile_neural_networks`, `ice__fire`, `immersive_engineering`, `industrial_foregoing`, `integrated_dynamics`, `iron_spells_and_spellbooks`, `justdirethings`, `mahou_tsukai`, `mainquestline_part_1`.


### FTB Quests — четвёртая партия SNBT, 05.11.2026

Проверены главы: `generators`, `hostile_neural_networks`, `ice__fire`, `immersive_engineering`, `industrial_foregoing`, `integrated_dynamics`, `iron_spells_and_spellbooks`, `justdirethings`, `mahou_tsukai`, `mainquestline_part_1`. EN-ключей 1220, RU-записей 1245, дополнительных RU-полей 25; все дополнительные поля ссылаются на quest ID в базовых SNBT. Удалена одна устаревшая запись с отсутствующим ID. Missing 0, stale extra 0, duplicates 0, placeholders 0, image mismatches 0, SNBT balance OK. Всего проверено 40/67 глав; осталось 27. Следующая партия: `mekanism`, `mekanism_reactors`, `mi_digital`, `mi_electric`, `mi_endgame`, `mi_steam`, `modular_router`, `natures_aura`, `neo_vitae`, `occultism`.


### FTB Quests — пятая партия SNBT, 05.11.2026

Проверены главы: `mekanism`, `mekanism_reactors`, `mi_digital`, `mi_electric`, `mi_endgame`, `mi_steam`, `modular_router`, `natures_aura`, `neo_vitae`, `occultism`. EN-ключей 1228, RU-записей 1250, дополнительных RU-полей 22; все дополнительные поля ссылаются на quest ID в базовых SNBT. Удалены 4 устаревшие записи с отсутствующими ID. Missing 0, stale extra 0, duplicates 0, placeholders 0, image mismatches 0, RGB mismatches 0, SNBT balance OK. Всего проверено 50/67 глав; осталось 17. Следующая партия: `oritech`, `pneumaticcraft`, `powah`, `productive_bees`, `productive_trees`, `pylons`, `railcraft`, `refined_storage`, `relics`, `silent_gear`.


### FTB Quests — продолжение аудита, 05.11.2026

Начата следующая десятка глав: `oritech`, `pneumaticcraft`, `powah`, `productive_bees`, `productive_trees`, `pylons`, `railcraft`, `refined_storage`, `relics`, `silent_gear`. Выполняется сверка с EN-оригиналами и базовыми SNBT. Партия не засчитана как завершённая до повторной проверки всех результатов. Подтверждённый прогресс: 50/67 глав; осталось 17.


## Заключительный аудит JSON — подтверждённые пропуски, 05.11.2026

Повторная сверка актуальных EN-файлов и текущих RU JSON подтвердила 3 неполных перевода (5750 отсутствующих ключей суммарно):

| Namespace | EN | RU | Missing |
|---|---:|---:|---:|
| `neovitae` | 3652 | 3652 | 0 |
| `mekanism` | 3239 | 3239 | 0 |
| `iceandfire` | 1809 | 1809 | 0 |
| `mekanismtools` | 800 | 800 | 0 |
| `silentgear` | 1191 | 616 | 575 |
| `supplementaries` | 1394 | 708 | 686 |
| `regions_unexplored` | 933 | 455 | 478 |
| **Итого** | **13018** | **7268** | **5750** |

По каждому из семи файлов: extra 0, пустых переводов 0, обнаруженных расхождений плейсхолдеров 0. Отсутствующие ключи требуют перевода.

### Дополнительные завершённые проверки

- `create_dragons_plus`: 356/356; удалён один лишний RU-only ключ. Missing 0, extra 0, placeholder mismatches 0, empty 0. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3a92c07d5c00d3a1ddd1d4c0272a17854ebf814d
- `sophisticatedstorage`: 425/425; missing 0, extra 0, placeholder mismatches 0, empty 0. Актуальное количество ключей — 425.
- `mekanismgenerators`: 364/364; missing 0, extra 0. Процент в значении `100%` не является плейсхолдером. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/513a0091918e9bfe9d232c1ea9d17bbabd61be3a


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

### Актуальное состояние семи локализаций после завершения Silent Gear

| Мод | EN | RU | Missing |
|---|---:|---:|---:|
| NeoVitae | 3652 | 3652 | 0 |
| Mekanism | 3239 | 3239 | 0 |
| Ice and Fire | 1809 | 1809 | 0 |
| Mekanism Tools | 800 | 800 | 0 |
| Silent Gear | 1191 | 1191 | 0 |
| Supplementaries | 1394 | 1394 | 0 |
| Regions Unexplored | 933 | 933 | 0 |
| Explorer's Compass | 68 | 68 | 0 |
| Measurements | 15 | 15 | 0 |
| Nature's Compass | 44 | 44 | 0 |
| **Итого** | **13145** | **13145** | **0** |

Десять модов текущей партии полностью сверены: NeoVitae, Mekanism, Ice and Fire, Mekanism Tools, Silent Gear, Supplementaries, Regions Unexplored, Explorer's Compass, Measurements и Nature's Compass. В последних трёх восстановлены только отсутствовавшие служебные поля _comment; пользовательские переводы уже были полными.



## Итог аудита 108 mod ID без одноимённого ru_ru.json и последующей локализации (05.11.2026)

Подробный отчёт: [NO_RU_JSON_AUDIT.md](NO_RU_JSON_AUDIT.md).

- Проверено 108 mod ID по официальному modlist ATM10 8.5.
- 89 модов не имеют собственного извлечённого `en_us.json` в архивной выгрузке; 5 найденных EN JSON пустые.
- ATM: Compat (10 ключей), Borderless Window (21) и Cloth Config (49) полностью покрыты существующими общими RU namespace.
- FTB Quests (774 ключа) оставлен для финального этапа.
- Colorwheel, Colorwheel Patcher, ImmediatelyFast и Uranus не требуют отдельной локализации по найденным ресурсам и назначению.
- Bibliobiomes 1.6.1: 9577/9577 ключей покрыты в общем `bibliocraft` namespace.
- Bibliowoods 1.6.2: 10833/10833 ключей покрыты в общем `bibliocraft` namespace; добавлено 157 переводов для Mauve.
- Iris: 73/73; IrisSearch: 13/13; Sodium: 89/89; Sodium Extra: 418/418. Для этих четырёх модов созданы отдельные русские JSON.
- По всем шести модам из очереди локализации проверены ключи, лишние записи, пустые значения и плейсхолдеры: пропусков и ошибок плейсхолдеров нет.

Все шесть модов из очереди аудита локализованы; 108-кандидатный список больше не является незакрытой очередью работ. FTB Quests/SNBT остаётся отложенным на конец проекта.


## Контрольная точка NeoVitae — 05.11.2026

В рабочей ветке `work/neovitae-ru` добавлено 600 новых переводов к ранее имевшимся 281 ключу. Текущее покрытие: **881/3652**, отсутствует 2771 ключ. Проверка актуального EN 1.1.51: extra 0, duplicates 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0; JSON корректен. Перевод не завершён и не опубликован в `main`.


## Контрольная точка NeoVitae — 05.11.2026 (вторая партия)

В ветке `work/neovitae-ru` добавлено ещё **600 новых ключей** к подтверждённому состоянию 881/3652. Текущее покрытие: **1 481/3 652**, отсутствует 2 171 ключ. Проверка актуального `neovitae-1.21.1-1.1.51`: JSON корректен; extra 0, duplicates 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0. Работа продолжается; в `main` не опубликована.


### Актуальная контрольная точка NeoVitae — 05.11.2026

В рабочей ветке `work/neovitae-ru` добавлено **600 новых ключей** к подтверждённому состоянию 881/3652. Текущее покрытие: **1 481/3 652**, отсутствует 2 171 ключ. Проверка актуального `neovitae-1.21.1-1.1.51`: JSON корректен; extra 0, duplicates 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0. Перевод продолжается; в `main` не опубликован.


### Актуальная контрольная точка NeoVitae — 05.11.2026

Текущее состояние рабочей ветки `work/neovitae-ru`: **1 481/3 652 ключей**, missing 2 171. После подтверждённой точки 881/3 652 добавлено 600 новых ключей. Сверка с актуальным EN 1.1.51: JSON корректен; extra 0, duplicates 0, empty 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0. Перевод не завершён и не опубликован в `main`.


### Актуальная контрольная точка NeoVitae — 05.11.2026

Текущее состояние рабочей ветки `work/neovitae-ru`: **1 541/3 652 ключей**, missing 2 111. После контрольной точки 881/3 652 добавлено 660 новых ключей. Сверка с актуальным EN 1.1.51: JSON корректен; extra 0, duplicates 0, empty 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0. Перевод не завершён и не опубликован в `main`.


### NeoVitae — продолжение от 2 835 ключей (05.11.2026)

В рабочей ветке `work/neovitae-ru` переведено ещё **20 ключей** руководства: заряды для валки деревьев и грибов, Адское горнило, Lex Vitae, маршрутизатор узлов и начальные страницы переработки руды. По проектному счётчику: **2 855/3 652**, осталось **797** значений.

Техническая сверка JSON с EN 1.1.51: RU-записей 2 898; missing keys 754, extra 0, duplicates 0. Для 20 новых строк проверены цветовые маркеры, экранированные переносы и плейсхолдеры — расхождений 0. Разница между проектным остатком (797) и отсутствующими ключами (754) связана с уже существующими RU-ключами, значения которых ещё требуют отдельной смысловой проверки на совпадение с английским текстом.

Коммиты переводов: [2aac1c5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2aac1c5736292c8e4eea53be9385e7ce72ab5f5d), [5b40181](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5b401816eb57dccc4378dfd14090f5e2bd5a2d20), [9f0a2ff](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9f0a2ff95f5685aac32dcf1f42d8e9e48f9ddb7a).

NeoVitae не завершён и в `main` не переносился. Продолжать в `work/neovitae-ru`.


## Завершение локализации NeoVitae — 05.11.2026

В ветке `work/neovitae-ru` переведены все **3 652 из 3 652** ключей актуального английского файла `neovitae-1.21.1-1.1.51`. Дополнительно проверены ранее существовавшие совпадения с EN: оставлены без изменений только названия собственных сущностей, латинские названия аспектов/ритуалов и технические значения; обычные подписи интерфейса и термины исправлены.

Финальная сверка:
- EN/RU: 3 652 / 3 652; missing 0; extra 0.
- Дубликаты ключей: 0; пустые значения: 0.
- Ошибки плейсхолдеров: 0; несовпадения переносов строк: 0; несовпадения форматирующих кодов Minecraft (§): 0.
- JSON корректен.

NeoVitae полностью переведён и проверен в рабочей ветке. До отдельного решения о публикации партии изменения в `main` не переносить.


## Productive Trees — завершение локализации (05.11.2026)

Актуальный английский оригинал: `productivetrees-1.21.1-1.1.1/productivetrees/en_us.json`.

- EN: 4 149 ключей.
- RU до работы: 3 832 ключа; missing 317; extra 0.
- Добавлено: 317 переводов.
- RU после работы: 4 149 ключей; missing 0; extra 0.
- Дубликаты ключей: 0.
- Ошибки плейсхолдеров: 0.
- Несовпадения переносов строк и кодов форматирования Minecraft (§): 0.
- JSON корректен.
- Четыре совпадения RU=EN оставлены обоснованно: два латинских ботанических названия (`Laurus nobilis`, `Maclura pomifera`), пустое значение исходного ключа `thunder_bolt.latin` и технический плейсхолдер `%s`.

Перевод опубликован в рабочей ветке `work/productivetrees-ru`; `main` не изменялся. Коммит: https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9c314b46f925358fdc01d66945f14bb88b482deb.


## Завершение локализации Silent Gear — 05.11.2026

Silent Gear для ATM10 8.5 полностью переведён в ветке `work/productivetrees-ru`: **1 191/1 191 ключ**. В исходном RU-файле было 617 ключей; добавлено 574 перевода. Существовавшие 617 значений сохранены. Переведены достижения, блоки, команды, интерфейсы машин, типы снаряжения, предметы и детали, JEI, материалы, характеристики, конфигурация и свойства.

Финальная сверка с read-only EN-файлом `silent-gear-1.21.1-neoforge-4.2.1.1/silentgear/en_us.json` (SHA `458a50aed74a049d099ab97bf14723b0fb91dc1b`): JSON корректен; EN/RU 1 191/1 191; missing 0; extra 0; дубликаты ключей 0; несовпадения плейсхолдеров 0; несовпадения кодов форматирования Minecraft (§) 0; несовпадения количества переносов строк 0. Три ранее совпадавших с EN описания достижений дополнительно переведены после смысловой проверки. Оставшиеся совпадения RU=EN — технические подписи, плейсхолдеры, название мода и буквенные/ранговые обозначения grade (A–E, S–SSS, MAX). Внутриигровое тестирование не проводилось.

Коммиты перевода: [4ae2a83](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4ae2a83cde5048aea1fc242a42b03adbd30ae04f), [5269ad8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5269ad88435aae15f3035ecd3aec35515e5fd185), [eaa0f20](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/eaa0f204c8d59459a3933f3ea5e4163135e8fc02), [e135d5b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e135d5b417c92e23b69414837ed8a21effd11f0e), [fa0a4f0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fa0a4f092ffb0414554c66329d7e621e1a729665), [d80af99](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d80af9995dfb5d98442ca28ac25391bf684332b3), [0a44d35](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0a44d3596f2bcb55d8d0ab41fa8b0e25610cd67c), [28e31bb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/28e31bb921f5dc0bda0762c7ba309005e9645391), [bd843c7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bd843c72bd123a157d4b03a2fc9c383e45651544), [0ca79f8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0ca79f848316918b55707c608135fec1195274cd) — финальная смысловая правка трёх достижений.

Работа опубликована только в рабочей ветке; `main` не изменялся. Следующая точка очереди — Supplementaries, затем Regions Unexplored. FTB Quests/SNBT остаются на финальном этапе.


## Завершение локализации Supplementaries — 05.11.2026

Supplementaries `4.0.2` полностью локализован в ветке `work/productivetrees-ru`: **1 394/1 394 ключа**. Исходный RU-файл содержал 708 ключей; добавлено 686 переводов. Сверка с read-only EN-файлом `supplementaries-1.21.1-4.0.2-neoforge/supplementaries/en_us.json`: missing 0, extra 0, duplicates 0, пустых значений 0, несовпадений плейсхолдеров 0, кодов форматирования Minecraft (§) 0, переносов строк 0; JSON корректен. 10 совпадений RU=EN оставлены как технические подписи/плейсхолдеры, название мода и имена авторов картин.

Коммиты перевода: [1162f92](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1162f92d8b1e1ff563eb40c024464b2e533f68b1), [1c25611](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1c25611518aa94613cc31055a05dc19812d1a1eb), [5d3b00b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5d3b00ba4aaa600ac2e309a70d5cac8facc980e7), [467d558](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/467d558dc9f34d8a374f82d8a001895aaf8ddb58), [77b513c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/77b513cdce529c84312404a43c07a6f5a5f9ded1), [c2bde08](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c2bde08bb7af919ea4b540ee705a57b2806a26ba), [a7d2542](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a7d2542ba9706c5574b0a918c4597630606fba1e), [1e570c4](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1e570c403fc3d6c5ab69eb0703b7e83287ff61dd), [28163da](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/28163dae789f5c7d759f13869993a7acb28fb6ad), [4f7685d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4f7685dc0a944d97bafe22aee69c4aa6e65fae7c), [ebedc5b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ebedc5ba3e944667319a9cfdd612b2c49904e15f), [17ed953](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/17ed9539adb2fe53fa5cc2ff6d3492eb4eb0ebe6), [67ec6db](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/67ec6dbfd75c42231aba1aeec39edecb8a181399), [94a68e7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/94a68e77c3de2467656bfd63f05a38ec6516c491), [c4c83c6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c4c83c66ca8cec569e91325114b376514ed1b997), [0e0edb5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0e0edb5445c73d543f148f55a32f9cd5a84b9b39), [b9f4314](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b9f431460a1a477891e20dc7bf0f1006f0a051dd), [7fd79ec](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7fd79ec80befe0580832671348ba0403112b9cd8), [0715ec2](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0715ec213a6f0a35793105ec6c75dd2fee7a3c4e), [2868ee7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2868ee73895dab557bdfeb1f8f7540d1291d9e77), [1c1d74e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1c1d74eced833a03982bc04fb62b8499b18c4eee), [7b52763](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7b52763403483dccd692d3608e0c19a97545b889), [3a8a44b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3a8a44be2dd79efbee8c5a2e6065502400593748), [7e140dc](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7e140dc0380765fdc274d9a71eb9722c6a2e5b42), [b89ab14](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b89ab1451140aa9f95dc6bbbe9101552f9fc2077), [c398256](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c398256d1a6311da13a7c788d147612ccd68ed5a), [d80a2b7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d80a2b7d2f5321e4d48cdc5987d1e1bd7ba81230), [ed92d28](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ed92d280a2d0c80910f3355ee00a78e56f08ef95), [1ccf560](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1ccf5608ddd77c0db0786b9b54f29e088cf9c66c), [fb3cc1a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fb3cc1a5771aad3d507777d12894099f33cd92da), [cfc8c1e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cfc8c1ef209cc3f137b80ed8f90e9dc4312bdcd9), [cd31c72](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cd31c72d9f4d7b1fe9fa9e2487267c22d754d60e), [4a23617](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4a23617062e8661ce6ae4bc7916b8b3fc1db260d), [88460c3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/88460c3d98d2349d906e7ebab4341710e2f6f291), [33eccc1](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/33eccc11a45bad94e7b07db4370c60767127d1bd), [0ea5de0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0ea5de0904068c96aa80c8d872a493fa8cc0c3a9), [f4a62cd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f4a62cd267624d846e216cedad68b0a43585f030), [4bbf087](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4bbf08765b82536b5ba5c118c0a2b6fce76601e7), [1170514](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/11705141a247c56fcb01c9bfd7a5185ee490a13b), [101fe88](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/101fe88efa79d29e707ede439903dc325fde543a), [16ba9ee](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/16ba9eeb304aa51385cf23e0d28f44cbf41f9d9d), [3a009e3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3a009e3fccf1c678e13a62a538319e6de1557138), [35ac622](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/35ac622e39c36ccc43e76ac4154ea3524a3e8616), [aa595b8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/aa595b8161785cd8eaf7e4d3a6b6ae78567e449a), [a736155](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a736155f1cbad2e2f0ea0ab45287fe43b5f719e1), [8c37d03](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8c37d033347b8c1798a144ad1a5f9466ed774ae5), [f6cc74f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f6cc74ff97bb21863025693b7d45aace5051ce0d), [ddd4cad](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ddd4cad47326a72a97f05fc851f00961338047f4), [756e1f0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/756e1f0e2c1b6fca49a3b658b5c4e4f993cbd23c), [0d135b6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0d135b6f85d886e2c41c31bdbbd2a5fde75099f5), [e86223b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e86223bcd60c6ce714a05dd6c75b80a5911a4397).

Глоссарий Supplementaries дополнен отдельными терминами. Следующая точка очереди — Regions Unexplored. Работа опубликована только в рабочей ветке; `main` не изменялся. Партия из десяти модов пока не завершена.


## Завершение локализации Regions Unexplored — 05.11.2026

Regions Unexplored `0.6.3-neoforge-21.1` полностью локализован в ветке `work/productivetrees-ru`: **933/933 ключа**. Исходный RU-файл содержал 455 ключей; добавлено 478 переводов. Сверка с read-only EN-файлом `regions-unexplored-0.6.3-neoforge-21.1/regions_unexplored/en_us.json`: missing 0, extra 0, duplicates 0, пустых значений 0, несовпадений плейсхолдеров 0, кодов форматирования Minecraft (§) 0, переносов строк 0; JSON корректен. Единственное совпадение RU=EN — название мода в творческой вкладке, оставленное без перевода намеренно.

Коммиты перевода: [304a42e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/304a42eed4878f680ad633c7df2ea002efb7550d), [7e9600f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7e9600f6b696407b6766cb0fde91297e73813928), [c8addb0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c8addb0b2e17a9f14892d3a493a34c6922876091), [dc83b6e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/dc83b6e4bd9a3b0d64952173dce57458a3ff9dd5), [f2a1036](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f2a10366f25d03b02c33d38f393f8ef0363c0281), [7affad8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7affad8265968599924b64d9fff82e25b42208c9).

Глоссарий дополнен терминами Regions Unexplored: [c844fe5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c844fe56b5115795d82fc4c9b59793f7b80fe7d5). Следующая точка — выбрать три следующих незавершённых мода после проверки INVENTORY.md и актуального дерева английских источников. Работа опубликована только в рабочей ветке; `main` не изменялся. FTB Quests/SNBT остаются на финальном этапе.


## Завершение партии из десяти локализаций — 05.11.2026

Партия закрыта: 10/10 модов. Семь крупных локализаций доведены до полного EN/RU-покрытия; ещё в трёх ранее переведённых файлах восстановлены отсутствовавшие служебные поля _comment для точного совпадения с EN.

- Explorer's Compass: 68/68, missing 0, extra 0, placeholders 0, formatting 0, newlines 0; commit [9cfe773](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9cfe773670b156ea801e8a53c2a9feeb6fcbc1e8).
- Measurements: 15/15, missing 0, extra 0, placeholders 0, formatting 0, newlines 0; commit [9c6c48a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9c6c48a3a76b66b7827d2871525da9ec2e08870a).
- Nature's Compass: 44/44, missing 0, extra 0, placeholders 0, formatting 0, newlines 0; commit [1b1cb11](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/1b1cb114c2a8fd8bd22212e99fe9e9f445c5451d).

Следующий кандидат в новой партии — Ad Astra: 831 EN-ключ, 685 RU-ключей, 146 отсутствующих, extra 0. В ходе дополнительной проверки также найден один отсутствующий служебный ключ ZeroCore (EN/RU 50/49); он остаётся в очереди.


## Актуальная контрольная точка — 05.11.2026

Ветка `main` содержит завершённую партию из 10 JSON-локализаций (сверка с EN ATM10 8.5):

| Namespace | EN/RU | Missing | Extra | Placeholder mismatches |
|---|---:|---:|---:|---:|
| `ad_astra` | 831/831 | 0 | 0 | 0 |
| `mekanism` | 3239/3239 | 0 | 0 | 0 |
| `iceandfire` | 1809/1809 | 0 | 0 | 0 |
| `neovitae` | 3652/3652 | 0 | 0 | 0 |
| `productivetrees` | 4149/4149 | 0 | 0 | 0 |
| `silentgear` | 1191/1191 | 0 | 0 | 0 |
| `supplementaries` | 1394/1394 | 0 | 0 | 0 |
| `regions_unexplored` | 933/933 | 0 | 0 | 0 |
| `aether` | 1238/1238 | 0 | 0 | 0 |
| `mekanismtools` | 800/800 | 0 | 0 | 0 |
| **Итого** | **19236/19236** | **0** | **0** | **0** |

Публикация: merge commit [a49e765](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a49e7659d0c8eded7295a92b95d3a8c5f5087a46), Aether [30bbf0d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/30bbf0d4b3f4386cf846d45d458fffe0b94bd185), Mekanism Tools [cb90493](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cb9049377678f3ed0479f6fe922ae25e5398cc32).

Проверка Mekanism Tools дополнительно исправила последнее пустое значение; оно теперь «Шанс появления нескольких частей брони». Восьмёрка переводов из PR #4 была ранее полностью сверена в рабочей ветке и теперь опубликована в `main`.

Следующие подтверждённо неполные namespace: `ars_nouveau`, `evilcraft`, `irons_spellbooks`, `pneumaticcraft`, `twilightforest`, `industrialforegoing`, `integrateddynamics`, `reliquary`. Для `actuallyadditions` требуется отдельная смысловая проверка 82 значений, совпадающих с EN; пустое значение ключа `info.actuallyadditions.gui.the` может быть языковой особенностью (в русском нет артикля), поэтому не заменять его механически. Перед следующей партией проверить дополнительные неполные namespace и выбрать десять фактических целей.


## Дополнение текущей рабочей сессии — 05.11.2026

- `actuallyadditions`: 1026/1026, missing 0, extra 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0. Переведены 62 пользовательские строки, ранее совпадавшие с EN. Пустое `info.actuallyadditions.gui.the` сохранено намеренно: русский язык не использует артикль. Бренд, CF/NBT/ESD и служебные комментарии оставлены без перевода.
- `industrialforegoing`: 683/683, missing 0, extra 0, empty 0, placeholder mismatches 0, newline mismatches 0, formatting mismatches 0. Оставшиеся совпадения EN/RU относятся к названию мода, FE и служебным комментариям.

Коммиты Actually Additions: [6146656](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/61466567329721c466729420646696fb7504c3b2), [c74229a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c74229a20476239869f02082311d8d99b8fafc61). Коммиты Industrial Foregoing: [23032f0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/23032f0d5ad06fcb3afefa9b560b702b82f552bd), [7a3f978](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7a3f97825e6b1a29346d171fd553e3772edb27a8).

Текущая партия не завершена: 2/10. Следующий мод — `irons_spellbooks` (1128/1315; missing 187). Upstream RU не использовать как замену: файл неполный; допустимо переносить только отдельные значения после проверки ключей и плейсхолдеров.

## Завершение локализации Iron's Spells 'n Spellbooks — 05.11.2026

`irons_spellbooks` (`3.16.3`) полностью локализован: **1 315/1 315 уникальных ключей**. В исходном RU-файле было 1 128 ключей; добавлено 187 переводов. Существовавшие RU-значения сохранены.

Сверка с read-only EN-файлом `irons_spellbooks-1.21.1-3.16.3/irons_spellbooks/en_us.json` (blob SHA `beadca863ebede25d55c7615f1a99c12b4b7249c`): JSON корректен; missing 0; extra 0; дубликаты RU-ключей 0; пустых значений 0; несовпадения плейсхолдеров 0; несовпадения кодов Minecraft (§) 0; несовпадения количества переносов строк 0. 14 совпадений RU=EN оставлены намеренно: технические шаблоны, название мода и римские обозначения уровней. Обычных непереведённых пользовательских строк среди совпадений не осталось.

**Особенность английского оригинала:** в EN-файле дважды объявлен ключ `death.attack.blood_magic` (строки 760 и 778); при разборе JSON действует последнее значение. В RU оставлен один ключ с переводом последнего, полного английского значения. Сам EN-файл не изменялся.

Коммиты:
- Перевод: [2ecbb4e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2ecbb4e10d59353fb6b76e97f2c8f5f213c3540b), [330c4c7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/330c4c78a480ddcf7e9ba2ae8e852f6f3931fde2), [6843521](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/68435214d97db7ae1b63b22440cef70268e77e99), [2567c09](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2567c09603df9b2b68f66450ce3990b33effc69f).
- Глоссарий: [коммит](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/02c7633734f452e66d64b6f139b631c4b4f2f7a9).

## Завершение локализации EvilCraft — 05.11.2026

`evilcraft` (`1.2.100`) полностью локализован: **629/629 ключей**. В исходном RU-файле было 376 ключей; добавлено 253 перевода. Существовавшие значения сохранены, кроме исправления выявленных расхождений форматирования в пользовательских текстах книги.

Сверка с read-only EN-файлом `evilcraft-1.21.1-neoforge-1.2.100/evilcraft/en_us.json` (blob SHA `85edb2f5a29645b01ac436ddc90e150a1b79407f`): JSON корректен; missing 0; extra 0; дубликаты RU-ключей 0; пустых значений 0; несовпадения плейсхолдеров 0; переносов строк 0; несовпадения кодов Minecraft (§) и форматирующих кодов книги (&) 0. Пять совпадений RU=EN оставлены намеренно: название мода/группы предметов и римские обозначения уровней.

В английском оригинале обнаружено 9 повторных объявлений ключей (`_comment` и subtitle-ключи); в RU-файле повторов нет. Для сверки использованы уникальные ключи после разбора JSON; EN-файл не изменялся.

Коммиты перевода: [4427380](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/44273800b06b8b7c692e2495a50ef16039243333), [1929218](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/192921836e3b2959eac96f3d4d5f58d2dd77a31c), [676c20e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/676c20e82fd9a2b2e64bd1ef6ac293e95ac06c8b), [afd8bcf](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/afd8bcfdce25aae5e5a06d4d2eaa6b21c9f89444), [29f0a59](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/29f0a5934ee0ab3246d2441c365be9943bbf7754), [2be1727](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2be1727a45f1b1313608b62ef122c07c2b1751d7).
- Глоссарий: [коммит](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5d976621540f09f7e4cca77d1c77237643807602).

## Завершение локализации PneumaticCraft: Repressurized — 05.11.2026

`pneumaticcraft` (`8.2.24`) полностью локализован: **2 274/2 274 ключа**. В исходном RU-файле было 1 987 ключей; добавлено 287 переводов. Также исправлены ранее существовавшие пользовательские ошибки в подсказках GPS-инструментов, справке фильтра существ, редакторе таблички, сообщениях Амадрона, описании улучшения дальности брони и нескольких строках форматирования.

Сверка с read-only EN-файлом `pneumaticcraft-repressurized-8.2.24-mc1.21.1/pneumaticcraft/en_us.json` (blob SHA `ca0b980ce454e782d23cdb8b4821faad90febfa3`): JSON корректен; missing 0; extra 0; дубликаты 0; пустых значений 0; несовпадения плейсхолдеров 0; переносов строк 0; несовпадения кодов Minecraft (§) 0. 22 совпадения RU=EN оставлены намеренно: названия/бренды, FE/RF/µI/CF, координатные оси, единицы измерения, шаблоны вывода и внутренние идентификаторы Jade.

Коммиты перевода: [f83e2ed](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f83e2ed07c312f5376dd783ae727cb34fb210d1c), [fb749b5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fb749b5e45ed4d48f6ae0e34e2d23a0a2309a8c4), [59dc0f2](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/59dc0f279846eb0155b8ee085275696427a8853b), [2d8c0bf](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2d8c0bf2e3d618587c857fbcab924ea0bf206eb0).
- Глоссарий: [коммит](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d238d3fb1ccda22a2ade88d74d2f1eb59aead27e).

## Завершение локализации Twilight Forest — 05.11.2026

`twilightforest` (`4.8.3345`) полностью локализован: **2 061/2 061 ключ**. В исходном RU-файле было 1 475 ключей; добавлено 586 переводов. Существовавшие значения сохранены; исправлены только точечные расхождения порядка плейсхолдеров и лишние пробелы в нескольких старых строках.

Сверка с read-only EN-файлом `twilightforest-1.21.1-4.8.3345-universal/twilightforest/en_us.json` (blob SHA `d378c0a02c7d95983b998781f792071bd612cdb5`): JSON корректен; missing 0; extra 0; дубликаты 0; пустых значений 0; несовпадения плейсхолдеров и их порядка 0; переносов строк 0; кодов форматирования 0; переменных `${...}` 0; расхождений завершающих пробелов 0. 18 совпадений RU=EN оставлены намеренно: названия композиций и авторов, командный шаблон, служебные обозначения, форматные символы и отступ.

Коммиты перевода: [4ee350b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4ee350b29b217ed85f5466fcf8feebfddd8a5d79), [4095f18](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4095f18ce3a0e6da8acf3317910a3f1e5fd1da32), [137ddde](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/137ddde891f3c955df1b068b61a536e656ef82e9), [0776c50](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0776c50e2722cc7b821964adc43435d59fbf2eae), [3b83005](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3b83005dac8dbd9483775837ce6d56ea9c9c26d1), [2cc21eb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2cc21eb25c39707c087e23f405e6576c94fb02d1), [c95129b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c95129bd7029aea85842c0d015bb4d1996e5c43b).
- Глоссарий: [коммит](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/60e4b6dd6f2923b90903cc8d516057d01eafa808).

## Завершение локализации Integrated Dynamics — 05.11.2026

`integrateddynamics` (`1.38.2`) полностью локализован: **1 854/1 854 ключа**. В исходном RU-файле было 1 629 ключей; добавлено 225 переводов. Также выровнены старые строки справочника по форматирующим кодам и исправлены некоторые формулировки учебника.

Сверка с read-only EN-файлом `integrateddynamics-1.21.1-neoforge-1.38.2/integrateddynamics/en_us.json` (blob SHA `9ed96bd78177b0786a0a9ff3a6b488cb335c1f6b`): JSON корректен; missing 0; extra 0; дубликаты RU-ключей 0; пустых значений 0; несовпадения плейсхолдеров 0; переносов строк 0; кодов форматирования (§ и &) 0; интерполяций 0; расхождений завершающих пробелов 0. В EN-файле два повторных объявления (`_comment` и `aspect.aspecttypes.integrateddynamics.integer.range`); в RU повторов нет. 10 совпадений RU=EN оставлены намеренно: RF, NBT, TPS, название мода и техническая строка ID.

Коммиты перевода: [d65e0f7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d65e0f74aba6fea851920893f4ad18151d97ddaf), [2882337](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2882337cf799a7ad8d4e0d913c9880ee65d6f0ce), [c0be297](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c0be297cb38fdd9a0d2f51c4263ca00a4c204a0a), [aa16aa2](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/aa16aa2f4a35f3b49b6632c93a137a121b76c5d4), [eb47cde](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/eb47cdeff037a1afac580b0be98bbe63cea128c0).
- Глоссарий: [коммит](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cdf0da7423c155537729248edda11519142b280a).

## Завершение локализации Reliquary — 05.11.2026

`reliquary` (`2.0.81.1579`) полностью локализован: **551/551 ключ**. В исходном RU-файле было 307 ключей; добавлено 244 перевода. Дополнительно исправлены старые ручные переносы строк в подсказках и описаниях, чтобы их количество точно совпадало с EN.

Сверка с read-only EN-файлом `reliquary-1.21.1-2.0.81.1579/reliquary/en_us.json` (blob SHA `d746dca920f938a59e80dffe9e4c5f6374fbfdb1`): JSON корректен; missing 0; extra 0; дубликаты 0; пустых значений 0; несовпадения плейсхолдеров 0; переносов строк 0; кодов форматирования 0; расхождений завершающих пробелов 0. 12 совпадений RU=EN оставлены намеренно: бренд мода, Shift, римские цифры, служебные шаблоны и обозначения.

Коммиты перевода: [af1e379](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/af1e37920f13865a8fe6742cf139a0782f9ba79c), [e715c2c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e715c2c290a43059bc4f71ceadb8e80a4b8c4b0e), [4df0756](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4df0756a43456af1bdf1267326fc08a44f526905), [318476b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/318476b356d0dbbabb8712997d579161acb00ebb), [b408fb1](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b408fb151c36ffd3333d208f0aafda5bb1f09047), [fff4284](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fff4284c96f785496544bfba6f627b1d3b5024dc).
- Глоссарий: [коммит](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cb774ff61bfb4c8b4a04022de7bbfc43912d8891).

## Завершение локализации Ars Nouveau — 05.11.2026

`ars_nouveau` (`5.13.3`) полностью локализован: **2 323/2 323 ключа**. В исходном RU-файле было 1 296 ключей; добавлено 1 027 переводов. Дополнительно пересмотрены устаревшие записи справочника и выровнена терминология Истока, связей с Истоком, камеры вливания, аппарата зачарования и фамильяров.

Сверка с read-only EN-файлом `ars_nouveau-1.21.1-5.13.3/ars_nouveau/en_us.json` (blob SHA `b16592155b2b4531aad4cfcc5a3bb1869505219d`): JSON корректен; missing 0; extra 0; дубликаты 0; пустых значений 1 (соответствует пустому значению EN); несовпадения плейсхолдеров 0; переносов строк 0; кодов форматирования 0; расхождений начальных/конечных пробелов 0. 10 совпадений RU=EN оставлены намеренно: название/мем Wololo, шаблоны и координаты, название стиля, названия музыкальных композиций и имена авторов.

Коммиты перевода: [a113ce3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a113ce37d8c8d606044fbcb6f49e4270ee30ff13), [0caf1ed](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0caf1ed8221fd735439d73ba2ee87a8d873e1069), [0fd225f](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0fd225f8864fe9467974c0cd3504af5a302d6bd4), [0034bf5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0034bf5a9a323dc175aa86edf611aa9d067e7f35), [8ee5c50](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8ee5c5074bfdfca9e4d5829529a89b0b2a9cc8f9), [69cbd0c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/69cbd0c905a152e81e659599ea5d7a60905ef996), [3efa0af](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3efa0af633db83f7a775738493dea38549631031), [57e04a6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/57e04a6adf82e0ca09e6e41b8956f654fd4663d1), [f3905da](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f3905da73702a4322c8653cc8a4d086d7228d957), [ca25b56](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ca25b563231658461f3d8650cec519acea0c9330), [36bf355](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/36bf355a621d8b8e7ec3ed3af8ba9275b55e3fb1), [08ff5e3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/08ff5e32a9d506732e41835c5bc62007d4e392a8), [af9a658](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/af9a658bd97e6c8faff5a402f527ea326691a12b), [921037e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/921037e879ddf2573d07aaf825f7e9486f6203d3), [155e7fd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/155e7fda7e5fd56a5a1f85edb6e617e0897b4022).
- Глоссарий: [коммит](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d63a95903d7dd1a51385e17f8862e4ab3202e1d3).


## Завершение локализации Mekanism: MoreMachine — 06.11.2026

- Namespace: `mekmm`; файл: `assets/mekmm/lang/ru_ru.json`.
- Английский оригинал (read-only): `ATM/LANGUAGES_EN_US/mekmm-1.21.1-1.4.2/mekmm/en_us.json`, blob SHA `98b0105375993268312f6c8bf18103bf5ae8d867`.
- EN/RU: **704/704 ключа**. В импортированном файле из Dropbox все ключи уже присутствовали, но 223 пользовательских значения полностью совпадали с английским оригиналом. Эти строки переведены с учётом механик Mekanism: MoreMachine и терминологии Mekanism; существовавшие качественные переводы сохранены.
- Проверки: JSON корректен; missing 0; extra 0; дубликаты 0; пустых значений 0; оставшихся точных совпадений RU=EN 0; несовпадений плейсхолдеров 0; форматирующих кодов (§ и &) 0; переносов строк 0; интерполяций 0; расхождений начальных/конечных пробелов 0.
- Перевод: [5087a5c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5087a5c90e2907574d447a4ab81d771de073237b), уточнения: [7bbcfd5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7bbcfd52197ae7edfa150f33e6146bd228f8259c), [16b0934](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/16b0934e9562cc90ccf77f1d06490ca5d95e51d1). Терминология: [e445dbf](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e445dbfc5064f8946f25216fac6435bb2918bdcc).


## Партия аудита JSON — 06.11.2026: Applied Energistics и дополнения

Проверены и завершены 10 namespace. Для всех файлов сверены актуальные EN-ключи и RU-файлы рабочей ветки; проверены JSON, missing/extra, дубликаты, пустые значения, плейсхолдеры, коды форматирования (§ и &), переносы строк, интерполяции и начальные/конечные пробелы.

| Namespace | EN/RU | Missing | Extra | Duplicates | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|
| `ad_astra_giselle_addon` | 168/168 | 0 | 0 | 0 | 0 |
| `additional_lights` | 157/157 | 0 | 0 | 0 | 0 |
| `advanced_ae` | 246/246 | 0 | 0 | 0 | 0 |
| `advancedperipherals` | 140/140 | 0 | 0 | 0 | 0 |
| `ae2` | 1 021/1 021 | 0 | 0 | 0 | 0 |
| `ae2ct` | 19/19 | 0 | 0 | 0 | 0 |
| `ae2importexportcard` | 8/8 | 0 | 0 | 0 | 0 |
| `ae2netanalyser` | 38/38 | 0 | 0 | 0 | 0 |
| `ae2wtlib` | 46/46 | 0 | 0 | 0 | 0 |
| `aeinfinitybooster` | 26/26 | 0 | 0 | 0 | 0 |
| **Итого** | **1 869/1 869** | **0** | **0** | **0** | **0** |

В 17 оставшихся совпадениях RU=EN сохранены только названия модов/брендов, обозначения FE, OpenComputers, P2P, служебный `_eof` и шаблоны с плейсхолдерами. Обычных непереведённых пользовательских строк среди совпадений не осталось.

Смысловые и терминологические правки:
- Advanced Peripherals: исправлены описания достижений, NBT Storage, Block Reader, Colony Integrator, ME Bridge и RS Bridge; нормализовано обращение и пунктуация.
- Advanced AE: исправлена подсказка Evasion, убран лишний завершающий пробел.
- Applied Energistics 2: исправлены команды, подписи SCS, выбор ЦП и название фиолетового стеклянного МЭ-кабеля; нормализована пунктуация и пробелы.
- Глоссарий дополнен терминами AE2 и дополнений.

Коммиты: Advanced Peripherals [585f167](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/585f167ee7e7e2a2cbbacbb9647a9d60ab4d7ea4), [e26d9bb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e26d9bb351e0558a7fadd43857d3396f7d3e5274); Applied Energistics 2 [d9d7687](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d9d768712dd2f5cd0e9b0d70a2d1baf26918dee2); Advanced AE [475187a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/475187a9e7bf4ea5f4ebc6b1ceb54b3e158ed3ac); глоссарий [2f0416a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2f0416adfd15844ba2994f4be858c848a2905548).


## Партия аудита JSON — 06.11.2026: Akashic Tome — Apotheosis

Проверены и завершены следующие 10 namespace. Для каждого файла сверены актуальные EN/RU ключи и выполнены технические проверки JSON, missing/extra, дубликатов, пустых значений, плейсхолдеров, кодов форматирования (§ и &), переносов строк, интерполяций и пробелов.

| Namespace | EN/RU | Missing | Extra | Duplicates | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|
| `akashictome` | 11/11 | 0 | 0 | 0 | 0 |
| `allthearcanistgear` | 28/28 | 0 | 0 | 0 | 0 |
| `allthecompressed` | 1 796/1 796 | 0 | 0 | 0 | 0 |
| `allthemodium` | 310/310 | 0 | 0 | 0 | 0 |
| `alltheores` | 516/516 | 0 | 0 | 0 | 0 |
| `allthetweaks` | 50/50 | 0 | 0 | 0 | 0 |
| `allthewizardgear` | 16/16 | 0 | 0 | 0 | 0 |
| `almostunified` | 6/6 | 0 | 0 | 0 | 0 |
| `amendments` | 316/316 | 0 | 0 | 0 | 0 |
| `apotheosis` | 802/802 | 0 | 0 | 0 | 0 |
| **Итого** | **3 851/3 851** | **0** | **0** | **0** | **0** |

27 совпадений RU=EN оставлены намеренно: названия модов и брендов, авторы картин, шаблоны плейсхолдеров, кнопка X и цветовое значение. Обычных непереведённых пользовательских строк среди совпадений не осталось.

Смысловые правки:
- Apotheosis: унифицировано обращение на «вы» в обучении, подсказках, описаниях аффиксов и достижениях; исправлена формулировка подсказки достижения; сохранены 20 завершающих пробелов в названии достижения, как в EN-оригинале.
- All The Tweaks: переведены два предупреждения о косметических функциях Valhelsia; бренд и смысл исходного сообщения сохранены.
- Глоссарий дополнен терминологией Apotheosis.

Коммиты: Apotheosis [423a2bd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/423a2bdbdab7c3a2ddfb130a64277193210fc10a), [65f0248](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/65f024888f80249bc5d54ce7a0bcef22cb58731c), [a758e5d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a758e5d9aa4ec6c0b5c1c2d7f9605edf43a6de8e); All The Tweaks [cf5c28c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cf5c28c31bf2364f8bf00dd2c24be2bcbe84d671); глоссарий [77d202e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/77d202e7eb82a6bece3317421472bdb1ee616463).


## Партия аудита JSON — 06.11.2026: Apothic и Ars addons

Проверены и завершены следующие 10 namespace. Для всех сверены EN/RU ключи и выполнены проверки JSON, missing/extra, дубликатов, пустых значений, плейсхолдеров, кодов форматирования (§ и &), переносов строк, интерполяций и начальных/конечных пробелов.

| Namespace | EN/RU | Missing | Extra | Duplicates | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|
| `apothic_attributes` | 161/161 | 0 | 0 | 0 | 0 |
| `apothic_enchanting` | 425/425 | 0 | 0 | 0 | 0 |
| `apothic_spawners` | 89/89 | 0 | 0 | 0 | 0 |
| `appflux` | 59/59 | 0 | 0 | 0 | 0 |
| `appleskin` | 22/22 | 0 | 0 | 0 | 0 |
| `appmek` | 15/15 | 0 | 0 | 0 | 0 |
| `aquaculture` | 291/291 | 0 | 0 | 0 | 0 |
| `ars_additions` | 235/235 | 0 | 0 | 0 | 0 |
| `ars_controle` | 83/83 | 0 | 0 | 0 | 0 |
| `ars_creo` | 18/18 | 0 | 0 | 0 | 0 |
| **Итого** | **1 398/1 398** | **0** | **0** | **0** | **0** |

144 совпадения RU=EN сохранены намеренно: названия и бренды, имена авторов и музыкальные композиции, римские обозначения уровней зачарования, FE/QIO, Shift/Ctrl, XNOR/XOR, служебный комментарий EMI и шаблоны с плейсхолдерами. Обычных непереведённых пользовательских строк среди совпадений не осталось.

Смысловые правки:
- Ars Additions: полностью переведены смешанные англо-русские описания Memory Crystal и Source Spawner, подсказка сохранения/загрузки, исправлен перевод Warp Index; название мода в группе предметов приведено к официальному написанию.
- Apothic Spawners: исправлено название корневого достижения, чтобы не показывать внутренний namespace.
- Ars Controle: описание пульта переписано естественно, термин radial menu согласован с глоссарием как «круговое меню».
- Глоссарий дополнен терминами Ars Additions, Ars Controle, Ars Creo, Memory Crystal, Source Spawner, Mob Jar и Warp Index.

Коммиты: Ars Additions [982b74b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/982b74b5d993da0c3d33b091c657e976c5daf587), [4257af8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4257af80ac6c60cf53cc8d096c4801a6fee2a843); Apothic Spawners [e57660d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e57660d082537663e188d6aca2495608cc491701); Ars Controle [afcf57c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/afcf57c68abbf6632e043af2605c199bfb23fe66); глоссарий [b6ed8fd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b6ed8fd7090f7ba478406ccc82dd13566d524df9), [f890452](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f890452656f803a89b5ee472bbb64ae9956b953a).


## JSON-аудит — партия после Ars Creo (06.11.2026)

Проверены 10 namespace: `ars_elemancy` (195), `ars_elemental` (668), `ars_ocultas` (10), `ars_technica` (169), `ars_unification` (11), `arseng` (17), `artifacts` (448), `auroral` (167), `auroras` (1), `balm` (36). Итого **1 722 ключа**.

Для всех файлов: JSON корректен; missing 0; extra 0; дубликаты 0; несовпадения плейсхолдеров, кодов форматирования, переносов строк и начальных/конечных пробелов — 0. Два пустых значения `ars_elemental.adv.desc.x` и `ars_elemental.adv.title.x` совпадают с пустыми значениями EN и сохранены. Остальные совпадения RU=EN относятся к названию мода, творческим вкладкам и шаблонам плейсхолдеров. Переводы не требовали изменений.

## JSON-аудит — следующая партия (06.11.2026)

Проверены 10 namespace: `bhc` (67), `bellsandwhistles` (39), `betteradvancedtooltips` (5), `betteradvancements` (1), `betterfortresses` (4), `bettermineshafts` (60), `betteroceanmonuments` (4), `betterstrongholds` (11), `betterwitchhuts` (4), `bigreactors` (522). Итого **717 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; дубликатов RU 0; пустых значений 0; несовпадений плейсхолдеров, форматирования, переносов строк и пробелов — 0. В EN-файле Big Reactors 31 повторное объявление ключа `_comment` (30 повторов одного служебного ключа); других повторяющихся ключей нет. В RU дубликатов нет.

В `bigreactors` переведены 13 ранее совпадавших с EN пользовательских значений: названия блоков и деталей энергизатора, а также подпись `Name:`. Оставшиеся совпадения относятся к названию мода, комментариям, числовым настройкам и техническим шаблонам. Добавлены термины Extreme Reactors в `GLOSSARY.md`.

Коммиты: перевод Big Reactors [64aa65e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/64aa65e1036b819ff400c362917d370cf7be4ca7); глоссарий [91bccf6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/91bccf6fb0b383c8d5c7f2f701e42977d043ee5) и последующее удаление повторной строки термина [d312883](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d3128835dddef70e1303370e1cae75baa0bbccbb).


## JSON-аудит — партия после Big Reactors (06.11.2026)

Проверены 10 namespace: `extremesoundmuffler` (78), `farmersdelight` (479), `fastbench` (7), `fluxnetworks` (123), `framedblocks` (436), `gateways` (96), `glassential` (155), `gmut` (11), `hostilenetworks` (279), `immeng` (4). Итого **1 668 ключей**.

Во всех файлах JSON корректен; missing 0; extra 0; дубликатов RU 0; пустых значений 1 (Hostile Neural Networks, совпадает с пустым EN); несовпадений плейсхолдеров 0. После исправлений переносы строк и пробелы совпадают с EN. В FramedBlocks сохранены 7 намеренно добавленных серых маркеров `§8` для обозначений направлений; это локальное оформление кратких обозначений, а не пропуск исходного форматирования. В EN Hostile Neural Networks 9 объявлений служебного ключа `_comment`; других дубликатов нет.

Исправлены лишние переносы и неточности в Hostile Neural Networks, восстановлен завершающий перенос в описании Gate Pearl, удалён лишний пробел и уточнено название сегмента шахматного куба в FramedBlocks. Глоссарий дополнен терминами Gateway, Gate Pearl, Data Model, Simulation, Framed Block и Checkered Cube.

Коммиты исправлений: FramedBlocks [36b1d42](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/36b1d42ae10035a07b52e11c230bd2a2295ad7cb), [fb74887](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fb74887bbcd2a0702285445d9b0b0c0bf35e8fe2); Gateways [d190753](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d190753758117d33ab676f3e3b51c36a5fc6b676); Hostile Neural Networks [f214cbc](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f214cbc8bfed1dafd265a06ccf20249d8d912e0a), [87494d1](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/87494d1a7e9214b92587bd7e650181d74dc601be), [8dafd63](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8dafd6385d8f0b43fa16bacb9dcdc1adadea0d06); глоссарий [a805b60](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a805b6080e5371cfa054e7b76f1f8723e7c26a57).


## JSON-аудит — партия после Immersive Energistics (06.11.2026)

Проверены 10 namespace: `immersiveengineering` (1 952), `ironjetpacks` (42), `jade` (410), `jei_mekanism_multiblocks` (103), `justenoughprofessions` (1), `keybindspurger` (4), `cataclysm` (735), `measurements` (15), `moderndynamics` (72), `modern_industrialization` (1 863). Итого **5 197 ключей**.

Во всех файлах JSON корректен; missing 0; extra 0; дубликатов RU 0; несовпадений плейсхолдеров, форматирования, переносов строк и пробелов — 0. Два пустых значения (Immersive Engineering `immersiveengineering.config.title` и Cataclysm `entity.cataclysm.rage_meter`) совпадают с EN. В EN Cataclysm дважды объявлен `maledictus_hurt.sub`: первое значение `Maledictus hurts`, последнее и фактически используемое — `Maledictus dies`; RU корректно переводит последнее значение как «Маледиктус умирает». В EN Measurements повторяется только служебный `_comment` (3 объявления). Других дубликатов нет.

В Cataclysm удалён лишний завершающий пробел в названии Abyss Portal. Глоссарий дополнен термином Abyss Portal.

Коммиты: Cataclysm [903d7cc](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/903d7cc3cce5dccb858f7a79bb49c14460f6c897); глоссарий [2897448](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2897448949ff6b2a8582f8b818099b190fb678ce).


## JSON-аудит — партия после Big Reactors: пропущенный блок B–C (06.11.2026)

Проверены 10 namespace: `biomeswevegone` (1 169), `blockui` (8), `bookshelf` (208), `botanypots` (238), `brandonscore` (102), `bridgingmod` (96), `buildinggadgets2` (112), `bwncr` (18), `cabletiers` (190), `caelus` (2). Итого **2 143 ключа**.

Во всех файлах JSON корректен; missing 0; extra 0; дубликатов EN/RU 0; несовпадений плейсхолдеров, форматирования, переносов строк и пробелов — 0. Семь пустых значений Bookshelf/Botany Pots совпадают с EN; это служебные разделители/метаданные и сохранены. Совпадения RU=EN относятся к названиям модов и музыкальных композиций, служебным комментариям, шаблонам форматирования и техническим идентификаторам. Переводы не требовали изменений.



## JSON-аудит — партия после Caelus (06.11.2026)

Проверены 10 namespace: `camol` (10), `charginggadgets` (5), `chisel` (2 774), `chromacarvings` (65), `cloudglass` (17), `cobblegengalore` (10), `codechickenlib` (18), `colorfulhearts` (14), `comforts` (83), `common_storage_lib` (3). Итого **2 999 ключей**.

Для всех файлов JSON корректен; missing 0; extra 0; duplicates EN/RU 0; empty 0; несовпадений плейсхолдеров, форматирования, переносов строк и пробелов — 0. Пять совпадений RU=EN относятся к названию Chisel, обозначению RF и техническому шаблону с плейсхолдером. Переводы не требовали изменений.



## JSON-аудит — партия после Common Storage Lib (06.11.2026)

Проверены 10 namespace: `commoncapabilities` (10), `compactmachines` (58), `connectedglass` (120), `constructionstick` (142), `controlling` (12), `cookingforblockheads` (260), `copycats` (67), `cosmeticarmorreworked` (5), `crafting_on_a_stick` (14), `craftingtweaks` (40). Итого **728 ключей**.

Во всех файлах JSON корректен; missing 0; extra 0; дубликатов RU 0; несовпадений плейсхолдеров, форматирования, переносов строк и пробелов — 0. В EN Common Capabilities три объявления служебного `_comment`, иных повторов нет. Три пустых значения Compact Machines, Construction Sticks и Crafting on a Stick совпадают с EN. В Cooking for Blockheads исправлены два значения: восстановлены экранированные последовательности `\\n` вместо обычных переносов строк, как в оригинале. Остальные совпадения RU=EN относятся к метаданным, плейсхолдерам и служебному обозначению `???`.

Коммит исправления Cooking for Blockheads: [5223759](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/522375983dbeb003719b937ad7ec01759c712396).


## JSON-аудит — партия после Crafting Tweaks (06.11.2026)

Проверены 10 namespace: `crashutilities` (4), `create` (3 639), `create_aquatic_ambitions` (39), `create_enchantment_industry` (593), `create_hypertube` (64), `createaddition` (292), `creeperoverhaul` (62), `cristellib` (4), `crystalix` (60), `curios` (48). Итого **4 805 ключей**.

Во всех файлах JSON корректен; missing 0; extra 0; duplicates EN/RU 0; несовпадений плейсхолдеров, форматирования, переносов строк и пробелов — 0. Семь пустых значений Create совпадают с EN. Проверка последовательности плейсхолдеров выполнена отдельно: несовпадений нет.

В `create_enchantment_industry` переведены **332 значения**, ранее полностью совпадавшие с EN; оставшиеся 4 совпадения — только технические шаблоны `%1$s: %2$s` и ` - %1$s`. В Create исправлены три расхождения пробелов в значениях. В Curios исправлен порядок непозиционных аргументов в двух сообщениях команд (число слотов, тип, получатель).

Коммиты: Create Enchantment Industry — [7d38e4d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7d38e4d82718b5ec9d5fd2293840b0429c5053ec), [3c14002](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/3c140029e8da5a6c3ed52c948819f8cfc10deafc), [2399885](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2399885320e7d9d41773e62a95d92fdc3ae35f80), [7cd1d6c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/7cd1d6c611f9e3bfb7f54d7b7a09dedda96bdfd5), [bdb5ac4](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bdb5ac47418f5b86983e225dd6a1b4a301334550), [23759ee](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/23759eeabfb0f3119424de610551fe5d6fcfd9ce); Create [ebce9d7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ebce9d7983f266e5eefb388ba62f5ad5fec83133); Curios [f2563b5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f2563b5cb0230a8e56c8534c6df9ecac3b0bbbf3), [9921f5d](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9921f5d7c878ca73eecf959d42845002f123d6da); глоссарий [9f96cd8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9f96cd8fcd9b490e71de53c87fc963029bb6e1a4).


## JSON-аудит — партия после Curios (06.11.2026)

Проверены 10 namespace: `darkmodeeverywhere` (24), `deeperdarker` (369), `dungeons_arise` (119), `easy_villagers` (32), `elevatorid` (29), `enderstorage` (8), `extendedae` (264), `enderdrives` (140), `endermanoverhaul` (135), `enderio` (608). Итого **1 728 ключей**.

Во всех файлах JSON корректен; missing 0; extra 0; duplicates EN/RU 0; empty 0; несовпадений плейсхолдеров, форматирования, переносов строк и пробелов — 0. В Ender IO переведены три оставшиеся пользовательские подписи слотов фильтров: Fluid Filter Slot, Item Filter Slot и Redstone Filter Slot. Оставшиеся совпадения RU=EN относятся к именам авторов, брендам, плейсхолдерам, числовым значениям и названиям собственных сущностей.

Коммиты: Ender IO [4f1d56b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4f1d56b283223434b20c2ef7541572db199ac09e); глоссарий [c3e9a24](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c3e9a24a11d2c1c1aa72ee553d71beea0ba08389).


## JSON-аудит — партия после Ender IO (06.11.2026)

Проверены 10 namespace: `farmingforblockheads` (55), `ftbchunks` (349), `ftbessentials` (94), `ftbfiltersystem` (65), `ftblibrary` (113), `ftbteams` (112), `ftbultimine` (89), `functionalstorage` (162), `fusion` (8), `mcwfurnitures` (661). Итого **1 708 ключей**.

Во всех файлах JSON корректен; missing 0; extra 0; duplicates EN/RU 0; empty 0; несовпадений плейсхолдеров, форматирования, переносов строк и пробелов — 0. В FTB Ultimine исправлен перенос строки в описании настройки обязательного инструмента. Два дополнительных английских файла `ftbjeiextras` и `ftbxmodcompat` содержат пустые JSON-объекты без языковых ключей и в десятку не включались. FTB Quests не затрагивался.

Коммит исправления FTB Ultimine: [e3dbc2e](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e3dbc2e3e1d133526319528848c437519f0023e6).


## JSON-аудит — партия после Macaw's Furniture (06.11.2026)

Проверены 10 namespace: `refurbished_furniture` (110), `guideme` (11), `handcrafted` (129), `jearchaeology` (44), `jei` (121), `jeistuff` (4), `journeymap` (1 398), `jupiter` (11), `justenoughbreeding` (5), `justzoom` (14). Итого **1 847 ключей**.

Во всех десяти файлах JSON корректен; missing 0; extra 0; duplicates EN/RU 0; empty 0; несовпадений плейсхолдеров, кодов форматирования, переносов строк и пробелов — 0. В JourneyMap переведены **819 пользовательских значений**, ранее полностью совпадавших с EN. Оставшиеся 49 совпадений относятся к брендам и доменам, осям координат, буквенным обозначениям цветовых каналов, единицам/форматам и техническим шаблонам. Остальные девять файлов не требовали правок.

Коммиты JourneyMap опубликованы в истории ветки [work/irons-spells-nov05](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commits/work/irons-spells-nov05); заключительная техническая коррекция [ab6d309](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ab6d3095d1cc13969053534faee9c1a5e5fce5f4). Глоссарий JourneyMap [e5064d6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e5064d64f5c3ee4ddf77c46fbe89d56d6e5973b8).


## JSON-аудит — партия после Just Zoom (06.11.2026)

Проверены 10 namespace: `keybindbundles` (26), `kubejstweaks` (4), `laserbridges` (11), `laserio` (95), `lionfishapi` (4), `little_big_redstone` (312), `livingthings` (106), `logisticsnetworks` (729), `lootr` (249), `luminax` (193). Итого **1 729 ключей**.

Во всех файлах JSON корректен; missing 0; extra 0; duplicates EN/RU 0; empty 0; несовпадений плейсхолдеров, форматирования, переносов строк и пробелов — 0. Совпадения RU=EN относятся к названиям модов, техническим сокращениям и идентификаторам, плейсхолдерам, числовым/логическим символам и обозначениям интеграций (AE2, RS, NBT). Переводы не требовали изменений.

## JSON-аудит — партия после Luminax (06.11.2026)

Проверены **10/10 namespace**, всего **3 918 ключей**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Duplicates | Empty RU | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|---:|
| mahoutsukai | 1 931/1 931 | 0 | 0 | 0 | 81 (совпадают с EN) | 0 |
| mcjtylib | 3/3 | 0 | 0 | 0 | 0 | 0 |
| mcwbridges | 156/156 | 0 | 0 | 0 | 0 | 0 |
| mcwdoors | 288/288 | 0 | 0 | 0 | 0 | 0 |
| mcwholidays | 338/338 | 0 | 0 | 0 | 0 | 0 |
| mcwlights | 146/146 | 0 | 0 | 0 | 0 | 0 |
| mcwfences | 184/184 | 0 | 0 | 0 | 0 | 0 |
| mcwpaths | 318/318 | 0 | 0 | 0 | 0 | 0 |
| mcwstairs | 228/228 | 0 | 0 | 0 | 0 | 0 |
| mcwwindows | 326/326 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **3 918/3 918** | **0** | **0** | **0** | **81 = EN** | **0** |

Во всех десяти файлах JSON корректен; ключи, дубликаты, плейсхолдеры, коды форматирования (§ и &), переносы строк, экранированные переносы и начальные/конечные пробелы проверены. В Mahou Tsukai осталось 14 непустых совпадений RU=EN: название мода, имена/обозначения, пунктуация и буквенные подписи цветовых каналов; пользовательских английских строк не осталось. В McJtyLib два совпадения — служебный _comment и название библиотеки. В остальных восьми namespace точных совпадений с EN нет.

Смысловые исправления:
- Mahou Tsukai: удалён лишний ключ emi.category.mahoutsukai; исправлены два лишних плейсхолдера в Fame/Style; согласованы Caliburn, Borrowed Authority, Rho Aias и названия нескольких техник/эффектов.
- Macaw's Windows: Window Key исправлено на «Ключ для окна» по описанию предмета — он запирает окна.
- Глоссарий дополнен терминологией Mahou Tsukai и Macaw's mods.

Коммиты:
- Mahou Tsukai: перевод [26f8fc0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/26f8fc007bfebe544363e5d9782ff20da8cc6a8b), глоссарий [9859cc3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9859cc3ccbbb9d14fc22b1b90fbd37c76100e484).
- Macaw's Windows: перевод [c0b64dd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c0b64ddd06df2eb03c8870189a739d709734ab82), глоссарий [58b2e98](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/58b2e980a733ef98ba606e5a40d2262543206db4).

Примечание по Mahou Tsukai: в исходном архиве также присутствует legacy-файл en_us.lang с 678 уникальными ключами, отсутствующими в актуальном en_us.json. В ru_ru.json эти записи не переносились; использование legacy-файла в версии ATM10 1.21.1 отдельно не подтверждено.

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия начинается после mcwwindows: mcwroofs, mcwtrpdoors, megacells, mekanismcovers, mekanisticrouters, memorysettings, merequester, merrymaking, mffs, mifa. Ранее завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## JSON-аудит — партия после Mifa (06.11.2026)

Проверены **10/10 namespace**, всего **1 657 ключей**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Duplicates RU | Empty RU | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|---:|
| mcwroofs | 610/610 | 0 | 0 | 0 | 0 | 0 |
| mcwtrpdoors | 201/201 | 0 | 0 | 0 | 0 | 0 |
| megacells | 134/134 | 0 | 0 | 0 | 0 | 0 |
| mekanismcovers | 3/3 | 0 | 0 | 0 | 0 | 0 |
| mekanisticrouters | 13/13 | 0 | 0 | 0 | 0 | 0 |
| memorysettings | 8/8 | 0 | 0 | 0 | 0 | 0 |
| merequester | 27/27 | 0 | 0 | 0 | 0 | 0 |
| merrymaking | 472/472 | 0 | 0 | 0 | 1 (совпадает с EN) | 0 |
| mffs | 186/186 | 0 | 0 | 0 | 0 | 0 |
| mifa | 3/3 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **1 657/1 657** | **0** | **0** | **0** | **1 = EN** | **0** |

Во всех десяти файлах JSON корректен; пропущенных/лишних ключей, дубликатов RU, несовпадений плейсхолдеров, форматирования, переносов строк и начальных/конечных пробелов нет. В EN Merrymaking один ключ повторён с одинаковым значением; RU содержит его один раз. Пустое значение Merrymaking совпадает с EN. Совпадения RU=EN: пустая строка Merrymaking и технические обозначения Shift/MFFS в MFFS.

Смысловые и технические исправления:
- MegaCells: MEGA Crafting Co-Processing Unit переведён как «Мега-сопроцессор крафта».
- Mekanistic Routers: восстановлена точная последовательность кодов форматирования в подсказке Chemical Refill Module.
- Memory Settings: восстановлен начальный пробел в строке, которая начинается с пробела в EN.
- ME Requester: в беспроводных терминалах восстановлено обозначение МЭ.
- Merrymaking: исправлено согласование рода/числа для кожаных, железных и алмазных предметов; возвращён смысл Ugly Christmas Sweater; восстановлены начальные пробелы у трёх каминных полок.
- MFFS: Fortron унифицирован как «Фортрон»; Warp в разрешениях прохода через силовые поля больше не переводится как телепортация; восстановлены завершающие пробелы двух подписей.
- Глоссарий дополнен терминами AE2, Mekanism, MFFS и Merrymaking.

Коммиты:
- MegaCells [addd475](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/addd475bab0bc2a977eeaffb379d5607cefb5bb6).
- Mekanistic Routers [e597e87](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e597e8712f611a7cd413d249f6db5477d1f6a10b), [e85eb01](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e85eb01d30e3b97970f542338617d3f8ab32331c).
- Memory Settings [9e329e4](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9e329e4d04764ec4642d158bbc4a93eff6e4d496).
- ME Requester [9120c52](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/9120c52c6fe50f0ada44ae0a400e03834508be03).
- Merrymaking [38a53dc](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/38a53dcff5f807841a720556a84ae799c245e813), [b20f1cd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b20f1cd2f088287097996a8a84928e6ae623d8c9), [cc3ad21](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cc3ad21ca85ee3123cb92a405c64642d6b198c18).
- MFFS [a8eb5f8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a8eb5f8cecc96ab7a954912c2f4bef354729dc60), [988d6a8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/988d6a8975ffaeaac16d35b8a2206e9d51915f5e).
- Глоссарий [5fb453b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5fb453b56630d2d1343e9b50b1e4a7a6d20c984f), [6704118](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/67041181eda9efeed639cbf98770896bd6437039).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия: minecolonies, mininggadgets, mob_grinding_utils, modernfix, modonomicon, modularrouters, modularbees, mes, mns, mss. Ранее завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## JSON-аудит — партия после Mifa, продолжение (06.11.2026)

Проверены **10/10 namespace**, всего **4 994 ключа**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Duplicates RU | Empty RU | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|---:|
| minecolonies | 3 925/3 925 | 0 | 0 | 0 | 0 | 0 |
| mininggadgets | 85/85 | 0 | 0 | 0 | 0 | 0 |
| mob_grinding_utils | 146/146 | 0 | 0 | 0 | 0 | 0 |
| modernfix | 155/155 | 0 | 0 | 0 | 2 (совпадают с EN) | 0 |
| modonomicon | 232/232 | 0 | 0 | 0 | 1 (совпадает с EN) | 0 |
| modularrouters | 371/371 | 0 | 0 | 0 | 2 (совпадают с EN) | 0 |
| modularbees | 59/59 | 0 | 0 | 0 | 0 | 0 |
| mes | 7/7 | 0 | 0 | 0 | 0 | 0 |
| mns | 7/7 | 0 | 0 | 0 | 0 | 0 |
| mss | 7/7 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **4 994/4 994** | **0** | **0** | **0** | **5 = EN** | **0** |

Во всех десяти файлах JSON корректен; пропусков/лишних ключей, дубликатов RU, несовпадений плейсхолдеров, кодов форматирования, переносов строк и начальных/конечных пробелов нет. В EN Mob Grinding Utils повторяется служебный ключ _comment (10 объявлений); эффективное последнее значение — Item Tool tips, RU содержит его перевод «Подсказки предметов». Пять пустых значений ModernFix/Modonomicon/Modular Routers совпадают с EN. Совпадения RU=EN в остальных файлах — бренды, технические шаблоны, единицы, символы операторов и смайлик.

Смысловые и технические исправления:
- Modular Routers: переведены оставшиеся пользовательские строки модулей энергии, фильтров, регуляторов и защиты; допереведены подсказки принудительного слива, защиты и вакуумного модуля; восстановлены все исходные переносы строк и форматирование.
- MineColonies: исправлены шесть расхождений начальных/конечных пробелов в сообщениях и длинных подсказках.
- Mob Grinding Utils: переведён служебный комментарий, соответствующий последнему повторяющемуся _comment в EN.
- ModernFix: переписано описание кэширования состояний блоков и восстановлен пропущенный абзац.
- Глоссарий дополнен терминами Modular Routers и Blockstate.

Коммиты:
- Modular Routers: [c400bd5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c400bd551ce455078c04e8cdb54e23b3629394ce), [4f2964c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4f2964c75f47603c2b773f253f053df76ca55aa0).
- MineColonies: [87d8bf6](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/87d8bf6dfcfdd74cf933795f3320ff2a85ba0a38).
- Mob Grinding Utils: [2cb4b64](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/2cb4b64ac6f62d14e2528f23d84d7013e554249f).
- ModernFix: [788024a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/788024ac9fede2b6bec4117cda97378ec8f3a277).
- Глоссарий: [6b5515c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6b5515c3074bddf54f656e18575040010730a61b), [8c1ad18](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8c1ad185cc02d9d1548a43eea93e97d9838d1403), [ae1ab43](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/ae1ab43b0222a30682fa605904021ecf0cf4b241).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия после mss: moogs_structures, mvs, moonlight, moreoverlays, morered, mostructures, multipiston, mysticalagradditions, mysticalagriculture, naturesaura. Ранее завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## JSON-аудит — партия после MNS (06.11.2026)

Проверены **10/10 namespace**, всего **1 497 ключей**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Duplicates RU | Empty RU | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|---:|
| moogs_structures | 14/14 | 0 | 0 | 0 | 0 | 0 |
| mvs | 7/7 | 0 | 0 | 0 | 0 | 0 |
| moonlight | 265/265 | 0 | 0 | 0 | 0 | 0 |
| moreoverlays | 40/40 | 0 | 0 | 0 | 0 | 0 |
| morered | 51/51 | 0 | 0 | 0 | 0 | 0 |
| mostructures | 27/27 | 0 | 0 | 0 | 0 | 0 |
| multipiston | 2/2 | 0 | 0 | 0 | 0 | 0 |
| mysticalagradditions | 104/104 | 0 | 0 | 0 | 0 | 0 |
| mysticalagriculture | 745/745 | 0 | 0 | 0 | 0 | 0 |
| naturesaura | 242/242 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **1 497/1 497** | **0** | **0** | **0** | **0** | **0** |

Во всех десяти файлах JSON корректен; пропусков/лишних ключей, дубликатов, несовпадений плейсхолдеров, кодов форматирования, переносов строк и начальных/конечных пробелов нет. 21 совпадение RU=EN — названия модов/сервисов, координатные обозначения, числовые уровни и технические шаблоны.

Смысловые исправления:
- Mystical Agradditions: согласованы названия пяти ресурсных уровней и Inferium Ore с терминологией Mystical Agriculture.
- Mystical Agriculture: исправлены род/число в названиях Prudentium Shovel, Prudentium Boots и Imperium Boots; удалены два лишних завершающих пробела.
- Nature's Aura: Ancient Log переведено как «Древнее бревно», а не «Древнее дерево».
- Глоссарий дополнен ресурсными уровнями Mystical Agriculture.

Коммиты:
- Mystical Agradditions [00dfc30](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/00dfc300d95d2ed3095374efadef68107d307bc9).
- Mystical Agriculture [c975d3a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c975d3a0b00d21a8d78517bda1e39131f1b5cb6e), [795fd3a](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/795fd3a54db0c6f7700600ee510f89b01ce3aec4).
- Nature's Aura [a959245](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a9592457d1a721de736a1dccefa61b09be3a9fd2).
- Глоссарий [dbadc93](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/dbadc93e7ffb574d9bfe6f21590a14785a45360c).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия после naturesaura: neo_auth, nochatreports, notenoughanimations, not_enough_glyphs, observable, oracle_index, owo, pamhc2crops, pamhc2foodcore, pamhc2foodextended. Nature's Compass, NeoVitae, Occultism, Biomes We've Gone, Oritech и PneumaticCraft уже завершены и пропускаются. FTB Quests/SNBT оставить на заключительный этап.

## JSON-аудит — партия после Nature's Aura (06.11.2026)

Проверены **10/10 namespace**, всего **2 030 ключей**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Duplicates RU | Empty RU | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|---:|
| neo_auth | 45/45 | 0 | 0 | 0 | 0 | 0 |
| nochatreports | 129/129 | 0 | 0 | 0 | 0 | 0 |
| notenoughanimations | 107/107 | 0 | 0 | 0 | 0 | 0 |
| not_enough_glyphs | 249/249 | 0 | 0 | 0 | 1 (совпадает с EN) | 0 |
| observable | 34/34 | 0 | 0 | 0 | 0 | 0 |
| oracle_index | 46/46 | 0 | 0 | 0 | 0 | 0 |
| owo | 25/25 | 0 | 0 | 0 | 0 | 0 |
| pamhc2crops | 320/320 | 0 | 0 | 0 | 0 | 0 |
| pamhc2foodcore | 203/203 | 0 | 0 | 0 | 0 | 0 |
| pamhc2foodextended | 872/872 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **2 030/2 030** | **0** | **0** | **0** | **1 = EN** | **0** |

Во всех десяти файлах JSON корректен; пропусков/лишних ключей, дубликатов верхнего уровня, несовпадений плейсхолдеров, кодов форматирования, переносов строк и начальных/конечных пробелов нет. В OWO сохранена структура JSON-компонентов и индексные плейсхолдеры. Единственное пустое значение Not Enough Glyphs совпадает с EN. 17 совпадений RU=EN — названия брендов/модов, технические идентификаторы, клавиши, алгоритмы, числовые/структурные шаблоны.

Смысловое/техническое исправление:
- No Chat Reports: в 12 строках заменены буквальные последовательности \\n на настоящие переносы строк, как в EN; теперь все переносы совпадают.
- Глоссарий дополнен терминами Pam's HarvestCraft.

Коммиты:
- No Chat Reports [d07da48](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d07da48559be4f0b4e7e064d31674aa87d6dd9bc).
- Глоссарий [8f098d5](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/8f098d567b89e46220b4e04fb5b5250faf73965c).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия после pamhc2foodextended: pamhc2trees, patchouli, pipez, placebo, pocketstorage, polylib, polymorph, potionsmaster, productivebees и productivemetalworks. Productive Bees ранее уже переводился; не перезаписывать существующие значения, только сверить и исправить подтверждённые ошибки. FTB Quests/SNBT оставить на заключительный этап.

## JSON-аудит — партия после Pam's HarvestCraft Food Extended (06.11.2026)

Проверены **10/10 namespace**, всего **1 899 ключей**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Duplicates RU | Empty RU | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|---:|
| pamhc2trees | 158/158 | 0 | 0 | 0 | 0 | 0 |
| patchouli | 92/92 | 0 | 0 | 0 | 0 | 0 |
| pipez | 83/83 | 0 | 0 | 0 | 0 | 0 |
| placebo | 6/6 | 0 | 0 | 0 | 0 | 0 |
| pocketstorage | 28/28 | 0 | 0 | 0 | 0 | 0 |
| polylib | 13/13 | 0 | 0 | 0 | 0 | 0 |
| polymorph | 3/3 | 0 | 0 | 0 | 0 | 0 |
| potionsmaster | 15/15 | 0 | 0 | 0 | 0 | 0 |
| productivebees | 1 125/1 125 | 0 | 0 | 0 | 0 | 0 |
| productivemetalworks | 376/376 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **1 899/1 899** | **0** | **0** | **0** | **0** | **0** |

Во всех десяти файлах JSON корректен; пропусков/лишних ключей, дубликатов, несовпадений плейсхолдеров, форматирования, переносов строк и начальных/конечных пробелов нет. 16 совпадений RU=EN — названия модов, технические идентификаторы, клавиши и плейсхолдеры.

Смысловые и технические исправления:
- Productive Bees: полностью локализованы названия 117 продвинутых ульев и 117 расширителей ульев, включая породы древесины из BYG, Regions Unexplored и других интеграций; исправлены инструкции Shift, названия достижений и подсказки.
- Pipez: согласованы названия пяти уровней улучшения труб и инструмента задания назначения фильтра.
- Placebo: Supporter Trails/Wings переведены как спонсорские косметические эффекты.
- Pam's HarvestCraft Trees: восстановлены три завершающих пробела в названиях саженцев.
- Глоссарий дополнен терминами Productive Bees, Pipez и Placebo.

Коммиты:
- Productive Bees [f7fa64c](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f7fa64c66fa40d78093fbfba148858696dfff573), [c62cb6b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/c62cb6bbf267d04e5d09cf28079a9963f18730b5).
- Pipez [311aae7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/311aae7c4f7b55de5814a4ca12684191b33d2411).
- Placebo [a10a081](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/a10a0816e7d7f525b9062b6ea8535b6a8149e5e4).
- Pam's HarvestCraft Trees [cd33c14](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/cd33c14c752157f1dc910c211c7115c0b8462255).
- Глоссарий [d0c2ecd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d0c2ecdd5cd4a246db21d4c025a1ac9de8de648a), [6ed7ef1](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/6ed7ef1066ba364d91882c2265e95831d3257cbf).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия после productivemetalworks: rangedpumps, rechiseledcreate, redstonepen, refinedtypes, refinedfluidsubstitution, refinedstorage_curios_integration, refinedstorage_jei_integration, refinedstorage_mekanism_integration, refinedstorage, refinedstorage_quartz_arsenal. Ранее завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## JSON-аудит — партия после Productive Metalworks (06.11.2026)

Проверены **10/10 namespace**, всего **1 349 ключей**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Duplicates RU | Empty RU | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|---:|
| rangedpumps | 9/9 | 0 | 0 | 0 | 0 | 0 |
| rechiseledcreate | 243/243 | 0 | 0 | 0 | 0 | 0 |
| redstonepen | 72/72 | 0 | 0 | 0 | 0 | 0 |
| refinedtypes | 164/164 | 0 | 0 | 0 | 0 | 0 |
| refinedfluidsubstitution | 3/3 | 0 | 0 | 0 | 0 | 0 |
| refinedstorage_curios_integration | 1/1 | 0 | 0 | 0 | 0 | 0 |
| refinedstorage_jei_integration | 10/10 | 0 | 0 | 0 | 0 | 0 |
| refinedstorage_mekanism_integration | 37/37 | 0 | 0 | 0 | 0 | 0 |
| refinedstorage | 788/788 | 0 | 0 | 0 | 0 | 0 |
| refinedstorage_quartz_arsenal | 22/22 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **1 349/1 349** | **0** | **0** | **0** | **0** | **0** |

Во всех десяти файлах JSON корректен; пропусков/лишних ключей, дубликатов, несовпадений плейсхолдеров, форматирования, переносов строк и начальных/конечных пробелов нет. 12 совпадений RU=EN — названия модов/интеграций, JEI, клавиши/технические идентификаторы и шаблон плейсхолдеров.

Смысловые и технические исправления:
- Redstone Pen: в трёх длинных подсказках RLC выровнены количество переносов строк и последовательности кодов форматирования.
- Refined Storage: переведены десять оставшихся пользовательских строк (приоритеты хранения, сочетания клавиш, настройки энергии и подсказки); исправлены три лишних переноса строк в описаниях.
- Глоссарий дополнен терминами Refined Storage.

Коммиты:
- Redstone Pen [15732cd](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/15732cdd82eda464e288e88f0c7905afffeea311).
- Refined Storage [d42aa73](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d42aa738c30c9e9000cb5379299e9d68985c6df8), [4274337](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4274337b955cae44af83dd53b21477cdc3e529c1).
- Глоссарий [edb01da](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/edb01dae26cac69495c4635a5ea354f065584f13).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия после refinedstorage_quartz_arsenal: rsinsertexportupgrade, reliquified_artifacts, repeatable_trial_vaults, repurposed_structures, resourcefulconfig, restrictions, rftoolsbase, rftoolsbuilder, rftoolspower, rftoolsstorage. Ранее завершённые namespace пропускать. FTB Quests/SNBT оставить на заключительный этап.

## JSON-аудит — партия после Refined Storage Quartz Arsenal (06.11.2026)

Проверены **10/10 namespace**, всего **1 078 ключей**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Duplicates RU | Empty RU | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|---:|
| rsinsertexportupgrade | 44/44 | 0 | 0 | 0 | 0 | 0 |
| reliquified_artifacts | 572/572 | 0 | 0 | 0 | 0 | 0 |
| repeatable_trial_vaults | 1/1 | 0 | 0 | 0 | 0 | 0 |
| repurposed_structures | 163/163 | 0 | 0 | 0 | 0 | 0 |
| resourcefulconfig | 28/28 | 0 | 0 | 0 | 0 | 0 |
| restrictions | 12/12 | 0 | 0 | 0 | 0 | 0 |
| rftoolsbase | 55/55 | 0 | 0 | 0 | 0 | 0 |
| rftoolsbuilder | 97/97 | 0 | 0 | 0 | 0 | 0 |
| rftoolspower | 65/65 | 0 | 0 | 0 | 0 | 0 |
| rftoolsstorage | 41/41 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **1 078/1 078** | **0** | **0** | **0** | **0** | **0** |

Во всех десяти файлах JSON корректен; пропусков/лишних ключей, дубликатов, несовпадений плейсхолдеров, форматирования, переносов строк и начальных/конечных пробелов нет. Пять совпадений RU=EN — названия модов/категорий и техническая подпись UUID.

Исправление:
- Reliquified Artifacts: в описании Shock Pendant восстановлен правильный порядок позиционных плейсхолдеров %2$s и %3$s (дальность и число перескоков).

Коммит:
- Reliquified Artifacts [b5f8ba3](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/b5f8ba34bc9d8f47bbf172129806dc4945b6d43e).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия после rftoolsstorage: rftoolsutility, rootsclassic, sawmill, searchables, sgearmetalworks, shiny, shrink, silentlib, silentgems и simplebackups. Silent Gear уже завершён и пропускается. FTB Quests/SNBT оставить на заключительный этап.

## JSON-аудит — партия после RFTools Storage (06.11.2026)

Проверены **10/10 namespace**, всего **1 178 ключей**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Duplicates RU | Empty RU | Placeholder / format / newline / whitespace |
|---|---:|---:|---:|---:|---:|---:|
| rftoolsutility | 242/242 | 0 | 0 | 0 | 0 | 0 |
| rootsclassic | 483/483 | 0 | 0 | 0 | 2 (совпадают с EN) | 0 |
| sawmill | 8/8 | 0 | 0 | 0 | 0 | 0 |
| searchables | 1/1 | 0 | 0 | 0 | 0 | 0 |
| sgearmetalworks | 132/132 | 0 | 0 | 0 | 0 | 0 |
| shiny | 137/137 | 0 | 0 | 0 | 0 | 0 |
| shrink | 12/12 | 0 | 0 | 0 | 0 | 0 |
| silentlib | 5/5 | 0 | 0 | 0 | 0 | 0 |
| silentgems | 118/118 | 0 | 0 | 0 | 0 | 0 |
| simplebackups | 40/40 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **1 178/1 178** | **0** | **0** | **0** | **2 = EN** | **0** |

Во всех десяти файлах JSON корректен; пропусков/лишних ключей, дубликатов, несовпадений плейсхолдеров, форматирования, переносов строк и пробелов нет. Два пустых значения Roots Classic совпадают с EN. Шесть совпадений RU=EN — название Roots Classic, плейсхолдер, save-all/Mc2Discord и технические обозначения.

Исправление:
- Roots Classic: удалён лишний начальный пробел в заголовке страницы Wildwood Boots.

Коммит:
- Roots Classic [51e15d7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/51e15d76edd4c431bd998535f0c375cbcd742327).

Работа опубликована в work/irons-spells-nov05; main не изменялся. Следующая партия после simplebackups: simplemagnets, simple_weather, simplylight, smithingtemplateviewer, solcarrot, sophisticatedbackpacks, sophisticatedcore, sophisticatedstorageinmotion и soulplied_energistics, starbunclemania. Sophisticated Storage уже завершён и пропускается. FTB Quests/SNBT оставить на заключительный этап.


## Сверка альтернативной партии work/atm10-batch-nov05 — 06.11.2026

Пять JSON-файлов сравнивались с актуальными EN-оригиналами и текущим main. Все ключи покрыты полностью; альтернативная ветка не содержит дополнительных ключей. В main оставлены более точные текущие формулировки, а подтверждённые улучшения из batch перенесены выборочно. Само слияние batch целиком не выполнялось.

| Namespace | EN/RU | Missing | Extra | Duplicates | Placeholder mismatch | Format-token mismatch |
|---|---:|---:|---:|---:|---:|---:|
| evilcraft | 629/629 | 0 | 0 | 0 | 0 | 0 |
| integrateddynamics | 1854/1854 | 0 | 0 | 0 | 0 | 0 |
| irons_spellbooks | 1315/1315 | 0 | 0 | 0 | 0 | 0 |
| pneumaticcraft | 2274/2274 | 0 | 0 | 0 | 0 | 0 |
| reliquary | 551/551 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **6623/6623** | **0** | **0** | **0** | **0** | **0** |

Отобранные смысловые и терминологические улучшения зафиксированы в `PROJECT_HANDOFF.md`. Все пять JSON успешно разобраны; повторная проверка ключей, плейсхолдеров и форматирующих токенов прошла без расхождений.


## Смысловая вычитка и повторный JSON-аудит — 06.11.2026

Завершена партия из 10 namespace (1197 ключей): simplemagnets 38, simple_weather 19, simplylight 192, smithingtemplateviewer 1, solcarrot 60, sophisticatedbackpacks 407, sophisticatedcore 318, sophisticatedstorageinmotion 8, soulplied_energistics 4, starbunclemania 150.

| Namespace | EN/RU | Missing | Extra | Duplicates | Empty mismatch | Placeholder/order | Formatting | Newlines | Edge whitespace |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| simplemagnets | 38/38 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| simple_weather | 19/19 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| simplylight | 192/192 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| smithingtemplateviewer | 1/1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| solcarrot | 60/60 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| sophisticatedbackpacks | 407/407 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| sophisticatedcore | 318/318 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| sophisticatedstorageinmotion | 8/8 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| soulplied_energistics | 4/4 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| starbunclemania | 150/150 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| **Итого** | **1197/1197** | **0** | **0** | **0** | **0** | **0** | **0** | **0** | **0** |

JSON корректен во всех файлах. Плейсхолдеры проверены с учётом позиционных индексов, форматирующие коды, переносы строк и начальные/конечные пробелы совпадают с EN. Одно пустое значение StarbuncleMania совпадает с EN и намеренно оставлено пустым.

Смысловые исправления внесены в Simply Light, Simple Weather, SoL Carrot, Sophisticated Backpacks, Sophisticated Core и StarbuncleMania; остальные четыре namespace проверены, смысловых правок не потребовали. Подробности и коммиты приведены в последней записи PROJECT_HANDOFF.md.

Следующая очередь из незавершённых RU/EN namespace: stepcrafter, storagedelight, structurize, supermartijn642corelib, sushigocrafting, terrablender, the_bumblezone, theurgy, tiab, titanium. Не повторять stevescarts, supplementaries, tempad и tempad_static: они уже проверены ранее.


## Контрольная точка вычитки — 06.11.2026

После завершения первой партии (10 namespace / 1197 ключей; см. предыдущую запись) начата следующая десятка. В main подтверждены смысловые правки в stepcrafter, storagedelight, structurize, sushigocrafting, the_bumblezone, theurgy и titanium. Коммиты и краткие описания приведены в PROJECT_HANDOFF.md. Это частичная работа: следующая десятка не объявляется завершённой, повторный полный технический аудит ещё не зарегистрирован. По supermartijn642corelib, terrablender и tiab закрытие работ не подтверждено.

Для Theurgy внесены крупные смысловые исправления аппаратов, алхимической терминологии, чанов, руководства и гадательных жезлов. Финальный аудит внутренних ссылок/разметки и полный повторный JSON-аудит остаются незавершёнными.

При продолжении: сначала проверить свежие main и GLOSSARY.md; закончить Theurgy, затем вычитать и проверить всю текущую десятку. Не повторять уже сделанные правки. Dropbox не изменялся.


## Полная вычитка — партия stepcrafter—titanium (06.11.2026)

Завершена партия **10/10 namespace, 5 205 ключей**. Все файлы сверены с актуальными EN-оригиналами из ATM/LANGUAGES_EN_US.

| Namespace | EN/RU | Missing | Extra | Дубликаты | Плейсхолдеры | Форматирование | Переносы | Краевые пробелы |
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

Во всех файлах JSON корректен; ключи, плейсхолдеры и их порядок, коды форматирования, количество переносов строк, краевые пробелы и пустые значения относительно EN совпадают. Для Theurgy и The Bumblezone дополнительно проверены ссылки item://, entry://, category://; расхождений нет.

Смысловые правки: StepCrafter — улучшение слотов; Storage Delight — блоки кухни и древесные варианты; Structurize — сканирование, схемы и конфигурация; Sushi Go Crafting — пищевая терминология; The Bumblezone — существа, мёд, соты с расплодом, эффекты, конфигурации, совместимость и торговые теги; Theurgy — аппараты, нитер, сера, реформация, трансмутация, гадательные жезлы, ртутная логистика и названия исходных материалов; Titanium — подсказки резервуара и тестовый блок. SuperMartijn642CoreLib, TerraBlender и TIAB проверены, правки не потребовались.

Коммиты и подробности приведены в последней записи PROJECT_HANDOFF.md. Глоссарий дополнен терминами Theurgy и The Bumblezone (коммит [f2d3579](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/f2d35794e753de50d7b8dd93ca782364291e084c)).

### Следующая очередь

После titanium и пропуска уже завершённого Twilight Forest следующая десятка по дереву английских источников: toastcontrol, tombstone, toolbelt, torchmaster, transfer_labels, trashcans, trashslot, treetap, trophymanager, universalgrid. Все десять RU JSON уже существуют; первичная сверка показывает совпадение наборов ключей с EN. Следующая работа — смысловая вычитка и полный повторный технический аудит, не создание файлов заново. После universalgrid идут utilitarian, utilityvest.
