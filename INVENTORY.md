# Инвентаризация локализаций ATM10

Дата сверки: **05.11.2026**  
Версия официальной сборки: **ATM10 8.5**  
Источник списка модов: [AllTheMods/ATM-10](https://github.com/AllTheMods/ATM-10), `config/crash_assistant/modlist.json`, ветка `main`.  
Базовый снимок русских файлов: ветка `main` репозитория `d1gorae/ATM10-RU-TRANSLATE`, пути `assets/<namespace>/lang/ru_ru.json`. Дополнения текущей рабочей партии отмечены отдельными разделами ниже и находятся в `work/productivetrees-ru`.

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
| Supplementaries | 1394 | 708 | 686 |
| Regions Unexplored | 933 | 455 | 478 |
| **Итого** | **13018** | **11854** | **1164** |

Пять модов из этой очереди полностью переведены и проверены: NeoVitae, Mekanism, Ice and Fire, Mekanism Tools и Silent Gear. Supplementaries и Regions Unexplored остаются незавершёнными. Эти семь модов не объявляются полной партией из десяти.



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

Финальная сверка с read-only EN-файлом `silent-gear-1.21.1-neoforge-4.2.1.1/silentgear/en_us.json` (SHA `458a50aed74a049d099ab97bf14723b0fb91dc1b`): JSON корректен; EN/RU 1 191/1 191; missing 0; extra 0; дубликаты ключей 0; несовпадения плейсхолдеров 0; несовпадения кодов форматирования Minecraft (§) 0; несовпадения количества переносов строк 0. Девять буквенных/ранговых обозначений grade (A–E, S–SSS, MAX) оставлены без перевода намеренно. Внутриигровое тестирование не проводилось.

Коммиты перевода: [4ae2a83](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/4ae2a83cde5048aea1fc242a42b03adbd30ae04f), [5269ad8](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/5269ad88435aae15f3035ecd3aec35515e5fd185), [eaa0f20](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/eaa0f204c8d59459a3933f3ea5e4163135e8fc02), [e135d5b](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/e135d5b417c92e23b69414837ed8a21effd11f0e), [fa0a4f0](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/fa0a4f092ffb0414554c66329d7e621e1a729665), [d80af99](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/d80af9995dfb5d98442ca28ac25391bf684332b3), [0a44d35](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/0a44d3596f2bcb55d8d0ab41fa8b0e25610cd67c), [28e31bb](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/28e31bb921f5dc0bda0762c7ba309005e9645391), [bd843c7](https://github.com/d1gorae/ATM10-RU-TRANSLATE/commit/bd843c72bd123a157d4b03a2fc9c383e45651544).

Работа опубликована только в рабочей ветке; `main` не изменялся. Следующая точка очереди — Supplementaries, затем Regions Unexplored. FTB Quests/SNBT остаются на финальном этапе.
